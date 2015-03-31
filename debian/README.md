Generating the Debian Package
=============================

In the top level source directory run the following command:

    dpkg-buildpackage -uc -us --changes-option='-DDistribution=lucid-genome-development'

afterwards, the debian package files will be available in the directory above
your command execution.
