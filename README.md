# xfMediaHotKey
Fix for XFCE's media hotkeys. Makes them able to work with multiple applications.

Introduction
============

This is a python implementation of a workaround on a XFCE4 "problem". Its media hotkeys do not work with multiple applications. In the Linux distro that I'm using (Fedora 21/22), I've observed that the default keyboard shortcuts (previous, next, play/pause) only work for the default audio player(Pragha). As I came across this "problem", I made this simple Python workaround.


Configuration
============

The only thing that needs to be done for this to work, is replace XFCE's keyboard shortcuts from pragha's to xfmhk. 
In xfce4-keyboard-settings, on the Application Shortcuts tab, you need to replace:
    * "pragha --next" for "/path/to/xfmhk -next";
    * "pragha --prev" for "/path/to/xfmhk -previous";
    * "pragha --pause" for "/path/to/xfmhk -play-pause";


Requirements
============

xfMediaHotKey requires the following:
    *python >= 2.7