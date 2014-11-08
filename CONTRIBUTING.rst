If on Ubuntu 14.04 + or Mint 17, you should be able to simply clone the github
repo, run ``sudo apt-get build-dep nemo``, then ``dpkg-buildpackage`` from the
source root.  This will generate .deb packages in the parent folder that you
can then install using dpkg.  One note:  Once you've done this once, you can do
a lot of subsequent testing of code changes by just running ``sudo make
install``, which will run much more quickly than dpkg-buildpackage (and no
installing packages).

Just be sure to kill nemo or ``nemo --quit`` after installing a new version, to
make sure you're not still running the previous one.

A bit of info here about building: `http://segfault.linuxmint.com/2013/05/how-
to-not-break-your-de-in-a-few-steps/`_

There's not much in the way of documentation for us - what we do have is on
github mostly, in the Cinnamon wiki:
`https://github.com/linuxmint/Cinnamon/wiki`_
