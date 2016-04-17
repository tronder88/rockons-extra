# rockons-extra

3rd party hub for Rocko-ons to Rockstor NAS distro.

Instructions how to install from https://github.com/rockstor/rockon-registry/ which is the original repo for rock-ons

How can I add app from this repo?

If you are familiar with Docker and know how to run apps by hand, you can create a Rock-on for the same with a little bit of craft. There are three broad steps.

Configure the Rock-On service on your Rockstor system. Please see the http://rockstor.com/docs/docker-based-rock-ons/overview.html.

Download the rockon you need via wget or download zip option (do not rightclick in windows and save target as..), winscp etc. to /opt/rockstor/rockons-metastore/[app].json. Hit update in the Web-UI and install your brand new Rock-On!

-To remove Rock-on, please uninstall rockon, and then remove JSON file from rockons-metastore folder. Hit update again in web-ui and it should be removed.

Please contribute to the Rockstor community on forum.rockstor.com and opt in for a subscription to keep the development of distro running


Short description of differences if existing image in Rock-ons:

-Plex: Has a separate mapping for transcoding since it is a part of Plex. Is not default for image, "/transcode" is the default pasth    inside plex.

-Duplicati - works, not tested too much, version is canary. When 2.0 is stable, I will change to stable channel.

Owncloud is not ready, will give error. Debug pending
