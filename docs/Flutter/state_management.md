# State management

<image src="/assets/state-management-explainer.gif"/>

## What is the state?

When a user interacts with an application, some information needs to be changed and the UI needs to be rebuilt at that moment, that information, which is necessary to reflect changes is called the State of application at that moment.

## What is State Management?

Whether you are building web applications or mobile applications, State Management is the key for managing application views.

State Management is the strategic approach to manage all the interactions that a user performs on an application and then reflect those changes to UI, update databases, server requests etc. Any application has many UI controls such as text fields, radio buttons, buttons, checkboxes, dropdowns etc. State management refers to handling the states of such UI controls as most of the time one or more UI controls are depending on one-another, based on business logic requirements.

Every development framework has its own unique way to efficiently perform state management. Like Flutter, many frameworks have more than one approach.

## Why is State Management important?

State Management reflects the efficiency of the system and the care taken by developers to build that system so that every functionality and feature performs smoothly and precisely.

State management helps to align and integrate the core business logic inside the application with servers and databases. Without proper state management burden on users will increase and that would certainly decrease the effectiveness of an application.

As well as by centralizing everything with State management, it will be easier to maintain a code base and will in-turn improve the code-quality and readability.


## Conceptual Types of States
At any point in time of the flutter application lifecycle, your application will be in either of two below states :

a. Local / Ephemeral State

b. Shared / App state

### Local State
Whenever you need to change the state of a single page view which may contain UI controls or animation then it is considered as a local state. You can easily do that using the Stateful widget.

### Shared App State
Whenever you need to change the state of multiple widgets which are shared across your application then it is Share app State.

<iframe width="560" height="315" src="https://www.youtube.com/embed/d_m5csmrf7I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

!!! tldr "Resources"
  To know more about different state management Techniques, read <a href="https://docs.flutter.dev/development/data-and-backend/state-mgmt/options">official documentation.</a>