manifest
========

manifest for downloading git repositories


Install the `repo` utility:

$ mkdir ~/bin
$ curl https://dl-ssl.google.com/dl/googlesource/git-repo/repo > ~/bin/repo
$ chmod a+x ~/bin/repo

Download the bitbake metadata required to build BSP:

$ export PATH=${PATH}:~/bin
$ mkdir workspace
$ cd workspace
$ repo init -u https://github.com/shivdasgujare/manifest.git -b branchname

  Possible branches are :
	beageboard - downloads and builds BSP for beageboard.
	hence command to download BSP for beagleboard will be,
	repo init -u https://github.com/shivdasgujare/manifest.git -b beagleboard

$ repo sync


This git repository describes how to clone different
repositories to local machine for building Linux
This is based on android manifest.xml
