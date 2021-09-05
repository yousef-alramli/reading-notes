# Component-Based Architecture

Component-based architecture focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties. It provides a higher level of abstraction and divides the problem into sub-problems, each associated with component partitions.
## What is a Component?

A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture.

A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties.

## Views of a Component
A component can have three different views − object-oriented view, conventional view, and process-related view.

- Object-oriented view
- Conventional view
- Process-related view

## Characteristics of Components
Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

- Replaceable − Components may be freely substituted with other similar components.

- Not context specific − Components are designed to operate in different environments and contexts.

- Extensible − A component can be extended from existing components to provide new behavior.

- Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality.

- Independent − Components are designed to have minimal dependencies on other components.

## Principles of Component−Based Design
A component-level design can be represented by using some intermediary representation (e.g. graphical, tabular, or text-based) that can be translated into source code.

### Component-Level Design Guidelines
Creates a naming conventions for components that are specified as part of the architectural model and then refines or elaborates as part of the component-level model.
### Conducting Component-Level Design
Recognizes all design classes that correspond to the problem domain as defined in the analysis model and architectural model.
## Advantages


- Reduced cost 

- Ease of development 

- Reusable

- Modification of technical complexity services.

- Reliability 

- System maintenance and evolution 

- Independent 




# Props  



## What is props short for?
Props stand for properties and is a special keyword in React

## How are props used in React?

1. Defining Attribute & Data : 
We can define our own attributes & assign values with interpolation { }.

2.  Step: Passing Data using Props:
Passing props is very simple. Like we pass arguments to a function, we pass props into a React component and props bring all the necessary data.

3. Rendering Props Data:
we have created an attribute and its value, then we passed it through props but we still can’t see it because we haven’t rendered it yet.

## What is the flow of props?

uni-directional flow. (one way from parent to child)

