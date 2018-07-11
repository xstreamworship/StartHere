# chi
CHI enhanced MIDI keyboard workstation

Work-in-progress
================

This is the top level project that contains manifest files to be used with 'repo' command.

You will need to download and prepare the 'repo' tool from google (if you don't have it already).  Then 'mkdir' a location to become your workspace.

Use 'repo init -u https://github.com/xstreamworship/chi --config-name' to setup workspace.  If you plan to submit changes for review using Gerrithub, then make sure that your userid used in your identity matches your github account userid.  For example, when it prompts for your email, simply provide your userid at github.  Then invoke 'repo sync' and it will all be pulled in and setup.  See doc/gerrithub-notes.txt for more information.

Manifest
========

The default.xml manifest is a symlink to chi-master-branch.xml.

Contents
========

A copy of this project is placed at etc/chi-manifest.

A couple of placeholder projects are placed under experimental.  These will be removed as real content is added.

Copyright
=========

Copyright (C) 2017, Darcy Watkins
All Rights Reserved

License
=======

Remember that 'repo' is used to manage a multi-project workspace.

See the license that is applicable per project pulled in using the manifest.

Creative Commons Attribution (CC BY) license applies to documentation (such as doc/gerrithub-notes.txt).
MIT License applies to the manifest files themselves.
