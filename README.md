Repo Manifests for Projects
===========================

This is the top level project that contains manifest files for projects to be used with 'repo' command.
Select the repo manifest for the project and the tool will assemble a workspace for it, checking out
from all dependent repos, and set it up for use.

Contents
========

chi-master-branch.xml - CHI enhanced MIDI keyboard workstation

---

The default.xml manifest is a symlink to chi-master-branch.xml.  The default.xml is deprecated and will be dropeed.
The manifest for Chi will be renamed to drop the 'master' once the branch names are updated.

Getting Started
===============

You will need to download and prepare the 'repo' tool from google (if you don't have it already).  Then 'mkdir' a location to become your workspace.

If you don't have Google's 'repo' script, then download it as follows:

  $: mkdir -p ~/bin

  $: curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo

  $: chmod a+x ~/bin/repo

To checkout a workspace for a specific project, pick the [manifest-name], then...

  $: mkdir mycheckout

  $: cd mycheckout

  $: repo init --config-name -u git@github.com:xstreamworship/StartHere.git --config-name -m [manifest-name].xml

  $: repo sync

A copy of StartHere project may be placed in workspace at etc/StartHere.  Changes made to a manifest file will only
show up in your workspace after it has been merged and then you invoke 'repo sync'.  If you need to customize the
layout in your workspace, use local_manifest files (see the doc for 'repo' for more infomation).

Copyright
=========

Copyright (C) 2017-2022, Darcy Watkins
All Rights Reserved

License
=======

Since 'repo' is used to manage a multi-project workspace, multiple licesnes may apply.

See the license that is applicable per project pulled in using the manifest.

Creative Commons Attribution (CC BY) license applies to StartHere project documentation.
MIT License applies to the manifest files themselves.
