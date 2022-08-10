# Stateful and stateless widgets

A widget is either stateful or stateless. If a widget can change—when a user interacts with it, for example—it’s stateful.

A stateless widget never changes. Icon, IconButton, and Text are examples of stateless widgets. Stateless widgets subclass StatelessWidget.

A stateful widget is dynamic: for example, it can change its appearance in response to events triggered by user interactions or when it receives data. Checkbox, Radio, Slider, InkWell, Form, and TextField are examples of stateful widgets. Stateful widgets subclass StatefulWidget.

A widget’s state is stored in a State object, separating the widget’s state from its appearance. The state consists of values that can change, like a slider’s current value or whether a checkbox is checked. When the widget’s state changes, the state object calls setState(), telling the framework to redraw the widget.

## Stateless widget
Stateless widgets do not require mutable state, i.e., it is immutable.

In simple words, Stateless widgets cannot change their state during the runtime of the app, which means the widgets cannot be redrawn while the app is in action.

The structure of a Stateless widget looks like this:

<image src="/assets/stateless_widget_structure.png"/>

So, let’s understand what is there in this small code snippet.

The name of this Stateless Widget is “StartScreen”, inside which we have to override the “build” method. This build method takes in a “BuildContext” as the parameter and returns a widget. That’s why you can see that the return type of the build method is a widget. And this the place where you can design the UI of this screen, which is Stateless.

In Stateless widget, The “build” method can be called only ONCE while the app is in action, which is responsible for drawing the widgets on to the device screen.

If you want to redraw the Stateless Widget, then you will need to create a new instance of the widget


## Stateful widget
Stateful widgets have a mutable state, i.e., they are mutable and can be drawn multiple times within its lifetime.

They are the widgets which can change their state multiple times and can be redrawn on to the screen any number of times while the app is in action.

The structure of a Stateful widget looks like this:

<image src="/assets/stateful_widget_structure.png"/>

The name of the widget is again “StartScreen”, but now it overrides the “createState” method, instead of the “build” method, which returns the instance of the class “_StartScreenState”.

The class “_StartScreenState” extends from State<> which takes “StartScreen” as a template input.

Now, this “_StartScreenState” overrides the “build” method and returns a widget. This is where you can define the UI of the app, which is Stateful. As it is a Stateful widget you can call the build method any number of times, which will redraw the widgets on the screen.

So, how can you call the build method?
It’s really easy, you can use the “setState” method to call the build method, which will, in turn, redraw the widgets. This is the most important method you will need to use with any Stateful widget, to really use the statefulness of the widget.

!!! tldr "Resources"
 <a href="https://medium.com/flutter-community/flutter-stateful-vs-stateless-db325309deae">official documentation.</a>