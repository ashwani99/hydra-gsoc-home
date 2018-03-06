title: Ideas Page for Google Summer of Code 2018
date: Tuesday, 6 March 2018

<a class="anchor" id="inspiration"></a>
# Our Inspiration
Building Web APIs seems still more an art than a science. How can we build APIs such that generic clients can easily use them? And how do we build those clients? Current APIs heavily rely on out-of-band information such as human-readable documentation
and API-specific SDKs. However, this only allows for very simple and brittle clients that are hardcoded against specific APIs. Hydra, in contrast, is a set of technologies that allow to design APIs in a different manner, in a way that enables
smarter clients.

You can read more [here](https://www.hydra-cg.com/)
***

<a class="anchor" id="hydrus"></a>
# About Hydrus
Hydrus is a set of Python based tools for easier and efficient creation of Hypermedia driven REST-APIs. Hydrus utilises the power of [Linked Data](https://en.wikipedia.org/wiki/Linked_data) to create a powerful REST APIs to serve data.
Hydrus uses the [Hydra(W3C)](https://www.hydra-cg.com/) standard for creation and documentation of it's APIs.
### Features
- A client that can understand Hydra vocabulary and interacts with a Hydra supporting server to basic [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) operations on data.
- A generic server that can serve required data and metadata(in the form of API documentation) to a client over HTTP.
- A middleware that allows users to use the client to interact with the server using Natural Language which is processed machine consumable language. (under developement)
***

<a class="anchor" id="getting-started"></a>
# How do I get started ?
Getting started is pretty easy. Head over to our [community page](https://www.hydra-cg.com/). There are a lot of demos, presentations, and talks to get you up to speed. Then head over to the [Hydrus repo](https://github.com/HTTP-APIs/hydrus) and clone it. Play with it a little, try to understand how the current implementation works, try to fix some bugs or report any issues you can find [here](https://github.com/HTTP-APIs/hydrus/issues).

Lastly, don't hesitate to reach out in the [Gitter channel](https://gitter.im/HTTP-APIs/Lobby) if you have any question, we are very friendly people and we'll be more than happy to help you out.

As a general entrypoint to understand the repositories, there is the [Hydrus Wiki](https://github.com/HTTP-APIs/hydrus/wiki) and related links. Having a clear insight of [Resource Description Framework](https://goo.gl/TCdYG3) is quite necessary, Mentors will give full support to catch up with it.

### Frequently Asked Questions
**What is Google Summer of Code?**

Google Summer of Code (GSoC) is a global program that matches students up with open source, free software and technology-related organizations to write code and get paid to do it! The organizations provide mentors who act as guides through the entire process, from learning about the community to contributing code. The idea is to get students involved in and familiar with the open source community and help them to put their summer break to good use.

You can read Google [Student Manual](https://developers.google.com/open-source/gsoc/resources/guide#student_manual) for more info.
***

**How to write a proposal?**

Writing a good proposal can be a really challenging task. We have curated a list of helpful resources to help you get started.
- [5 Tips to get your Google Summer of Code proposal accepted](http://people.csail.mit.edu/baghdadi/TXT_blog/5_advices_to_get_your_proposal_accepted.lyx.html)
- [How to write a good GSoC proposal (Quora) ?](https://www.quora.com/How-to-write-a-good-GSoC-proposal)
- [How to write a kick-ass proposal for Google Summer of Code](http://teom.org/blog/kde/how-to-write-a-kick-ass-proposal-for-google-summer-of-code/)
***

**Proposal template**

[Here](https://docs.google.com/document/d/1qPR02o6jY4uFBdCf3S0ous4LG32YCe6ZJuDGojXH2JY/edit)'s a proposal template for you to get started.
***

### Communication Channels
- [Gitter](https://gitter.im/HTTP-APIs/Lobby)
- [W3C Group](https://www.w3.org/community/hydra/)
- Email
  - [Lorenzo Moriondo](mailto:tunedconsulting@gmail.com)
  - [Akshay Dahiya](mailto:xadahiya@gmail.com)
  - [Chris Andrew](mailto:chrisandrew119@gmail.com)
  - [Kristian Koci](mailto:kristian.koci@gmail.com)
  - [Matteo Franchi](mailto:damrgrass@gmail.com)


<a class="anchor" id="ideas"></a>
# Project Ideas
**NOTE:** Every student should apply for any (up to three) of the macro-task (ideas) listed below. Every macro-task involves participating in different activities (listed for every task). Students can build a proposal by choosing a macro-task and then detail which activities and how they want to carry on.

## 1. Ideas related to improving Hydrus
### 1.1 Design a Command line interface for Hydrus

#### Description
Although Hydrus is primarily a Python-based library right now, most Hydra users may not be familiar with Python to set up servers. It would be great if we could have a CLI for Hydrus where users would just need to pass parameters to set up a server and get it up and running. Also, the current process of server setup is long and needs a lot of prerequisite knowledge to be able to set up. This process needs to be abstracted to make it simpler, and more powerful for a user to have more control over the server. Maybe something similar to Python’s SimpleHTTPServer.

#### Skills Required
- Python
- Git
- Flask
- Command Line
- Basic knowledge of Semantic Web and Graph Databases
- Ability to learn new technologies quickly
- Ability to write test suites

#### Difficulty Level - Easy to Intermediate

#### Related Links
- [Hydrus Repo](https://github.com/HTTP-APIs/hydrus)
- [Hydrus Wiki](https://github.com/HTTP-APIs/hydrus/wiki/)
- [The Book of Hydrus](https://gsocchrizandr.wordpress.com/the-book-of-hydrus/)
- [Hydra Draft](https://www.hydra-cg.com/spec/latest/core/)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 1.2 Better API Querying

#### Description
Right now, we only have no mechanism for searching an instance of a class in the Hydra API. Most APIs implement a search feature where the data is queried using a defined syntax. This is more of an issue with Hydra itself as the mechanism for search is not defined in Hydra yet. It would be great if we can have some advance querying functionality like they have in graph databases.

#### Skills Required
- Flask
- Python
- SQLAlchemy
- PostgreSQL
- Command Line
- Basic knowledge of Semantic Web and Graph Databases
- Basic knowledge of graph querying languages
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Hydrus Database Design](https://github.com/HTTP-APIs/hydrus/wiki/Design#dbdesign)
- [Graph querying languages overview](https://developer.ibm.com/dwblog/2017/overview-graph-database-query-languages/)
- [The Book of Hydrus](https://gsocchrizandr.wordpress.com/the-book-of-hydrus/)
- [Hydra Draft](https://www.hydra-cg.com/spec/latest/core/)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 1.3 More User defined Controls for the server

#### Description
There is no way right now to actually change the way the client accesses the server set up by Hydrus. Although there is some support for Authentication/Authorization, the actual implementations are very basic and do not offer much security features. There is also no way to control server access or limit/modify user privilege. There may be APIs that provide different levels of access to different users. There are also bottlenecks in place in REST APIs that limit the number of requests each user can make, such control is not given to users. There needs to be a way to add additional controls to the server, that can be built on top of the original Hydrus app.

#### Skills Required
- Python
- Git
- Flask
- Strong knowledge of Authentication and Authorization in various APIs
- Basic knowledge of Semantic Web
- Ability to learn new technologies quickly
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Hydrus GitHub Repo](https://github.com/HTTP-APIs/hydrus)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 1.4 Support Redis as Graph database

#### Description
Graph based data is everywhere now days, Facebook, Google, Twitter and Pinterest are only a few who've realize the power behind relationship data and are utilizing it to the fullest, as a direct result we see a rise both in interest and variety of graph data solutions.

RedisGraph is a graph database developed from scratch on top of Redis, using the new Redis Modules API to extend Redis with new commands and capabilities. Its main features include: - Simple, fast indexing and querying - Data stored in RAM, using memory-efficient custom data structures - On disk persistence - Tabular result sets - Simple and popular graph query language (Cypher) - Data Filtering, Aggregation and ordering.

Currently Hydrus uses a relational database model to store graph data. It would be interesting to switch to a graph databasee like Redis. We need to implement a multi-layered hexastore to store graph data. This will also help in the implementation of **Idea #1.2 - Better API querying**.

#### Skills Required
- Python
- Git
- Flask
- Basic knowledge of graph databases
- Ability to learn new technologies quickly
- Basic knowledge of Semantic Web
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Redis Graph : A graph database module for Redis](http://redisgraph.io/design/)
- [Paper on representing and querying graphs using an hexastore.](https://redis.io/topics/indexes#representing-and-querying-graphs-using-an-hexastore)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 1.5 Open API to Hydra Parser

#### Description
The OpenAPI Specification (OAS) defines a standard, programming language-agnostic interface description for REST APIs, which allows both humans and computers to discover and understand the capabilities of a service without requiring access to source code, additional documentation, or inspection of network traffic.

OpenAPI and Hydra do much of the same thing and it would be great to have an interface to convert OpenAPI definitions to Hydra API Documentation.

#### Skills Required
- Python
- Flask
- HYDRA
- REST APIs
- Ability to learn new technologies quickly
- Basic knowledge of Semantic Web
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [OpenAPI Spec](https://github.com/OAI/OpenAPI-Specification)
- [Hydra Draft](https://www.hydra-cg.com/spec/latest/core/)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 1.6 Keep Hydrus up-to-date with Hydra Specs

#### Description
Hydra [Draft Specs](https://github.com/HydraCG/Specifications/issues) are evolving and Hydrus needs to follow the most recent updates in the Specs. Code has to be amended to implement new features.

#### Skills Required
- Python
- Git
- Good Knowledge of Semantic Web and REST paradigm
- High problem-solving abilities
- Ability to write test suites

#### Difficulty Level - Hard

#### Related Links
- Hydra [Draft Specs](https://github.com/HydraCG/Specifications/issues)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 1.7 Be Creative

#### Description
Have any ideas of your own? Please feel free to integrate those into your proposal. It'll help your proposal stand out and will increase your chances of being accepted.

#### Skills Required
- To be decided ...

#### Difficulty Level - Interesting

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

## 2. Ideas Related to Demos using Hydrus
### 2.1 Implement Satellite and Subsystems Demo

#### Description
We may finally end up implementing the astronomy/satellites vocabulary as thought in the beginning. We need a way to demonstrate how Hydra can be utilized by Satellites to communicate with each other and get information about each of their subsystems and statuses. The OWL Vocabulary for Subsystems is given [here](https://github.com/chronos-pramantha/RDFvocab). We need to create a Hydra Spec for a demo system that will use these ontologies for a demo.

#### Skills Required
- Python
- Linux
- Server Management
- At least basic knowledge of DevOps
- HTML, CSS, JS
- Knowledge of any Javascript framework is a plus ( React Js or Vue Js)
- Basic Knowledge of Semantic Web
- High problem-solving abilities
- Ability to write test suites

#### Difficulty Level - Intermediate to Hard

#### Related Links
- [Hydrus GitHub Repo](https://github.com/HTTP-APIs/hydrus)
- [A sample drone simulation](https://github.com/HTTP-APIs/hydra-flock-demo)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 2.2 Improve the flock demo

#### Description
We had created a demo using drones and a forestry simulation that communicated in real time to measure temperatures in a forest region. There could be a lot of improvements added to this simulation to add more use cases for Hydra/Hydrus and implementing them in the simulation.

#### Skills Required
- Python
- Linux
- Hydra
- Server Management
- At least basic knowledge of DevOps
- HTML, CSS, JS
- Knowledge of any Javascript framework is a plus ( React Js or Vue Js)
- Basic Knowledge of Semantic Web
- High problem-solving abilities
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Hydrus GitHub Repo](https://github.com/HTTP-APIs/hydrus)
- [A sample drone simulation](https://github.com/HTTP-APIs/hydra-flock-demo)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 2.3 Implement demos for early stage API standards

#### Description
There are many early stage API standards such as WFS-3.0 or Open-EO that are developed for geospatial applications. A cool demo could be developed that uses some geospatial application built using these standards and ports it to Hydrus. This idea is not limited to geo-spatial domains. You could use any API standard that allows two applications to communicate and use Hydra/Hydrus as an interface between them.

#### Skills Required
- Python
- Linux
- Hydra and Hydrus
- OpenEO/WFS/Any other API Standard for some application
- Basic Knowledge of Semantic Web and Hydra
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Hydrus](https://github.com/HTTP-APIs/hydrus)
- [OpenEO](http://r-spatial.org/2016/11/29/openeo.html)
- [WFS](https://github.com/opengeospatial/WFS_FES)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 2.4 Demonstration with Dynamic API paths

#### Description
If we can create an API whose structure(paths to different kinds of data) is constantly changing only the vocab path stays same. Then we can use a Hydra client to discover the required paths for various kinds of data. This can be a great way to demonstrate the capabilities and use cases of HTTP-APIs and Hydra in general. We can have a UI showing the API structure in real-time and allow users to POST/GET/PUT/DELETE any type of data. We can also show how the client and API server interact with each other ( We had a lot of requests going on in the drone demo and it was very difficult to understand how things are working in the background.) For example: Suppose we have a Student class with basic properties like Name, Id, Class etc. Then the user can request for data say "Students with Id = 1*" without knowing anything about the API structure as it's dynamic. We can also demonstrate advanced querying features with this.

#### Skills Required
- Python
- Linux
- Server Management
- At least basic knowledge of DevOps
- HTML, CSS, JS
- Knowledge of any Javascript framework is a plus ( React Js or Vue Js)
- Basic Knowledge of Semantic Web
- High problem-solving abilities
- Ability to write test suites

#### Difficulty Level - Intermediate to Hard

#### Related Links
- [Hydrus GitHub Repo](https://github.com/HTTP-APIs/hydrus)
- [A sample drone simulation](https://github.com/HTTP-APIs/hydra-flock-demo)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 2.5 Rail Management System

#### Description
We can have a cool demo about railway management where trains are routed based on available tracks and are assigned platforms and routes based on live information taken from several trains. This could be a good demo to showcase how Hydra can be used as a generic language since not all railway stations would use the same API to convey information to trains. We could have multiple Hydra based APIs running on railway stations and trains and all of them communicating with each other using Hydra and a common Vocabulary. We still need to find a vocabulary for this, or we could also create one.

#### Skills Required
- Python
- Linux
- Server Management
- At least basic knowledge of DevOps
- HTML, CSS, JS
- Knowledge of any Javascript framework is a plus ( React Js or Vue Js)
- Basic Knowledge of Semantic Web
- High problem-solving abilities
- Ability to write test suites

#### Difficulty Level - Intermediate to Hard

#### Related Links
- [Hydrus GitHub Repo](https://github.com/HTTP-APIs/hydrus)
- [A sample drone simulation](https://github.com/HTTP-APIs/hydra-flock-demo)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 3. Python Client Implementation

#### Description
Implement a generic Hydra client that can reference an API Documentation and allow users to interact with an API using objects, rather than URIs/paths. The HydraConsole is a good reference client to use, and we could extend functionality and implement a Python version of it. More ideas are welcome on this.

#### Skills Required
- Strong Knowledge of Graphs
- At least basic knowledge of RDF
- JSON and JSON-LD
- Python
- Command Line
- Basic knowledge of Semantic Web
- Ability to learn new technologies quickly
- Ability to write test suites

#### Difficulty Level - Intermediate to Hard

#### Related Links
- [Current implementation by @pchampin](https://github.com/pchampin/hydra-py)
- [RDF overview](https://www.w3.org/RDF/)
- [JSON-LD wiki](https://en.wikipedia.org/wiki/JSON-LD)
- [The Book of Hydrus](https://gsocchrizandr.wordpress.com/the-book-of-hydrus/)
- [Hydra Draft](https://www.hydra-cg.com/spec/latest/core/)
- [Hydra Console](https://www.markus-lanthaler.com/hydra/console/)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 4. Support Falcon based server

#### Description
Falcon is a minimalist WSGI library for building speedy web APIs and app backends. When it comes to building HTTP APIs, other frameworks weigh you down with tons of dependencies and unnecessary abstractions. Falcon cuts to the chase with a clean design that embraces HTTP and the REST architectural style. Hydrus is currently implemented using Flask, we're thinking about switching to Falcon.

#### Skills Required
- Python
- Git
- SQLAlchemy
- Falcon Web Framework
- Command Line
- Basic knowledge of Semantic Web
- Ability to learn new technologies quickly
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Falcon Docs](https://falcon.readthedocs.io/en/latest/)
- [Creating resource with Falcon](https://falcon.readthedocs.io/en/latest/user/tutorial.html#creating-resources)
- [Hydus Github Repo](https://github.com/HTTP-APIs/hydrus)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 5. Django-rest-hydra

#### Description
Hydrus is developed in Flask because the applications we had in mind were mostly related to IoT and sensors, so it was supposed to be lightweight and functional. But if we may want to look for more traditional applications and the wider public, we may like to have a Django library ( http://hirokiky.org/tech/create_django_library.html ) that does have the same features as hydrus but works with Django.

As Django has already a well-established REST library (Django-rest) it would be probably useful to extend it and create something like Django-rest-hydra, a library that let Django developers deploy hydra server in Django as now hydrus does with flask (starting from an RDF vocabulary or an OpenAPI definition).

**Note:** [How to create a Django middelware](https://simpleisbetterthancomplex.com/tutorial/2016/07/18/how-to-create-a-custom-django-middleware.html)

#### Skills Required
- Python
- Git
- Django
- Django rest
- Basic knowledge of Semantic Web
- Ability to write test suites

#### Difficulty Level - Intermediate

#### Related Links
- [Creating a Django Library](http://hirokiky.org/tech/create_django_library.html)
- [How to create a Django middleware](https://simpleisbetterthancomplex.com/tutorial/2016/07/18/how-to-create-a-custom-django-middleware.html)
- [Django rest framework](http://www.django-rest-framework.org/)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***

### 6. Create a QGIS plugin

#### Description
Create a QGIS plugin that works with hydrus. QGIS is an opensource geospatial client, geospatial clients are used to load maps in different formats (images, rasters, vectors). QGIS can work as an HTTP client to fetch data from special Web services called OGC Web Standards (WMS, WMTS, WFS). Plugin for QGIS can be developed in Python, a QGIS-HYDRA plugin may be able to query geospatial data stored in hydrus using the HYDRA vocabulary. The same functionality could be accomplished with a MapBox or LeafLet client app that uses a python-hydra client as middleware and hydrus as a backend.

#### Skills Required
- Python
- Git
- Basic Knowledge of Semantic Web
- Good Knowledge of GIS software ecosystem
- High problem-solving abilities
- Ability to write test suites

#### Difficulty Level - Hard

#### Related Links
- [QGIS Homepage](https://qgis.org/en/site/)
- [QGIS Github Repo](https://github.com/qgis)
- [OpenGeoSpatial Consortium Web standards](https://en.wikipedia.org/wiki/Open_Geospatial_Consortium#Standards)

#### Potential Mentors
[Lorenzo Moriondo](https://www.linkedin.com/in/lorenzomoriondo/), [Akshay Dahiya](https://www.linkedin.com/in/xadahiya/), [Chris Andrew](https://www.linkedin.com/in/chrizandr/), [Kristian Koci](https://www.linkedin.com/in/kristian-koci-1304a025/), [Matteo Franchi](https://www.linkedin.com/in/matteofranchi)
***
