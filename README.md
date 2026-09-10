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

* clone your repository to your local computer
* initialize the godot-cpp git submodule via `git submodule update --init`
* Go to the CMakeLists.txt and change the LIBNAME from EXTENSION-NAME to the intended name. Ensure there are no spaces.
* change the paths of the to be loaded library name inside the [demo/bin/example.gdextension](./demo/bin/example.gdextension) file, by replacing `EXTENSION-NAME` with the name you chose for `libname`.
* change the `entry_symbol` string inside [demo/bin/example.gdextension](./demo/bin/example.gdextension) file.
    * rename the `example_library_init` function in [src/register_types.cpp](./src/register_types.cpp) to the same name you chose for `entry_symbol`.
* change the name of the `demo/bin/example.gdextension` file
