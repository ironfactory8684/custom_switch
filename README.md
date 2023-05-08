<h1> Custom Switch</h1>
It's easy to implement custom switches for Flutter. You can change the custom height and width, border of switches and toggles, border radius, color, and toggle size. 

Here's how the code works:

The CustomSwitch class extends StatefulWidget, indicating that it has mutable state that can change over time.

```
The CustomSwitch class has several properties that can be customized:

onChanged: A callback function that takes a boolean value as a parameter. This function will be called when the switch is toggled.
value: A boolean value representing the current state of the switch.
trackWidth, trackHeight: Dimensions of the switch track.
toggleWidth, toggleHeight: Dimensions of the switch toggle.
toggleActiveColor: Color of the toggle when the switch is active.
trackInActiveColor, trackActiveColor: Colors of the switch track when it is inactive and active, respectively.
The _CustomSwitchState class is the state class for the CustomSwitch widget. It manages the state of the switch.
```
In the initState method, the initial state of the switch is set based on the value property provided to the CustomSwitch widget.

The build method creates the switch UI using Flutter's widget hierarchy. It wraps the switch in a GestureDetector to handle taps and a Container to control the size of the switch.

The switch UI consists of two main components:

The track: A Container with rounded corners and a background color that changes based on the switch state.
The toggle: A Container with a circular shape and a color that changes based on the switch state. It is animated horizontally using AnimatedPositioned when the switch is toggled.
When the switch is tapped or dragged horizontally, the _isSwitched state is updated, and the onChanged callback is called with the new switch state.

You can use this CustomSwitch widget in your Flutter application by instantiating it and passing the required properties, such as onChanged and value.
