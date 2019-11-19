# DataStax Examples Style Guide
This guide is meant to provide a reference for how to create repositories meant for submission to the DataStax Examples platform.

## Types of Examples
The first decision that needs to made when working on a project for submission is what type of project are you trying to build.  Projects within the DataStax Examples platform fall into one of four types:

* Snippets - Simple small code samples that demonstrate a best practice for a single task

    **Examples**
    
    * Switching between connecting to Apollo or DSE in the same application
    * DS Graph Studio notebooks

* Tasks - These demonstrate common activities that developers do all the time and would like to be able to see working examples 
    
    **Examples** 
    * Paging results in a web application
    * Working with Reactive Programming in Java


* Applications - Full fledged end to end applications used to demonstrate best practices for a specific use case

    **Examples**
    * Solution Factory for Customer 360
    * Using DataStax for Graph Embeddings

* Tools - Simple open source tools or add ons to existing tooling

    **Examples**
    * Add a new stack for DataStax Desktop
    * Deployment Scripts for Ansible/Puppet/Chef


## File Organization in GitHib
All submissions are expected to be on the `master` branch of the repository.  Any other branches may be made for bug fixes, features, or improvements but must be merged into the `master` branch for submission.

All submission can only use publicly available tooling.  These can require that a license be purchased but this needs to be noted as a pre-requisite.  Non-public are not allowed

Because there is such a wide variety of potential languages and projects that will take part in the DataStax Examples platform so their is no explicit folder structure required.  The folder structure of the repository will be checked upon submission to ensure it is logical for the type and language of project being submitted.  As such we suggest that the guidelines found [here](https://github.com/kriasoft/Folder-Structure-Conventions) be used as a starting point for any repository.

While no explicit folder structure is specified their are a few files which are required to be in the root of the repository:

* README.md - This is the central narrative describing the details of how the example works.  For a detailed overview of what should be included in the README checkout out the [README Guidelines](##-README-Guidelines)

* LICENSE.md - The license for the repository.  This must be an Open Source License, preferably Apache 2.0 or MIT
  
* CONTRIBUTING.md - This provides potential contributors to this project a guide on the process and guidelines for contributing.

* CODE_OF_CONDUCT.md - Defines the standard for how to engage the community and signals the inclusive and welcoming nature of the project which respects and acknowledges all contributions to the project

For an example base repository with all the required files already added you can use the template repo available [here](https://github.com/bechbd/datastax-examples-template).

## README Guidelines

## Format of a README
A Code Snippet README doc has these major sections:

* Title
* Overview
  * Don't use any heading. Just start with the first sentence.
  * Up to a few paragraphs describing how the sample works
* Objectives
  * A short bulleted list of what the reader is expected to learn through this example
* Body
  * Provides the details, use numbered steps as they are helpful.
  * Contains appropriate headings and subheadings as needed to make the content easy to read
* Attribution
  * A quick one liner giving credit to the creator/maintainer of the repo something like "Created and Maintained by [bechbd](https://github.com/bechbd)"

## Writing a Sample Document
* Title
* Overview
  * Don't use any heading. Just start with the first sentence.
  * Up to a few paragraphs describing how the sample works
* Objectives
  * A short bulleted list of what the reader is expected to learn through this example
* Files
  * A listing of the important files in the project that a customer would want to look at.  This can exclude well known files used for a project structure such as `pom.xml` for Java projects or `package.json` for NodeJS projects.
* Setup and Running
  * List out any steps required to prepare for this example and how to achieve them if they do not
    
    **Example** Have an Apollo Account, if you don't have one go [here]().
  * List any Pre-requisites
    
    **Example** Java 8 must be installed
  * Provides the details.
  * Contains appropriate headings and subheadings as needed to make the content easy to read
  * Use Screenshots when they clarify a point, they are not needed at ever step.  
  * Describe what success looks like after every major step in the process
      
      **Example** You should now see that "Connected" has been printed to the terminal window of your application
  * End this section with any clean up required
    
    **Example** Don't forget to terminate the Apollo instance to prevent any additional charges
* Attribution
  * A quick one liner giving credit to the creator/maintainer of the repo something like "Created and Maintained by [bechbd](https://github.com/bechbd)"
## Writing a Project or Tool Document
* Title
* Overview
  A short few sentences describing what is the purpose of the example and what the user will learn

e.g.
This application shows how to use configure your NodeJs application to connect to DDAC/Cassandra/DSE or an Apollo database at runtime.

Contributors: A listing of contributors to this repository linked to their github profile

## Objectives
A list of the top objectives that are being demonstrated by this sample

e.g.
* To demonstrate how to specify at runtime between a standard (DSE/DDAC/C*) client configuration and an Apollo configuration for the same application.
  
## Project Layout
A list of key files within this repo and a short 1-2 sentence description of why they are important to the project

e.g.
* app.js - The main application file which contains all the logic to switch between the configurations

## How this Works
A description of how this sample works and how it demonstrates the objectives outlined above

## Setup and Running

### Prerequisites
The prerequisites required for this application to run

e.g.
* NodeJs version 8
* A DSE 6.7 Cluster
* Schema added to the cluster

### Running
The steps and configuration needed to run and build this application

e.g.
To run this application use the following command:

`node app.js`

This will produce the following output:

`Connected to cluster with 3 host(s) ["XX.XX.XX.136:9042","XX.XX.XX.137:9042","XX.XX.XX.138:9042"]`

## General Style Guidelines
When writing content for this site it is fair to assume that readers are technical.  This means:

* Write for a technical audience.  There is no need to explain concepts or terminology that are common within the software development community.
* If a new concept or term is used as part of the example then provide a brief explanation or link to the explanation
* These are not meant to be sales brochures so do not write these examples as a product pitch.  Avoid superlatives such as "the best", "amazing", "fantastic", and so on as they reduce the validity with which your writing is received.  
* Use active voice when possible in the content
    
    **Active (Preferred)** "The Client writes a record to the database"
    
    **Passive (Discouraged)** "A record was written to the database by the client"
* Speak to the reader in an informal way and use second person pronouns (e.g. you) not first person (e.g. I or we).
* Speak in the present tense 

### Markdown Usage
All content will be written in Markdown and stored on GitHub.  For a quick reference guide on proper Markdown syntax for Github please visit: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
