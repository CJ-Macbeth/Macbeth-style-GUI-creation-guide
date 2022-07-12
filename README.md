# Macbeth-style-GUI-creation-guide
Guide for creating highly efficient application GUIs using visual menus, symbols, keybinds, and user customization

<img src="Images/Macbeth%20UI%20Guide.svg" style="width:50%;" />

## User Workspace
The User Workspace is area where the main contents of the program will be interacted through.<br>
In a text application, this would be the text document itself.<br>
In a 3D modeling application, this would be the 3D viewport.<br>

<img src="Images/Application%20Workspace.svg" style="width:50%;" />

## Actions Interface
The Actions Interface is the panel where all currently active actions are accessible/visible.<br>
It does not necessarily have to be present on a certain side of the screen, be tethered to a particular location, or be visible at all times.<br>
It may contain a function to minimize or hide it.<br>
If it is minimized/hidden, an action or keybind should be displayed somewhere on-screen with the functionality to maximize/unhide it.<br>

<img src="Images/Actions%20Interface.svg" style="width:50%;" />

## Action Box
Action boxes contain information and/or functionality relating to an individual Action or Action Submenu.<br>
An Action Box may contain any number of items that may be implemented within an Action Box.<br>
The best practice minimum for an Action Box is to contain a Symbol, Name, Keybind, and Onclick action.<br>
An action box with any items should also have a name.<br>

<img src="Images/Action%20Box.svg" style="width:50%;" />

## Action Symbol
An Action Symbol is a simple symbol used to represent the Action.<br>
Action Symbols should be minimally complicated, and scalable.<br>
SVGs are the best option for implementing Action Symbols.<br>

<img src="Images/Action%20Symbol.svg" style="width:50%;" />

## Action Name
An Action Name is a simple, minimal-length name describing the Action.<br>
Action Names should aim to be one, two, or three words long, but may be longer.<br>

<img src="Images/Action%20Name.svg" style="width:50%;" />

## Action Keybind Hint
An Action Keybind Hint describes the keybind attached to the Action, if any.<br>
The keybind described by an Action Keybind Hint must be active when the Action is visible.<br>
Keybinds may be replaced/change depending on the Action Submenu the user has navigated to.<br>
A keybind should be written in plain text, with each key referenced visually separated, and ordered according to the order in which to press them (respecting the language text direction of the application).<br>
All keybinds should be represented by Actions for the duration that they are active.<br>

<img src="Images/Action%20Keybind%20Hint.svg" style="width:50%;" />

## Action Description
An Action Description is a pain text description of the functionality/effect offered by the Action.<br>
Action Descriptions are best applied only when the Action functionality/effect is not intuittive, visually noticeable, or easily understood based on the name alone.<br>

<img src="Images/Action%20Description.svg" style="width:50%;" />

## Action Elements
Action Elements are advanced parameters for the Action, best applied to configurable Actions or Actions representing attributes of application aspects that the user can manipulte (for example, in a 3D modelling program, an action may be used to represent the current dimensions of a rectangular prism using multiple numerical input boxes).

<img src="Images/Action%20Elements.svg" style="width:50%;" />

## Preferances Action
A good best practice is to bind a Preferances Action Menu opening Action at the bottom of the Actions Interface (either floating or at the end of the list), where users can manipulate settings based on application customization.<br>
Customization options should be contained in individual configuration files, to make the full range of customizations made by users portable, and to make it easy to switch between configurations. If so, all settings based on such configuraton files should be contained within the same Action Submenu, which should also visually identify which configuration file is in use, and which are available.<br>

<img src="Images/Preferances%20Action.svg" style="width:50%;" />
