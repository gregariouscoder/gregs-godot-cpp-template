# gregs-godot-cpp template
This repository serves as a quickstart template for GDExtension development with Godot 4.0+ and cmake as the primary
meta-builder.

## Contents
* Preconfigured source files for C++ development of the GDExtension ([src/](./src/))
* An empty Godot project in [project/](./project), to test the GDExtension
* godot-cpp as a submodule (`godot-cpp/`)

## How To Use This Template

To use this template, log in to GitHub and click the green "Use this template" button at the top of the repository page. This will let you create a copy of this repository with a clean git history.

To get started with your new GDExtension, do the following:

* Clone your repository to your local computer
* Initialize the godot-cpp git submodule via `git submodule update --init`
* Go to the CMakeLists.txt and change the LIBNAME from EXTENSION-NAME to the intended name. Ensure there are no spaces.
* Change the paths of the to be loaded library name inside the [project/bin/example.gdextension](./project/bin/example.gdextension) file, by replacing `EXTENSION-NAME` with the name you chose for `libname`.
* Change the `entry_symbol` string inside [project/bin/example.gdextension](./project/bin/example.gdextension) file.
    * Rename the `example_library_init` function in [src/register_types.cpp](./src/register_types.cpp) to the same name you chose for `entry_symbol`.
* Change the name of the `project/bin/example.gdextension` file. This file does not need a specific name.
