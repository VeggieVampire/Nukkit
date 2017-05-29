Nukkit
===================
![nukkit](https://github.com/Nukkit/Nukkit/blob/master/images/banner.png)

	This program is free software: you can redistribute it and/or modify
	it under the terms of the GNU Lesser General Public License as published by
	the Free Software Foundation, either version 3 of the License, or
	(at your option) any later version.

	This program is distributed in the hope that it will be useful,
	but WITHOUT ANY WARRANTY; without even the implied warranty of
	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
	GNU Lesser General Public License for more details.

	You should have received a copy of the GNU Lesser General Public License
	along with this program.  If not, see <http://www.gnu.org/licenses/>.


__A Nuclear-Powered Server Software For Minecraft: Pocket Edition__

[![PayPayl donate button](https://img.shields.io/badge/paypal-donate-yellow.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=magicdroidx%40gmail%2ecom&lc=US&item_name=Nukkit&currency_code=USD&bn=PP%2dDonationsBF%3apaypal%2ddonate%2dyellow%2esvg%3aNonHostedGuest)
[![Gitter](https://img.shields.io/gitter/room/Nukkit/Nukkit.js.svg?style=flat)](https://gitter.im/Nukkit/Nukkit)
[![Travis](https://img.shields.io/travis/Nukkit/Nukkit.svg?style=flat)](https://travis-ci.org/Nukkit/Nukkit)

Introduction
-------------

Nukkit is nuclear-powered server software for Minecraft: Pocket Edition.
It has a few key advantages over other server software:

* Written in Java, Nukkit is faster and more stable.
* Having a friendly structure, it's easy to contribute to Nukkit's development and rewrite plugins from other platforms into Nukkit plugins.

Nukkit is **under improvement** yet, we welcome contributions. 

Get Nukkit & Plugins
--------------------

#### Recommended Sites

* __[Official Site](https://nukkit.io)__
* __[Jar Download at Circle CI](https://circleci.com/gh/Nukkit/Nukkit/tree/master/)__ (**login required**)
* __[Discussion](#discussion)__

*Thank you for visiting our official sites. Our official websites are provided free of charge, and we do not like to place ads on the home page affecting your reading. If you like this project, please [donate to us](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=magicdroidx%40gmail%2ecom&lc=US&item_name=Nukkit&currency_code=USD&bn=PP%2dDonationsBF%3apaypal%2ddonate%2dyellow%2esvg%3aNonHostedGuest). All the donations will only be used for Nukkit websites and services.*


#### Unofficial Download Mirrors
*These sites are provided by our users, Nukkit stuff are not responsible for the reliability of these sites. Jar files downloaded here are only for reference - to try the latest update or for commercial uses, compile by yourself.*

* __[Jenkins by MengCraft](http://ci.mengcraft.com:8080/job/Nukkit/lastSuccessfulBuild/)__ (**UNOFFICIAL**)

Build JAR file
-------------
- `git submodule update --init`
- `mvn clean`
- `mvn package`


Build and Install on a Raspberryp Pi<br>
-------------
Install JDK<br>
Visit http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html, click the download button of Java Platform (JDK) 8. Click to Accept License Agreement, download jdk-8-linux-arm-vfp-hflt.tar.gz for Linux ARM v6/v7 Hard Float ABI.<br>
<br>
Log-in Raspberry Pi, enter the command to extract jdk-8-linux-arm-vfp-hflt.tar.gz to /opt directory.<br>
- `sudo tar zxvf jdk-8-linux-arm-vfp-hflt.tar.gz -C /opt'
<br>
Set default java and javac to the new installed jdk8.<br>
- `sudo update-alternatives --install /usr/bin/javac javac /opt/jdk1.8.0_131/bin/javac 1'
- `sudo update-alternatives --install /usr/bin/java java /opt/jdk1.8.0_131/bin/java 1'
- `sudo update-alternatives --config javac'
- `sudo update-alternatives --config java'
<br>
After all, verify with the commands with -verion option.<br>
- `java -version'
- `javac -version'
How to Install Nukkit<br>
- `sudo apt-get install -y git'
- `sudo apt-get install -y maven'
- `git clone https://github.com/Nukkit/Nukkit.git'
- `cd Nukkit'
- `git submodule update --init'
- `mvn clean'
- `mvn package'
To start Nukkit go to target and find the nukkit jar file. You can also create a shell script that can start it.<br>
- `cd Nukkit/target'>
- `java -jar nukkit-1.0-SNAPSHOT.jar'

Running
-------------
Simply run `start.sh` or `start.cmd`, or execute `java -jar Nukkit.jar`.

Plugin API
-------------
#### **Example Plugin**
Example Plugin which shows the API of Nukkit.

* __[Example Plugin](http://github.com/Nukkit/ExamplePlugin)__

Development Tools
-----------------
There're some tools for Nukkit developers.

* __[FDevTools](https://github.com/fengberd/FDevTools)__ (**Load source and pack them easily**)
* __[PocketServer](https://github.com/fengberd/MinecraftPEServer)__ (**Run Nukkit on android devices**)

Discussion
-------------
* __[Forums](https://forums.nukkit.io)__
* __[百度 Nukkit 吧](http://tieba.baidu.com/f?kw=nukkit)__
