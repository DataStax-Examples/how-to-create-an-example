# DataStax Examples Style Guide
This guide is meant to provide a reference for how to create repositories meant for submission to the DataStax Examples platform.

## Types of Examples
The first decision that needs to made when working on a project for submission is what type of project are you trying to build.  Projects within the DataStax Examples platform fall into one of four types:

* Code Snippet - A short simple code sample to demonstrate a simple concept 
    
    **Example** Connecting to a Apollo Cluster with Java

* Sample - A smaller code project that demonstrates a more complex concept potentially involving multiple components
    
    **Example** Using the Kafka Connector with Apollo

* Project - A complete code project that demonstrates a full end to end work flow
    
    **Example** Building an E-Commerce site on Apollo


* Tool - A fully developed and tested tool for use within the DataStax product environment 
  
  **Example** Cassandra Schema Diff Tool

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

## Writing a Code Snippet Document
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

## Writing a Sample Document
* Title
* Overview
  * Don't use any heading. Just start with the first sentence.
  * Up to a few paragraphs describing how the sample works
* Objectives
  * A short bulleted list of what the reader is expected to learn through this example
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

## Writing a Project or Tool Document
* Title
* Overview
  * Don't use any heading. Just start with the first sentence.
  * Up to a few paragraphs describing how the sample works
* Objectives
  * A short bulleted list of what the reader is expected to learn through this example
* Setup and Running
  * List any Pre-requisites
    
    **Example** Java 8 must be installed
  * Provides the details.
  * Contains appropriate headings and subheadings as needed to make the content easy to read
  * Use Screenshots when they clarify a point, they are not needed at ever step.  
  * Describe what success looks like after every major step in the process
      **Example** You should now see that "Connected" has been printed to the terminal window of your application
  * End this section with any clean up required
    **Example** Don't forget to terminate the Apollo instance to prevent any additional charges
* How this Sample Works
  * Provides the details on how the sample works including any architectural diagrams and explanation needed
  * Contains appropriate headings and subheadings as needed to make the content easy to read
  * Use Screenshots when they clarify a point, they are not needed at ever step.  
  * Describe what success looks like after every major step in the process
      
      **Example** You should now see that "Connected" has been printed to the terminal window of your application
  * End this section with any clean up required
    
    **Example** Don't forget to terminate the Apollo instance to prevent any additional charges

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
