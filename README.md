# Learning Resources for Data Scientist

## About this document

### What is it?

- A **curated** and **opinionated** list of the learning resources for **data scientist**.
  - During my professional career, I have always been thinking what can I learn to improve myself. While there are a lot of resources on the internet, deciding what resources to learn with my limited amount time can yield the highest return is actually a time consuming process.
  - This document is the resources/classes that I think can help improve myself as a data scientist, which **may or may not** work for you.
  - When I use the word **data scientist**, I actually refer to the union of data analysts, data scientists, and data engineers. See [What is a data scientist](#what-is-a-data-scientist) for my viewpoint.
- Focus more on technical skill, and less on soft (people) or management skill.

### Who is this document for?

While I create this document for my own learning purpose, this document is also suited for

1. anyone who is currently a data scientists and wants to improve himself/herself
2. anyone who is not a data scientist but wants to step into the data scientist world

#### Prerequisite expectation

I expect the reader to has basic skills in statistics, machine learning,
and programming. If you have a BS or MS degree in STEM, then you should have the
prerequisite skills.

### What is a data scientist?

Despite no universally agreed definition for data scientist, here is my viewpoint.

***A data scientist is someone who creates value out of data.***

There are several ways to `create value` out of data. And based on the `how` to create value, people have created different job titles.

- Data analysts: analyze existing data to answer business problem
- Data scientist: create algorithm/model to solve business problem
- Data engineer: build algorithm/model in production

While the separation makes sense from a hiring perspective, I don't see it make much sense from a learning perspective. Therefore, in this document I include all of them in the big `data scientist` umbrella.

### What are the responsibilities of data scientists?

1. Build data pipeline
    - In most cases, raw data are not suitable for data analysis. They need to be read, cleaned, and processed data before they can be used in data analysis
    - This is also referred to as `extract, transform, load (ETL)`.
    - Traditionally, this is what data engineers do.
2. Analyze data to extract business value
    - `Business value` may come in various forms. But the most common form is find answer for a particular business problem. For example, explain why the system behaves like this, what can be done to increase the revenue and reduce cost.
    - Traditionally, this is what data analysts do.
3. Develop models for business problems
    - Common situations
        - The models may be machine learning models, signal processing algorithms, are combinations of both.
        - The data scientist may need to design experiments to collect the data, if there is no data available.
        - The data scientist may need to define the performance evaluation metric. It needs to be not only computable but also understandable by the stakeholder. It needs to be computable so that it can be used in the algorithm development. It needs to be understandable so that the stakeholders can understand the outcome of the algorithm.
        - After the models are built, it is the data scientist's job to present the result to stakeholders. This means data scientists are expected to explain the algorithms/models to non-technical people (stakeholders). Data scientists are also expected to make a product suggestion.
    - Traditionally, this is what data scientists do.
4. Create a prototype
    - There are two purposes for creating a prototype of the developed model.
        1. It can be used either internally or by alpha customers to realize the business value **before** the new model is put into production.
        2. It will be the reference point when ths new model is being implemented in production.
    - There are various ways of realizing the prototype. The commons ways are:
        1. Creating a http endpoint
        2. Creating an importable code module
        3. Creating a website where user can interact with the new model
        4. Creating an stand-alone tool (say, a Docker image) for user to run the model locally
    - Traditionally, this is what data scientists do.
5. Implement model in production
    - Traditionally, this is what data engineers or software engineers do.
    - However, since the data scientist is the one who create the algorithm, it is inevitable for the data scientist to be heavily involved in the productionalization process. In some small-mid size companies, it is also not uncommon to ask the data scientist to write production code, or at least part of it.

### Structure of the document

Instead of listing out the resources/courses that I find useful, I take a different approach.

#### The approach

For each `responsibility` (see [data scientist responsibilities](#what-are-the-responsibilities-of-data-scientists?) for the list), I will explain what it is, what does it include, and what are the `skill sets`. Then, I will share the `resources` that I find useful for these skill sets.

In this way, I ensure that I only spend time studying the resources that can help me with the expected responsibility as a data scientist.

## Data scientist responsibilities and learning resources

1. [Build data pipeline](build_data_pipeline.md)

## Unclassified Learning Resources

See [here](unclassified_resources.md) for other useful resources that are not classified (yet) in any of the responsibility.
