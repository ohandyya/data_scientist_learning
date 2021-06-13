# Learning resources for data scientist

## About this document

### What is it?

- A curated and **opinionated** list of the learning resources for data scientist.
- Focus more on technical skill, and less on soft (people) or management skill.

### What is data scientist?

Despite there is no universally agreed upon definition for data scientist, here is my definition.

***A data scientist is someone who creates value out of data.***

Below are some common tasks for creating value out of data. The tasks below cover the work for data analysts, data engineer, and data scientist. I put all of them under the big data scientist umbrella.

1. Build data analytics pipeline to read, clean, and process data from various sources for future use.
    - This is also referred to as `extract, transform, load (ETL)`.
    - Traditionally, this is what data engineers do.
2. Analyze existing data to answer particular business questions.
    - Traditionally, this is what data analysts do.
3. Develop algorithms for a particular business problem, and present the result to stakeholders.
    - Common situations
        - The algorithms usually refer to either machine learning algorithms or signal processing algorithms.
        - The data scientist may need to design experiments to collect the data, if there is no data available.
        - The data scientist may need to define the performance evaluation metric. It needs to be not only computable but also understandable by the stakeholder.
        - It is usually the data scientist's job to explain the idea and the performance of the algorithm to the stakeholder. Data scientists also are expected to make a product suggestion.
    - Traditionally, this is what data scientists do.
4. Create a prototype for the newly developed algorithms.
    - There are two purposes for creating a prototype.
        1. It can be used either internally or by alpha customers to realize the business value **before** the new algorithm is put into production.
        2. It will be the reference point when ths new algorithm is being implemented in production.
    - There are various ways of realizing the prototype. The commons ways are:
        1. Creating a http endpoint
        2. Creating an importable code module
        3. Creating a website where user can interact with the new algorithm
        4. Creating an stand-alone tool (say, Docker image) for user to run the algorithm locally
    - Traditionally, this is what data scientists do.
5. Implement the algorithm into production.
    - Traditionally, this is what either data engineers or software engineers do.

### Who is this for?
TBD