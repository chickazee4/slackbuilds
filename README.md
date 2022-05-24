This repository contains precompiled binary packages for some SlackBuilds, compatible with Slackware64-current. This is not a package repository suitable for use with slapt-get or similar; you'll need to download and install packages ad hoc. (I would like to configure it as a package repository in the future, though.)

In each directory there is a license file for the software and a subdirectory. Each subdirectory includes a .tgz package. SlackBuilds are not being redistributed here in order to avoid disseminating out of date scripts and in order to slightly simplify licensing. All package names correspond to the name of their SlackBuild so you can refer back to their listing on SlackBuilds.org if necessary.

Software here which requires dependencies can have those dependencies satisfied using a combination of Slackware official packages, [AlienBOB's builds](http://www.slackware.com/~alien/slackbuilds/), and other packages included here. You shouldn't need to build any software from source to support any of the pakckages in this repository.

Included also is a very small shell script (`sb`) that I like to use to shorten the commands necessary to install and preserve a SlackBuild package. In order to use it, you should be inside a directory with the name of the software to be built (no version) containing the SlackBuild and other necessary files, for example:

    softwarename
	|-  README
	|-  slack-desc
	|-  softwarename.info
	|-  softwarename.SlackBuild
	|-  softwarename-version.tar.xz

From here you can run `sb` to 1) run the SlackBuild script and produce a package, 2) copy the package back to the source folder, and 3) install the package.
