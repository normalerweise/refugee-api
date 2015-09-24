# Refugee API (Working title)

\#refugeehackathon project proposal

## Motivation
Following the raising #refugeehackathon movement and some local activities indicates one at the same time great and sad fact:

Several people have ideas how to support with the help of IT.
Several people start projects that overlap at least on the data level.

Ideas like “Platform to macht supply and demand for help”, “Directory of volunteers”, “List of upcoming events”, “Directory of language courses offerings” came up more than once.

Considered pragmatic and realistic it is likely impossible to avoid fragmentation, similar/overlapping projects and maybe required to figure out what works.  

However…

## Idea

…consolidated, aggregated and publicly accessible data add value in several ways.

Therefore I propose to develop and operate a “Refugee API”.

New Projects: Using an existing API reduces effort and speeds up the development. The API could e.g. serve as a Backend as a Service for several small, focused but useful mobile Apps.

Existing Projects: Leverage the data of existing projects by
combining data sets. Existing projects also could use the API to add additional data to their project.

More Projects: Having a stronger database could enable new projects with completely different value.

Let us develop a modular system that provides a consistent, intuitive, stable and reliable API to access data related to refugee aid. The system should contain frequently changing data like available supplies as well as static data like a knowledge base for frequently required information.  

Around the core API further services a like full text search system, a matching or a recommender system could evolve that enrich the capabilities. The following diagram sketches the envisioned system:

![](https://raw.githubusercontent.com/normalerweise/refugee-api/master/doc/system_design.png)  

———————————————————————————
Work in progress………

## System Design



## Thoughts about technology

How to store data?
   - “Classic” REST API, i.e. using something like PostgreSQL + Loopback
   - Semantic WEB technology: The [DBpedia](http://wiki.dbpedia.org/) approach - building an ontology, store the data in a triple store and provide a SPARQL endpoint.
   - Combination of both approaches?

Are there existing systems that could be extended/adjusted to fulfill the features described above?

## Related / Complementary Projects

- [HelperAuth](http://refugeehackathon.de/projekte/helperauth/)

## Work Packages

WP1: Design and develop V1 of the core api
     - Define the most important entities
     - Provide basic user management, authentication and authorization  

WP2: Organizational
     - Decide for and register a domain
     - Decide for an appropriate Software License
     - Usage agreement?

WP3: Find computational resources
    - Where could the API be deployed at which costs?

WP4: Define and design a deployment process
   - Automate as much as possible

TBD: ———

WP X: Full text search API
WP X: Help “Supply and Demand” matching service
WP X: Crawler/connector to link other databases
