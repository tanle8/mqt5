# Contents:
## Objectives: 
Ensuring your Qt foundatons are *safe* before studying *advanced* concepts.

-----
- Create a simple **todo** application using Qt Creator.
	- This application will display a list of tasks that you can `create`/`update`/`delete`.

- Cover the `Qt Creator` and `Qt Designer` intefaces,
- An introduction to the `signal/slot` mechanism,
- The creation of a custom widget with custom `signals/slots`, and its intefration into your application.

[C++ 14 features]
- implement a todo app using new C++14 semantics:
	- lambdas,
	- auto variables,
	- for loops

## Goal:
Be able to create a desktop application with a flexible UI using Qt widgets and new C++ semantics.

## Topics:
- Qt project basic structure
- Qt Desinger interface
- UI fundamentals
- Signals and Slots
- Custom `QWidget`
- C++14 lambda, auto, for each

-----------------------------------------
# 1. Creating a project
## 1.1 `.pro` file is Qt's configuration project file.
- As Qt adds speicfic file formats and C++ keywords, an intermediate build step is performed, parsing all files to generate final files.
- This rocess is done by `qmake`, an executable from the Qt SDK.
- It will also generate the final Makefiles for your project.

A basic `.pro` file generally contains:
- Qt modules used (`core`, `gui`, and so on)
- Target name (`todo`,`todo.exe`, and so on)
- Project template (`app`, `lib`, and so on)
- Sourcesm headers, and forms


