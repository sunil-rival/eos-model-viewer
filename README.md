# eos-model-viewer
3D model viewer for the eos Morphable Model library

This is a viewer that displays Morphable Models from the eos Morphable Model library ([github.com/sunil-rival/eos](https://github.com/sunil-rival/eos)).
It allows to play around with the shape and colour PCA models as well as the blendshapes.

![Screenshot of the viewer](https://github.com/sunil-rival/eos-model-viewer/blob/master/doc/viewer_screenshot.png)


## Build & installation

It uses the libigl 3D viewer and nanogui.

**Note:** The viewer works well, but the code is not very polished and will crash if you do unexpected things (e.g. cancel the loading dialogues).
The CMake scripts are in serious alpha-stage - You are on your own compiling it!

Make sure to clone the repository with `--recursive`, or, if already cloned, run `git submodule update --init --recursive`.

There is a Windows binary in the Releases section which may or may not work on other systems, none exists for Linux yet.

## Running the viewer

The viewer can be given a `-m` and `-b` options to open a specific model and blendshapes. If you don't specify these options, a GUI file dialog will pop up, asking you to first select the model, and then the blendshapes file.
