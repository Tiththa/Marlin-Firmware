# M-Firmware-Configuration
This document is based on Marlin 1.1.0 RC8 configuration for 3D printer (scratch mode)

Introduction
Marlin is a huge C++ program composed of many files, but here we’ll only be talking about the two files that contain all of Marlin’s compile-time configuration options:

Configuration.h contains the core settings for the hardware, language and controller selection, and settings for the most common features and components.
Configuration_adv.h serves up more detailed customization options, add-ons, experimental features, and other esoterica.
These two files contain all of Marlin’s build-time configuration options. Simply edit or replace these files before building and uploading Marlin to the board. A variety of pre-built configurations are included in the example_configurations folder to get you started.

To use configurations from an earlier version of Marlin, try dropping them into the newer Marlin and building. As part of the build process, the SanityCheck.h will print helpful error messages explaining what needs to be changed.

Compiler Directives
Marlin is configured using C++ compiler directives. This allows Marlin to leverage the C++ preprocessor and include only the code and data needed for the enabled options. This results in the smallest possible binary. A build of Marlin can range from 50K to over 230K in size.




