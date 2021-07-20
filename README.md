# [openAns](https://openansorg.github.io) - SRS
Open source project for creation and computation of formulas
<br/><br/>
![openAns Logo](./CompleteLogo.png)
<br/> 

## Introduction
This document lays out a project plan for the development of “openAns” open source project by Devaraja G.
<br/><br/>
The intended readers of this document are current and future developers working on “openAns” and the sponsors of the project. The plan will include, but is not restricted to, a summary of the system functionality, the scope of the project from the perspective of the “openAns” team , scheduling and delivery estimates, project risks and how those risks will be mitigated, the process by which I will develop the project, and metrics and measurements that will be recorded throughout the project.
<br/> 

## Overview
Most of the questions we face in scientific world are formula based. But there is no one unified place currently, where we can refer any formula we want, compute using the formula and even contribute our own ones. The model I aim to make is like StackOverflow but for formulae with the included functionality of having your own set of formulas which you can choose to keep private and a way to use that formula by entering the values for variables and calculating the result. The formulae will be written in a programming language, saved in our servers and whenever a user requests it, the file will be sent so that they can do computations on their browser. This will also include a in browser runtime for python to run the code.
<br/>
- ### Customers
Anyone who has questions or answers that are formula based and willing to contribute to the effort of gathering all of the worlds formulae in a single place.
<br/>
- ### Functionality
  - Passwordless auth with JWT
  - See formulae in feed according to search
  - Upvote or downvote public formulae
  - Have personal private formulae
  - Verified users badge
  - Verified answers badge
  - Generate graphs
  - Comment and disscuss
  - Edit formulae (only creator access)
  - Ask questions and request formulae
  - Have communities
<br/>

- ### Platform
Initially planned for web, but since it will use a common backend API, in future a mobile app for Android and iOS will be made too.
<br/>

- ### Development Responsibilty
I, Devaraja G, take responsiblity for the software all of it's workings.
<br/> 

## Goals and Scope
- Users must be able to register and login with passwordless auth
- They can refer formulae (Public access)
- They can do computations (User access)
- They can ask questions in communities and get answers
- They can upvote or downvote answers based on it's workings
- They can comment on answers
- They can have their own private set of formulae too, which can be made easier to use with the GUI
- They can join communities
- They can follow other users
<br/> 

## Deliverables
I will be taking care of the project from its start till a team can be formed and afforded.
<br/> 

## Risk Management
The following will be the risks of my project:
- Risk Identification
People already have access to formulae accross the internet scattered accross a wide range of websites

- Risk mitigation
  - Even though people have access to formulae already, the non existance of a universal platform to refer and compute with those formulae provides us an edge and market.
This difference is a so large that it can form a new market, I believe.
<br/> 

## Scheduling
Yet to be released.
<br/> 

## Business Logic
There are two main approaches available:
- Create a GUI system for creating formulae in which others can plug in values and find answer
- Create a system where a formula is essentially and program and whenever someone wants to use a particular formula they can run the program and give the values in input

After giving it some thought, I have decided to use a program based solution, because it's accurate, dynamic and will also help the goal of creating a library in certain programming languages that will contain all the formulae defined as a function in that language.

Also the initial release is set to be used only Python as the programming language, because the code will be run on client-side inorder to minimize the load on servers. We are set to use [Pyodide](https://pyodide.org/en/stable/) as the  python runtime.

The search results will be displayed in the main page with a try it button, which takes the user to another page prefilled the code of the choice selected previously. It uses Pyodide to run the code and display the output. 

The code is presented inside a editor from "Codemirror". The code editor and  terminal are resizeable panes. 

For using the formula, the code will be presented using highlight.js, since editting the code is not allowed. Also including codemirror for the usage page increases the size of the page unnecessarily.

Function creation pages will include codemirror.
<br/>

## Technical Process
Yet to be released.
<br/> 

## Pricing
This is a free for all open source project.
<br/> 

## Security and Authentication
This project will be using Passwordless authentication with JWT web tokens in order to minimize the chances of a password breach (suprisingly over 80% of breaches today happen with password hacking). JWT is currently considered to be the gold standard for web auth and it paired with passwordless login where a user will get a login link to theur email, improves the robustness of the system.

## User stories

<br/> 

## Wireframe

<br/> 

## UI/UX

<br/> 

## Backend Design

<br/> 

## Frontend (Web)

<br/> 

## Frontend (Mobile)
Will be done after the release of web-application
<br/> 

## Marketing
In page ads, with a minimal effect on user experience by having only 10% of the page's area alloted for it. Reason behind this is for running the servers and servers and provide the developers some reward for their contribution.
<br/> 

## Summary

<br/> 
<p align="center"><img src="https://forthebadge.com/images/badges/built-with-love.svg"/><br/><a href="htpps://github.com/codizt"><b>©Codizt</b></a></p>
