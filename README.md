Mercurial Ansible Module
========================

Deploys software (or files) from Mercurial clones.

Author: Brad Olson

Maintained at: https://github.com/bradobro/ansible-module-mercurial

Usage
=====

mercurial
    repo = source repository location
    dest = destination directory for the repository clone
    revision = mercurial revspec to update CLEAN to. 
               NOTE: this param deviates from the git module's branch & version params
               because mercurial uses 'hg up -C' to switch to branch tips, tags, or
               changesets
    owner = name of the user to own the repository tree, as if this user had run Mercurial

Prerequisites
=============

Mercurial executable installed in /usr/bin/hg.


