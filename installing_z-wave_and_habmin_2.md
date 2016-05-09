Installing Z-Wave & HABmin 2
-------------------------------

Introduction
==============

Setting up the Z-Wave protocol inside OpenHab 2 requires two steps :
- Z-Wave binding install
- HABmin install

In this chapter:
- I have chosen to download the latest nigth build, as HABmin2 2 is in a beta phase,


Z-Wave binding install
======================

We install Z-Wave binding _before_ HABmin as HABmin relies on the first one.

Installing this binding is quite straightforward. It is to be done through the Paper UI of OpenHab.

1. Open your browser web at [http://localhost:8011], you should see the following screen :

![OpenHab 2 Welcome screen](Accueil_Openhab.png)

2. Click on __Paper UI__ tile, you should see the following screen :

3. In the left column, select __Extensions__. The list of the bindings appears.

4. Scroll down to Z-Wave binding, click on "install" (at the right).

5. After some times, the Z-Wave binding is installed and the display has changed. The logo of the binding is now blue, and "uninstall" has replaced "install".

> After a reasonable wait, if the progress bar is still on the screen and nothing else has changed on the display, try to refresh the page.


HABmin install
======================

We install HABmin _after_ the Z-Wave binding as HABmin relies on the last one.

HABmin is not yet integrated to the Karaf architecture. So, we have to install it manually.

1. Search for the latest build of HABmin 2 at the adress [https://github.com/cdjackson/HABmin2/tree/master/output]

2. Click on the org.openhab.ui.habmin_2.0.0.SNAPSHOT-0.1.4.jar link, this screen appears :

3. At the left on the screen __click on the RAW__ button. Other way of downloading HABmin2 will corrupt the software.

4. The download finished, back to the terminal, at the OpenHab> prompt :

	cal:OpenHab admin$ ./start.sh
	Launching the openHAB runtime...

    	                      __  _____    ____
	  ____  ____  ___  ____  / / / /   |  / __ )
	 / __ \/ __ \/ _ \/ __ \/ /_/ / /| | / __  |
	/ /_/ / /_/ /  __/ / / / __  / ___ |/ /_/ /
	\____/ .___/\___/_/ /_/_/ /_/_/  |_/_____/
	    /_/                        2.0.0-SNAPSHOT

	Hit '<tab>' for a list of available commands
	and '[cmd] --help' for help on a specific command.
	Hit '<ctrl-d>' or type 'system:shutdown' or 'logout' to shutdown openHAB.

	openhab>

5. stop OpenHab by keyboarding logout and enter :

	openhab> logout

6. A few seconds after, the terminal prompt is displayed :

	openhab> logout
	cal:OpenHab callas$

7. Move the HABmin software from the _download_ folder to the _addon_ folder

	> cal:OpenHab admin$ mv ../Downloads/org.openhab.ui.habmin_2.0.0.SNAPSHOT-0.1.4.jar addons

> Time for a trick
>
> org.openhab.ui.habmin 2.0.0.SNAPSHOT-0.1.4.jar  can be a little difficult to type. Terminal allows us to use auto completion to avoid that :
> just type the beginning, i.e. : _mv ../Downloads/org.op_ and press the tab key. Terminal will complete the name for you.



