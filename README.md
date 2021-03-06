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

### Structure of the document

Instead of simply listing out the resources/courses that I find useful, I take a different approach.

#### The approach

First, I will list the key [`responsibility`](#data-scientist-responsibilities) for data scientists. For each responsibility, I will include a brief description and the skill sets that needed for this responsibility.

For some `skill set`, I will include the resources that I find useful in improving this skill set.

## Data scientist responsibilities

1. Build data pipeline
    - Description
        - In most cases, raw data are not suitable for data analysis. They need to be read, cleaned, and processed data before they can be used in data analysis
        - This is also referred to as `extract, transform, load (ETL)`.
        - Traditionally, this is what data engineers do.
    - Skill sets
        - Science: basic statistics
        - Science: basic machine learning
        - [Programming best practices](#Programming-best-practices)
        - [Programming: python](#Programming-python)
        - [Programming: Golang](#Programming-Golang)
        - Programming: python machine learning packages (numpy, scipy, pandas, scikit-learn) 
        - [Technology: Docker](#Technology-Docker)
        - [Technology: Spark](#Technology-Spark)
        - [Technology: AWS](#Technology-AWS)
        - [Technology: Azure](#Technology-Azure)
        - [Technology: GCP](#Technology-GCP)
2. Analyze data to extract business value
    - Description
        - `Business value` may come in various forms. But the most common form is find answer for a particular business problem. For example, explain why the system behaves like this, what can be done to increase the revenue and reduce cost.
        - Traditionally, this is what data analysts do.
    - Skill sets
        - Good presentation skill to explain technical results to business & product people
        - Good understanding of the business (what is valuable, what is the operation cost, etc)
        - Science: basic statistics
        - Science: basic machine learning
        - [Programming: python](#Programming-python)
        - Technology: data visualization
3. Develop models for business problems
    - Description
        - Common situations
            - The models may be machine learning models, signal processing algorithms, are combinations of both.
            - The data scientist may need to design experiments to collect the data, if there is no data available.
            - The data scientist may need to define the performance evaluation metric. It needs to be not only computable but also understandable by the stakeholder. It needs to be computable so that it can be used in the algorithm development. It needs to be understandable so that the stakeholders can understand the outcome of the algorithm.
            - After the models are built, it is the data scientist's job to present the result to stakeholders. This means data scientists are expected to explain the algorithms/models to non-technical people (stakeholders). Data scientists are also expected to make a product suggestion.
        - Traditionally, this is what data scientists do.
    - Skill sets
        - Good presentation skill to explain technical results to business & product people
        - Good understanding of the business (what is valuable, what is the operation cost, etc)
        - Science: basic statistics
        - Science: basic machine learning
        - [Science: advanced machine learning](#Science-advanced-machine-learning)
        - [Programming: python](#Programming-python)
        - Programming: python machine learning packages (numpy, scipy, pandas, scikit-learn)
        - [Technology: Tensorflow](#Technology-Tensorflow)
        - Technology: PyTorch
        - [Technology: Docker](#Technology-Docker)
        - [Technology: AWS](#Technology-AWS)
        - [Technology: Azure](#Technology-Azure)
        - [Technology: GCP](#Technology-GCP)
4. Create a prototype
    - Description
        - There are two purposes for creating a prototype of the developed model.
            1. It can be used either internally or by alpha customers to realize the business value **before** the new model is put into production.
            2. It will be the reference point when ths new model is being implemented in production.
        - There are various ways of realizing the prototype. The commons ways are:
            1. Creating a http endpoint
            2. Creating an importable code module
            3. Creating a website where user can interact with the new model
            4. Creating an stand-alone tool (say, a Docker image) for user to run the model locally
        - Traditionally, this is what data scientists do.
    - Skill sets
        - [Programming best practices](#Programming-best-practices)
        - [Programming: python](#Programming-python)
        - Programming: python machine learning packages (numpy, scipy, pandas, scikit-learn)
        - [Technology: Tensorflow](#Technology-Tensorflow)
        - Technology: PyTorch
        - [Technology: Docker](#Technology-Docker)
        - Technology: Protobuf
        - [Technology: AWS](#Technology-AWS)
        - [Technology: Azure](#Technology-Azure)
        - [Technology: GCP](#Technology-GCP)
        - [Technology: Rest API](#Technology-Rest-API)
        - [Technology: gRPC](#Technology-gRPC)
5. Implement model in production
    - Description
        - Traditionally, this is what data engineers or software engineers do.
        - However, since the data scientist is the one who create the algorithm, it is inevitable for the data scientist to be heavily involved in the productionalization process. In some small-mid size companies, it is also not uncommon to ask the data scientist to write production code, or at least part of it.
    - Skill sets
        - [Programming best practices](#Programming-best-practices)
        - [Programming: System design](#Programming-System-design)
        - [Programming: python](#Programming-python)
        - [Technology: Docker](#Technology-Docker)
        - Technology: Protobuf
        - [Technology: Terraform](#Technology-Terraform)
        - [Technology: AWS](#Technology-AWS)
        - [Technology: Azure](#Technology-Azure)
        - [Technology: GCP](#Technology-GCP)
        - [Technology: Rest API](#Technology-Rest-API)
        - [Technology: gRPC](#Technology-gRPC)
        - Technology: Databases
        - Technology: Kubernetes
        - Technology: Jenkins

## Skill sets and resources

### Programming best practices

- [Clean Architecture: A Craftsman's Guide to Software Structure and Design](https://www.amazon.com/Clean-Architecture-Craftsmans-Software-Structure/dp/0134494164/ref=sr_1_1?crid=34434EFXB4FPV&dchild=1&keywords=clean+architecture&qid=1624128513&sprefix=clean+architcture%2Caps%2C165&sr=8-1)

- [The Pragmatic Programmer](https://www.amazon.com/Pragmatic-Programmer-Anniversary-Journey-Mastery/dp/B0833FBNHV/ref=sr_1_1?crid=6NFNMM3E5U9T&dchild=1&keywords=the+pragmatic+programmer&qid=1624128656&sprefix=The+pragmatic+%2Caps%2C164&sr=8-1)

- [SOLID Principles of Object-Oriented Design and Architecture](https://www.udemy.com/course/solid-principles-object-oriented-design-architecture/)

- [The Complete Data Structures and Algorithms Course in Python](https://www.udemy.com/course/data-structures-and-algorithms-bootcamp-in-python/)

- [The twelve-factor app](https://12factor.net/)

- [How To Become An Outstanding Solution Architect](https://www.udemy.com/course/how-to-become-an-outstanding-solution-architect/)

### Programming: System design

- [AWS Lambda & Serverless Architecture](https://www.udemy.com/course/aws-lambda-serverless-architecture/)

### Programming: python

- [Python Cookbook](https://www.amazon.com/Python-Cookbook-Third-David-Beazley/dp/1449340377/ref=sr_1_3?crid=JQTU3RVB4T97&dchild=1&keywords=python+cookbook&qid=1624128807&sprefix=python+cook%2Caudible%2C159&sr=8-3)

- [Fluent Python: Clear, Concise, and Effective Programming](https://www.amazon.com/Fluent-Python-Concise-Effective-Programming/dp/1491946008/ref=sr_1_1?crid=1N7X8LWWLACDA&dchild=1&keywords=fluent+python&qid=1624128911&s=books&sprefix=fluen%2Cstripbooks%2C165&sr=1-1)

### Technology: Docker

- [Docker Mastery: with Kubernetes +Swarm from a Docker Captain](https://www.udemy.com/course/docker-mastery/)

### Technology: Spark

- [Spark and Python for Big Data with PySpark](https://www.udemy.com/course/spark-and-python-for-big-data-with-pyspark/)

### Technology: Tensorflow

- [Complete Tensorflow 2 and Keras Deep Learning Bootcamp](https://www.udemy.com/course/complete-tensorflow-2-and-keras-deep-learning-bootcamp/)

### Technology: AWS

- [Ultimate AWS Certified Developer Associate 2021](https://www.udemy.com/course/aws-certified-developer-associate-dva-c01/)

### Technology: GCP

- [Ultimate Google Certified Processional Cloud Architect 2020](https://www.udemy.com/course/google-cloud-architect-certifications/)

### Technology: Azure

- [AZ-204 Developing for Microsoft Azure](https://www.udemy.com/course/70532-azure/)

### Technology: Terraform

- [Learn DevOps: Infrastructure Automation With Terraform](https://www.udemy.com/course/learn-devops-infrastructure-automation-with-terraform/)

### Technology: Rest API

- [REST APIs with Flask and Python](https://www.udemy.com/course/rest-api-flask-and-python/)

### Technology: gRPC

- [gRPC (Golang) Master Class](https://www.udemy.com/course/grpc-golang/)

### Programming: Golang

- [Learn How To Code: Google's Go (golang) Programming Language](https://www.udemy.com/course/learn-how-to-code/)

- [The Go Programming Language](https://www.amazon.com/Programming-Language-Addison-Wesley-Professional-Computing/dp/0134190440/ref=sr_1_3?dchild=1&keywords=the+go+programming+language&qid=1624133815&sr=8-3)

- [Go in practice](https://www.amazon.com/Go-Practice-Techniques-Matt-Butcher/dp/1633430073/ref=sr_1_1_sspa?dchild=1&keywords=go+in+practice&qid=1624133855&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUEzSjA4OVVIMFNXM0RCJmVuY3J5cHRlZElkPUEwOTYxMjc2VkNOUUg5TVhEM0tBJmVuY3J5cHRlZEFkSWQ9QTA1OTA5MzQ2TzNVVEJJTFRNTzQmd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)

- [Golan Tutorial](https://www.bogotobogo.com/GoLang/GoLang_HelloWorld.php)

## Science: advanced machine learning

- [Advanced Machine Learning Specialization](https://www.coursera.org/specializations/aml?ranMID=40328&ranEAID=vedj0cWlu2Y&ranSiteID=vedj0cWlu2Y-g_TM.SFgPEE4Je3U4Uodig&siteID=vedj0cWlu2Y-g_TM.SFgPEE4Je3U4Uodig&utm_content=10&utm_medium=partners&utm_source=linkshare&utm_campaign=vedj0cWlu2Y#courses)

- [Generative Adversarial Networks (GANs) Specialization](https://www.coursera.org/specializations/generative-adversarial-networks-gans?action=enroll&utm_campaign=EmailPartnerPromoGANs&utm_medium=institutions&utm_source=deeplearningai)

- [Probabilistic Graphical Models Specialization](https://www.coursera.org/specializations/probabilistic-graphical-models)

## Programming: practice coding

- [Exercism](https://exercism.io/)

- [Leetcode](https://leetcode.com/)

## Unclassified Learning Resources

Useful resources that are not classified (yet) in any of the responsibility.

- [Awesome MLOps](https://github.com/visenger/awesome-mlops)

- [MLOps Specialization](https://www.coursera.org/specializations/machine-learning-engineering-for-production-mlops)

- [The data engineering cookbook](https://github.com/andkret/Cookbook)

- [Awesome CTO](https://github.com/kuchin/awesome-cto)

- [Data Engineering Study Guide](https://docs.google.com/spreadsheets/d/1GOO4s1NcxCR8a44F0XnsErz5rYDxNbHAHznu4pJMRkw/edit?usp=sharing)
