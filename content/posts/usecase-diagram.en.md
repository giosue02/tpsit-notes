--- 
title: "Use Case Diagram" 
description: "Describes the functions of a system" # update text ! 
date: 2021-02-23T17:15:00+01:00 # update date ! 

draft: true # toggle to false when final version is approved ! 

languageName: "English" 
author: ["Giosuè", "Alessio", "Daniel", "Giacomo"] 

tags: ["Software Requirements"]   
categories: ["Software Requirements"]   
---  

<!-- Write content Down Here :) --> 

# What is the Use Case Diagram

The Use Case Diagram is a representation of a user's interaction with the software system, showing the relationship between the user and the different use cases in which the user is involved.

A use case diagram can identify the different types of users of a system and is often accompanied by other types of diagrams.

Use cases specify the intended behaviour, but not the exact method of achieving it.

The key concept of the diagram is to design a system from the point of view of the end user.

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Initial_scheme.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Initial_scheme.svg)

# Origins of the Use Case Diagram

- In 1986, Ivar Jacobson first formulated textual and visual modelling techniques for specifying use cases.
- In 1992, Jacobson published "Object-Oriented Software Engineering - A Use Case Driven Approach", which helped to popularise the technique for capturing functional requirements, especially in software development.

# Aims and objectives of the Use Case Diagram

- To specify the context of the system under development
- Understand the system requirements
- Validate a system architecture
- Promote implementation and generate test cases

# Elements in a use case diagram

- Actor: is someone who interacts with the use case and is named by a noun.

    ![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Actor.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Actor.svg)

- Use case: is a function of the system, it is represented by verb + noun.

    ![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Use_Case.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Use_Case.svg)

- Association link: links an actor to a use case.

    ![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Association.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Association.svg)

- System boundary: is potentially the whole system, it can be a system boundary for specific use cases.

# Generalization relationship

It is a parent-child relationship between use cases. The child use case is an enhancement of the parent use case.

It is represented by an arrow with a triangular tip. The child use case is connected to the base of the arrow and the parent use case is connected to the tip of the arrow.

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Generalization_1.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Generalization_1.svg)

The child use cases (Search by call number/author) inherit the behaviour and meaning of the parent use case (Search).

The child use case can add to or override the behaviour of the father.

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Generalization_2.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Generalization_2.svg)

# "include" relationship

When a use case is described as a user of another use case, their relationship is called "include".

A use case relationship is represented by a dotted line and an arrow. The tip indicates the child process, while the base is the parent.

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Include_3.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Include_3.svg)

The "include" relationship adds functionality not specified in the use case. The included case is part of the behaviour of the one that includes it.

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Include_1.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Include_1.svg)

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Include_2.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Include_2.svg)

# "extend" relationship

You write "extend" to identify an extension relationship between two use cases.

It is represented by a dotted arrow. At the tip of the arrow is the base case and at the base is the child use case.

In this case the use case "Invalid password" can include the behaviour specified in the base use case "Login Account".

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Extend_3.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Extend_3.svg)

The relationship "extend" shows optional functionality, it is used to include the behaviour of an optional use case (Search) in the base use case (Request a book).

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Extend_1.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Extend_1.svg)

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Extend_2.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Extend_2.svg)

# Difference between "include" and "extend"

Include: the action is always executed during the execution of the use case at the base of the arrow.

Extend: the action can be executed under certain circumstances of the use case at the tip of the arrow.

# How to build a Use Case model

Information can be obtained from interviews with users. Objectives are identified, i.e. what the system should do according to the users, and interactions, i.e. what the different users would or could do.

The main steps in building a Use Case model are:

1. Identify the actors
2. Identify use cases
3. Define the associations between actors and use cases
4. Describe use cases
5. Structuring use cases
6. Identifying actors

## Identification of the actors

Useful questions:

- Who uses the system?
- Who installs the system?
- Who starts the system?
- Who maintains the system?
- Who stops the system?
- What other systems use this system?
- Who receives the information from this system?
- Who provides information to the system?
- Does something happen automatically at this moment?

A typical mistake that is made when identifying actors is to use different names to identify the same role and therefore the same actor (e.g. counter worker, teller).

This problem is particularly frequent when the same case model is carried out by different teams.

To solve this problem, it is sufficient to draw up a shared list of actors that is updated each time a new actor is added.

## Identification of use cases

Useful questions:

- What functions does the actor demand from the system?
- Does the system store information? Which actors will create, read, update or delete this information?
- Does the system have to notify an actor of changes in the internal state?
- Are there external events of which the system needs to be aware? Which actor informs the system of those events?

For each actor:

- Identify the tasks or functions that it must be able to perform
- Identify the tasks that the system requires it to perform.

Then it is necessary to group the tasks and functions into use cases that:

- Must correspond to a specific objective for the actor or the system.
- Must group functions that are executed in sequence or that are triggered by the same event.
- Must not be too specific if not necessary

Finally, each use case must be given a meaningful name that summarises the functions performed.

## Definition of associations

- Each actor must participate in at least one use case.
- Each use case must have at least one actor with which it communicates
- If two actors participate in the same use cases, it is possible to combine them into a single actor.

## Description of use cases

- It is useful to consider both the main scenario and alternative and exceptional scenarios
- For each scenario it is necessary to specify
    - how and when the use case starts
    - who starts the use case
    - the interaction between actor and use case and what is exchanged
    - how and when there is a need to store data
    - how and when the use case ends
- If there are two use cases that have slightly different behaviours but have the same actors, one can consider having a single use case with alternative scenarios.

## Structuring use cases

Identify generalisation and extension relationships:

- specialise use cases that have many alternative scenarios
- linking new use cases to the original ones by means of generalisation or "extend" relationships

Identify inclusion relations:

- identify common parts in different use cases
- linking use cases sharing a common part to the new use case (representing the shared behaviour) by means of the "include" association

# Examples of Use Case Diagrams

## 1. Passenger service

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Passenger_Service.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Passenger_Service.svg)

## 2. Broadcasting service

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Broadcasting_System.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Broadcasting_System.svg)

## 3. Restaurant

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Restaurant.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Restaurant.svg)

## 4. Sale of vehicles

![Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Vehicle_Sales_System.svg](Use%20Case%20Diagram%2028433171f0d741f2a250a55c0f069d27/Vehicle_Sales_System.svg)
