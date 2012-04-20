Conjcraft
==============

Conjcraft is an open source mod for [Minecraft](http://www.minecraft.net/) written in [Clojure](http://clojure.org/). It uses [ModLoader](http://www.minecraftdl.com/modloader-risugami-downloads/) and [Minecraft Coder Pack](http://mcp.ocean-labs.de/index.php/Main_Page) (aka MCP) (thanks guys!).


Installing the mod
----

*Quick Note:* All instructions here assume you have the current latest stable version of Minecraft, which is [1.2.5](http://www.minecraftwiki.net/wiki/Version_history#1.2.5).

This assumes you have basic dev tool setup (specifically wget and curl) and lawfully own a copy of Minecraft.

If you don't have [ModLoader](http://www.minecraftdl.com/modloader-risugami-downloads/) install, you can install it and the mod in one line

	$ curl https://raw.github.com/danielribeiro/conjcraft/master/setup_scripts/full_install.sh | bash

If you have [ModLoader](http://www.minecraftdl.com/modloader-risugami-downloads/) installed, you can install the mod in one line:

	$ curl https://raw.github.com/danielribeiro/conjcraft/master/setup_scripts/install.sh | bash


Installing the mod (full developer mode, including MCP)
----
This is not required if you just wanna play with the recipes, as they are all plain text clojure files included in the conjcraft folder installed on your home directory (the above installation creates them).

This setup assumes the setup above, and that you have git installed.

	$ curl https://raw.github.com/danielribeiro/conjcraft/master/setup_scripts/dev_install.sh | bash

You do not need [ModLoader](http://www.minecraftdl.com/modloader-risugami-downloads/) installed, unless you want to release your changes (just run ./release.sh). In this case, after the setup, just change to minecraft_modding and run

	$ ./startclient.sh

If you cloned this git repo, you can setup everything just by using:

	$ ./setup_scripts/setup.sh


Running tests
----
The recipe [DSL](http://www.manning.com/ghosh/) has basic clojure/test tests in the recipe_dsl_test.clj. They can be run with:

	$ ./run_tests.sh

Locally installing your changes
---- 
To install your changes (java ones, as, by default, clojure changes will be in the correct path if you haven't changed anything), just run

	$ ./release.sh

This requires [ModLoader](http://www.minecraftdl.com/modloader-risugami-downloads/) installed. If you have not it installed, you can do it in one line with:

	$ ./setup_scripts/install_modloader.sh


Meta
----

Created by Daniel Ribeiro. Not affiliated with Mojang. Minecraft is a trademark of [Mojang](http://mojang.com/).

Released under the MIT License: http://www.opensource.org/licenses/mit-license.php

https://github.com/danielribeiro/conjcraft
