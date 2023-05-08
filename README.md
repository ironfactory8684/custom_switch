<h1> Custom Switch</h1>
It's easy to implement custom switches for Flutter. You can change the custom height and width, border of switches and toggles, border radius, color, and toggle size. 

<br> 
<br> 
Here's how the code works:
<br> 
<br> 

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

<br> 
<h4>Sample Usage</h4>

```
  CustomSwitch(
            value: isSwitched,
            onChanged: (value) {
              setState(() {
                isSwitched = value;
              });
            },
          )
```
