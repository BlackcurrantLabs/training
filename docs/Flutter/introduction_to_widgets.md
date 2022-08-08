# Widgets


Flutter widgets are built using a modern framework that takes inspiration from React. The central idea is that you build your UI out of widgets. Widgets describe what their view should look like given their current configuration and state.


When a widget’s state changes, the widget rebuilds its description, which the framework diffs against the previous description in order to determine the minimal changes needed in the underlying render tree to transition from one state to the next.


The minimal Flutter app simply calls the runApp() function with a widget:

    import 'package:flutter/material.dart';

    void main() {
    runApp(
        const Center(
        child: Text(
            'Hello, world!',
            textDirection: TextDirection.ltr,
        ),
        ),
    );
    }

The runApp() function takes the given Widget and makes it the root of the widget tree. In this example, the widget tree consists of two widgets, the Center widget and its child, the Text widget. The framework forces the root widget to cover the screen, which means the text “Hello, world” ends up centered on screen. The text direction needs to be specified in this instance; when the MaterialApp widget is used, this is taken care of for you, as demonstrated later.


## Basic widgets
Flutter comes with a suite of powerful basic widgets, of which the following are commonly used:

### Text
The Text widget lets you create a run of styled text within your application.
### Row, Column
These flex widgets let you create flexible layouts in both the horizontal (Row) and vertical (Column) directions. The design of these objects is based on the web’s flexbox layout model.
### Stack
Instead of being linearly oriented (either horizontally or vertically), a Stack widget lets you place widgets on top of each other in paint order. You can then use the Positioned widget on children of a Stack to position them relative to the top, right, bottom, or left edge of the stack. Stacks are based on the web’s absolute positioning layout model.
### Container
The Container widget lets you create a rectangular visual element. A container can be decorated with a BoxDecoration, such as a background, a border, or a shadow. A Container can also have margins, padding, and constraints applied to its size. In addition, a Container can be transformed in three dimensional space using a matrix.

## Below example combine these and other widgets:
    import 'package:flutter/material.dart';

    class MyAppBar extends StatelessWidget {
    const MyAppBar({required this.title, super.key});

    // Fields in a Widget subclass are always marked "final".

    final Widget title;

    @override
    Widget build(BuildContext context) {
        return Container(
        height: 56.0, // in logical pixels
        padding: const EdgeInsets.symmetric(horizontal: 8.0),
        decoration: BoxDecoration(color: Colors.blue[500]),
        // Row is a horizontal, linear layout.
        child: Row(
            children: [
            const IconButton(
                icon: Icon(Icons.menu),
                tooltip: 'Navigation menu',
                onPressed: null, // null disables the button
            ),
            // Expanded expands its child
            // to fill the available space.
            Expanded(
                child: title,
            ),
            const IconButton(
                icon: Icon(Icons.search),
                tooltip: 'Search',
                onPressed: null,
            ),
            ],
        ),
        );
    }
    }

    class MyScaffold extends StatelessWidget {
    const MyScaffold({super.key});

    @override
    Widget build(BuildContext context) {
        // Material is a conceptual piece
        // of paper on which the UI appears.
        return Material(
        // Column is a vertical, linear layout.
        child: Column(
            children: [
            MyAppBar(
                title: Text(
                'Example title',
                style: Theme.of(context) //
                    .primaryTextTheme
                    .headline6,
                ),
            ),
            const Expanded(
                child: Center(
                child: Text('Hello, world!'),
                ),
            ),
            ],
        ),
        );
    }
    }

    void main() {
    runApp(
        const MaterialApp(
        title: 'My app', // used by the OS task switcher
        home: SafeArea(
            child: MyScaffold(),
        ),
        ),
    );
    }

Output:

<image src="/assets/flutter-widget-output.png" width=200px/>
