# [PullTheStrings](http://www.virtualmarionette.grifu.com)

## Marionette Programming Language

Pull The Strings is a digital puppetry visual node-based control environment for performance animation.
It acts as a middle-ware interface between puppeteers and puppets, between device drivers and driven objects, between input interfaces and applications.

It is a marionette programming engine that works as a digital mediator between devices and applications, it provides the building blocks for the digital puppeteer to establish the manipulation semantics. It is a visual programming language inspired by the strings of the marionettes and by the patch cords that connect modules in the old analog video synthesizers. In this environment the signals are processed and sent to the network. Finally the data arrives to Remote Control for Unity which is a plugin that facilitates the mapping of OSC messages.

It was designed with a minimalistic but intuitive interface and was developed in C++ with Openframeworks making use of multiple add-ons to provide their main features. 
A multidisciplinary enviorment (MMMM:  Multi-plataform, Multi-modal, Multi-mediator, Multi-user).
An enviorment for artists with non-programming background. Design for digital puppeteers.


Pull the strings is a middle-ware, an interface between applications, devices, and performing objects. It can be consider a visual programming environment for remote control made for artists and designers.
Sometimes you find hard to use one environment or application that offers all those nice features that your are looking for, so why not use a multiple set of applications in real-time ?
The goal of Pull the Strings is to facilitate the use and control of all your resources found in your computer and on the network.
An abstraction from technology making use of generic signals and communication protocols.
Connects, and transforms signals from input and virtual devices into performing object controls. Map and orchestrate multimedia data using OSC, DMX, MIDI and VRPN
Is a remote control application, an interface that connects inputs to outputs and provides a series of functionalities that helps to control the animation. It is a OSC-based environment and all nodes work with OSC format.


Version Alpha 0.050316 (first release 6 March 2016)
Pull The Strings will become open source soon. It is completly free to use in your art, research, or professional projects.
Built with [openFrameworks](http://www.openframeworks.cc).
It is developed by Luís Leite (GRIFU) for the Digital Media PhD with the support of FCT - Fundação para a Ciência e a Tecnologia.


![Pull The Strings](https://vimeo.com/grifu/pre-pullthestrings)


## Download

Download Pull The Strings: 

[Mac OSX (32 bits) ]
[Windows (32 bits) ]

## Demo video
https://vimeo.com/grifu/pullthestrings-armtrack


## License

    Copyright 2012-2016 Luís Leite

                    GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007

 Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 Everyone is permitted to copy and distribute verbatim copies
 of this license document, but changing it is not allowed.

                            Preamble

  The GNU General Public License is a free, copyleft license for
software and other kinds of works.




## Pull The Strings Interface

Pull The Strings allows you to create, save and load your projects.
You should start by always saving your project first which will create a folder to gather all the files needed.
To navigate through the canvas use the <SPACE> key, to open the menu use the <TAB> and then start writing the operator name or use the mouse to navigate.
To delete an operator just use the <BACKSPACE> to access to operators options click the <*> on the operator.
Connect nodes from the outputs to the inputs. Add new input nodes by clicking the <+ O> button.
You can create multiple graph windows.


### OSC Communication
Pull The Strings is based on OSC protocol. It receives OSC messages and sends OSC messages and all its interface communicate internally via OSC.
You can send several messages from one output port.
It supports bonjour so you can easely find Pull The strings with Bonjour compatible applications, such as TouchOSC.
It makes use of RemoteUI to remote control the operators with other applications or devices.

### Pull The Strings operators

input.number (to create a Float or Int inside the interface or with remote applications)
input.string (to create strings)
math.scale (a scalar function with a learning input range option)
osc.combine (combine several OSC messages into one, it allows message syncincing)
osc.expand (expands an OSC message into seperated out nodes, it allows to inspect the data types and choose the address)
osc.port.in (opens port for incoming OSC data)
osc.port.out (opens port for sending)
math.dot.vec (math operations: dot between two vectors)
osc.rename (renames the address of the message)
osc.split (splits messages)
filter.data (applies signal transformations, noise reduction)
timeline.number (a time line for animation that returns a float value)
print (for debugging, it prints in the interface the incoming messages)
show.plot (makes a plot from the values)
LeapMotion support (only for the 0.321 MAC version)

## Version History

 - Alpha 003 (March 5th 2016) Mac OSX
 - Alpha 003 (Jully 8th 2016) Windows
 - Alpha 006 (November 2016) Mac OSX
 - Alpha 006 (December 2016) Windows

## Whats new in 0.6
- new operator (math.dot.vec)
- new operator (osc.rename)
- new operator (osc.split)
- new operator (filter.data)
- new operator (timeline.number)
- osc.port.out now is active by default
- new maping features included in different operators
- Leapmotion (MAC only) Pinch for leapmotion

## Whats new in 0.627
- Retrieve local IP (press the shortkey "i") (Mac only)
- OSC.Port.IN and timeline.number are initalized on start
- Keep ON is now turned on by default
- Added a Scrollbar in the operator menu
- OSC address tracer in the OSC.Port.IN

## Whats new in 0.6272
- Mouse.input operator

## Whats new in 0.6273
- input.XY operator (2D panel input to control the position of a point in space)
- Initial support for the Wiimote (very instable, accelerometer, buttons, IR)
- viewport 3D for visualization purposes, you can track the input points in the 3D space
- New menu system with the right click based on ofxClickDownMenu
- A very tiny and simple local network address to retrieve the IP address of the network adapter (press "i")

## Support

![Support](http://www.virtualmarionette.grifu.com)


## Other features
Pull The Strings as other operators that are not yet avaiable such as:
LeapMotion support for the Windows version
Wiimote support
Math operations
Recording OSC performance

## Developed with
Pull The Strings is based on ofxDuct and makes use of many other ofxAddons such as:
ofxRemoteUI
ofxLeapMotion
Wiiuse
ofxBonjour
ofxAppGLFWindowMulti
ofxHistoryPlot
ofxUI
ofxTimecode
ofxMSATimer
ofxRange
ofxTimeline
ofxOsc
ofxGui
ofxMSAInteractiveObject
ofxClickDownMenu
