# Macbeth-style-GUI-creation-guide
Guide for creating highly efficient application GUIs using visual menus, symbols, keybinds, and user customization
## User Workspace
The User Workspace is area where the main contents of the program will be interacted through
In a text application, this would be the text document itself
In a 3D modeling application, this would be the 3D viewport
## Actions Interface
The Actions Interface is the panel where all currently active actions are accessible/visible
It does not necessarily have to be present on a certain side of the screen, be tethered to a particular location, or be visible at all times
It may contain a function to minimize or hide it
If it is minimized/hidden, an action or keybind must be displayed somewhere on-screen with the functionality to maximize/unhide it
## Action Box
Action boxes contain information and/or functionality relating to an individual Action or Action Submenu
An Action Box may contain any number of items that may be implemented within an Action Box
The best practice minimum for an Action Box is to contain a Symbol, Name, Keybind, and Onclick action
An action box with any items should also have a name
## Action Symbol
An Action Symbol is a simple symbol used to represent the Action
Action Symbols should be minimally complicated, and scalable
SVGs are the best option for implementing Action Symbols
## Action Name
An Action Name is a simple, minimal-length name describing the Action
Action Names should aim to be one, two, or three words long, but may be longer
## Action Keybind Hint
An Action Keybind Hint describes the keybind attached to the Action, if any
A keybind should be written in plain text, with each key referenced visually separated, and ordered according to the order in which to press them (respecting the language text direction of the application)
## Action Description
An Action Description is a pain text description of the functionality/effect offered by the Action
Action Descriptions are best applied only when the Action functionality/effect is not intuittive, visually noticeable, or easily understood based on the name alone
## Action Elements
Action Elements are advanced parameters for the Action, best applied to configurable Actions or Actions representing attributes of application aspects that the user can manipulte (for example, in a 3D modelling program, an action may be used to represent the current dimensions of a rectangular prism using multiple numerical input boxes)
## Preferances Action
A good best practice is to bind a Preferances Action Menu opening Action at the bottom of the Actions Interface (either floating or at the end of the list), where users can manipulate settings based on application customization
Customization options should be contained in individual configuration files, to make the full range of customizations made by users portable, and to amke it easy to switch between configurations. If so, all settings based on such configuraton files should be contained within the same Action Submenu, which should also visually identify which configuration file is in use, and which are available.
