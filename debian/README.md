Generating the Debian Package
=============================

Download the Source Repository
------------------------------

    git clone --recursive https://github.com/genome-vendor/vcflib.git

Enter and Setup the Source Directory
------------------------------------

    cd vcflib
    git checkout -b debian origin/debian

Run the Build Command
---------------------

    dpkg-buildpackage -uc -us --changes-option='-DDistribution=lucid-genome-development'

The debian package files will be available in the parent directory, next to
`vcflib` directory itself.
