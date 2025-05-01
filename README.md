# Open UI Initiative - Overview Repository

NASWA, in partnership with the U.S. Department of Labor, is collaborating with state workforce agencies and other groups to strengthen the unemployment insurance (UI) system with a focus on how modern technology and digital practices can make state systems more accessible, resilient and secure.

The Open UI Initiative will change how we create and purchase technology. It involves forming new collaborations and partnerships to make a wider range of open and modular solutions available

## Table of Contents

1. [About the Open UI Initiative](#about-the-open-ui-initiative)
2. [Open UI GitHub Repositories](#open-ui-github-repositories)
3. [What is the Open UI Framework?](#what-is-the-open-ui-framework)
4. [How to Support the Open UI Initiative](#how-to-support-the-open-ui-initiative)
5. [FAQs](#faqs)
6. [GitHub Tips for Beginners](#github-tips-for-beginners)

<br>

## About the Open UI Initiative

### Background

The way UI systems are typically procured and managed today - as monoliths - makes it difficult for states to adapt systems quickly and leverage emerging technologies. This “all or nothing” paradigm forces states into a choice between maintaining their legacy technology far longer than they would like or embarking on an expensive and lengthy system overhaul. That process often either fails to deliver desired results or delivers short-lived results that require repeating the overhaul process a few years later.

### Initiative Start

NASWA, in partnership with the U.S. Department of Labor, is collaborating with state workforce agencies and other groups to strengthen the unemployment insurance (UI) system with a focus on how modern technology and digital practices can make state systems more accessible, resilient and secure. 

The current environment of UI system modernization varies by state and the overall cost of change is often the major barrier to program and system enhancement. Simultaneously, the marketplace for software solutions is limited and struggles to meet demand and provide cost-effective, flexible solutions. 

A coordinated investment is needed for states to fully benefit from modern technology in the UI system. Thanks to the Open UI Initiative, the system will undergo some of the most significant changes since the introduction of mainframe technologies. 

### Vision

Our vision is a collaborative community promoting a resilient technology landscape and cost-effective innovation in the marketplace to support timely and accurate UI program administration.  

### Theory of Change

Openly sharing ideas and evolving our approach with community at its center is the key to reducing implementation risk, developing a thriving ecosystem for all participants, and maximizing innovation in UI technology. We believe this approach will provide more choices for states in terms of how they invest in technology to meet the goals of the UI program. 

In order to make this change happen, our objectives are: 

#### Objectives

- Define and evolve a standardized modular UI technology framework 

  The Open UI Framework defines what we hope will become the standard topography of UI systems throughout the field. The ability to evolve these modules provides the ability to change their boundaries, adapt their interactions, and optimize their outputs for new standards and technologies.

- Sustain a collaborative process for community contributions 

  Our community provides a trusted structure for individuals and organizations to create, develop, validate, and iterate on the Open UI Framework, and encourage the unemployment insurance ecosystem to evolve. 

- Facilitate adoption of the Open UI Framework 

  Partnering with states and vendors to implement software and products in accordance with the Open UI Framework will help drive positive outcomes and create market-based incentives that drive new innovations. By supporting state implementation and procurement we hope to provide stability in modernization efforts as UI systems adapt to new technologies. 

### About NASWA

The National Association of State Workforce Agencies (NASWA) is the national organization representing all 50 state workforce agencies, D.C. and U.S. territories. These agencies deliver training, employment, career, business and wage and hour services, in addition to administering the unemployment insurance, veteran reemployment and labor market information programs. NASWA provides policy expertise, shares promising state practices and promotes state innovation and leadership in workforce development.

<br>

## Open UI GitHub Repositories

### Overview Repository
The purpose of this repository is to introduce the community to the Open UI Initiative and explain its constituent parts. This repository is openly available to anyone.

Here you’ll find top-level information on the Open UI Initiative and Open UI Framework, answers to frequently asked questions, our [Code of Conduct](CODE_OF_CONDUCT.md) and some beginner tips on how to use GitHub.

### Framework Repository
The purpose of this repository is to host the Open UI Framework, define the modules within it, and how a standardized data schema supports those modules. We will evolve the Framework over time with community support whether that is changing module boundaries, adapting interactions between modules, or optimizing a module’s outputs for new standards and technologies.

This repository is currently available by invitation only. We will soon by expanding access to this repo via an access request form, where additional members of the community will be to request to be able to view, comment, and contribute to content within the repository. Please check back soon for more information.

<br>

## What is the Open UI Framework?

### Introduction 

One of the objectives of the Open Unemployment Insurance (UI) Initiative is to define and evolve a standardized modular UI technology framework. We anticipate the Open UI Framework will become the standard topography of UI systems throughout the field. To learn more about the initiative, please see our About the Initiative page. 

The Open UI Framework defines key groups of functionalities or system boundaries as “modules.” The complete [Open UI Module Set ](https://github.com/NASWA-OpenUI/Overview/blob/72d3a056746146a854475936787e150923499c58/Open%20UI%20Initiative%20Module%20Set.md) is the minimum set of modules needed to fully support the administration of UI. For each of these modules, it specifies data and interface standards for interacting with the rest of a UI system. 

This document discusses the Open UI Framework, how modules are defined within it, and how a standardized data schema supports those modules. With input from the Open UI Community, we will evolve the Open UI Framework over time, whether that is changing module boundaries, adapting interactions between modules, or optimizing a module’s outputs for new standards and technologies.   

### Description 

The Open UI Framework breaks down into three main bodies of work: 
* The [**Open UI Module Set**](https://github.com/NASWA-OpenUI/Overview/blob/72d3a056746146a854475936787e150923499c58/Open%20UI%20Initiative%20Module%20Set.md) enumerates the list of modules and describes each of them at a high level. 
* An **Open UI Module Specification** defines how a given module will interact within a UI system, whether that is from one Open UI Module to another or from an Open UI Module to part of an existing UI system. This information is availble in the [Open UI Framework repository](#framework-repository)
* An **Open UI Data Schema** (forthcoming) to support the standardized interactions specified for each module. 

### More details: Open UI Module Specifications 

#### Module Specifications: What’s in scope? 

The Open UI Framework is intended to capture UI system boundaries as individual module specifications. To do this, an Open UI Module specification will define:  
* Standardized format for data inputs and outputs; the specs will provide one or more examples in e.g., JSON or XML. 
* API specifications for how to trigger functionality within the module, including communication protocol and error handling.  
* Standardized data types, requests, and responses that the module will expose to the rest of the system. Some amount of data validation may also be standardized. 
* Configurable items as needed (whether that is defining certain variables to be set or enabling certain capabilities to be toggled on or off.) 

#### Module Specifications: What’s NOT in scope?  
The Open UI Framework is not meant to define specific implementation details as to how to achieve certain functionality within a module. As such, an Open UI Module specification will NOT:  
* Define the business rules for how to achieve the functionality within the module as these are specific to each state’s UI program 
* Define the interfaces for how a module implementation would connect with external services to achieve the functionality within the module, though we will identify these where possible (e.g., how a module might use ICON to get the outputs it needs) 
* Define the user interfaces for how the module functionality is achieved in an implementation as these will be state dependent and incorporate things like state-specific design patterns, branding, etc.  
* Define security/authentication requirements because these are specific to each state’s UI program and enterprise IT needs. 

### More details: Open UI Data Schema 

For Open UI Modules to be interoperable, we need a standardized data schema, or an outline of how the data should be organized in a database. With a standardized data schema, modules can exchange data without the need for third-party adapters. 

Each Open UI Module Spec does this within its own functional context (for example in defining inputs and outputs), but we will also create documentation in support of a clear data schema across the system. 

Where appropriate the Framework will also standardize field semantics as relates to, for example, how to handle company names that start with the word “The.” Doing this will clarify data handling across scenarios, whether that is within an Open UI module, among Open UI Modules, between an Open UI module and a non-standardized module, or between an Open UI Module and a central data infrastructure. 

<br>

## How to Support the Open UI Initiative
Find more information and updates on the Open UI Initiative at our [website](https://www.naswa.org/open-ui-initiative) or email us at [openui@naswa.org](mailto:openui@naswa.org).

If you have specific feedback to provide about this Overview Repository, please see instructions for how to submit an Issue in our [Contributing Guide](CONTRIBUTING.md).

<br>

## FAQs

### What is the Open UI Initiative?
The Open UI Initiative (Open UI) was created to help address the well documented challenges and risks in state Unemployment Insurance systems through the creation of a technical framework and functional definitions of a state UI system that is modular and therefore more adaptable, scalable, and provides a better user experience to claimants, employers, and state agency staff. The Initiative seeks to create not only technical definitions and documentation but also establish and grow a community of states, vendors, and other stakeholders who can contribute, comment, and iterate modular approaches and implementations.

The Open UI Initiative seeks to create a blueprint, or framework, of an unemployment insurance (UI) system, based on the structure of UI systems across the U.S. We are calling this the Open UI Initiative Framework, and states and vendors can use this framework as a guide to develop their own UI software or to modernize existing systems with the flexibility to fit their policies and workflows.

The framework will follow a modularized approach, or one where the system is sectioned by key functionalities, allowing for the ability to update, change, or replace parts of the system as needed rather than needing to overhaul the entire system all at once. The framework will describe how the modules will communicate with each other, or be interoperable, as well as how they will communicate with other external systems.

### Where can I learn more about the Initiative?
Visit the [Open UI Initiative website](https://www.naswa.org/open-ui-initiative). There you’ll find links to helpful resources and more information about the Open UI Initiative. If you have more questions about the Open UI Initiative, please send an email to [openui@naswa.org](mailto:openui@naswa.org) and include your question and your contact information.

### How is the Open UI Initiative funded?
The Open UI Initiative is currently funded by a grant from the US Department of Labor for a term of three years that ends September 30, 2026. The Initiative operates out of the[ National Association of State Workforce Agencies (NASWA)](https://www.naswa.org/?check_logged_in=1) alongside the[ Unemployment Insurance Information Technology Support Center (UI ITSC)](https://www.naswa.org/services/uiitsc) at NASWA.

### Will the Open UI Initiative include working code?
As of March 2025, the Initiative is not seeking to create, procure, or otherwise develop working code for the modules. As the Initiative evolves this may be a part of the roadmap. To keep up to date on the latest developments in the Open UI Initiative please visit our website.

### Is the Open UI Initiative considered “Open Source”?
The materials created by or contributed to the Initiative are available under an Apache 2.0 license. To learn more about what is allowed under this type of license, please visit our [license documentation](https://github.com/NASWA-OpenUI/Overview?tab=Apache-2.0-1-ov-file).

### What does the Open UI Initiative mean by the word “open”?
The Initiative recognizes that there are number of interpretations to the first word in our name, Open. We’ve come to define it in three ways:

We are open in our way of working with states, vendors, and others who want to contribute to the vision of the Initiative
We aim to open the UI technology marketplace to new ideas, vendors, and approaches
We see value and opportunity in open source software and communities

<br>

## GitHub Tips for Beginners

If you are new to using GitHub, we recommend checking out the following resources to familiarize yourself with its different features and how it works:

- [About GitHub and Git](https://docs.github.com/en/get-started/start-your-journey/about-github-and-git) - Introductory information on GitHub and how it works
- [Beginner’s guide to GitHub repositories](https://github.blog/developer-skills/github/beginners-guide-to-github-repositories-how-to-create-your-first-repo/) - A resource from GitHub that describes what a repository is, how to interact with them, and what the most commonly used features are. Is mostly geared towards creating your own repository but contains helpful introductory information for those who plan to only view or interact with other organizations' repositories
- [Open UI Initiative Contributing Guidelines](url) - Information on how to submit feedback on content in this repository as well as a list of GitHub terms and definitions

