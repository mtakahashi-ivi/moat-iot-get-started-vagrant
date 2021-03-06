MOAT IoT Example Application Building Environment Setup
===

This configuration allows you to create application development environment on your local machine with [VirtualBox](https://www.virtualbox.org/) and [Vagrant](http://www.vagrantup.com/) so that you can try [MOAT IoT example apps](https://github.com/inventit/moat-iot-get-started) shortly.

The environment is built on the VirtualBox image and never affects your current working environment.

You are now free from performing a bunch of downloading and installation tasks for setup.

## Get Started

At first, please read this [page](http://docs.vagrantup.com/v1/docs/getting-started/index.html) and install  [Vagrant](http://www.vagrantup.com/) along with [VirtualBox](https://www.virtualbox.org/).

After installing Vagrant and VirtualBox, then checkout this project:

### Git

    $ git clone git://github.com/inventit/moat-iot-get-started-vagrant.git

### Wget/Browser

    $ wget https://github.com/inventit/moat-iot-get-started-vagrant/archive/master.zip

Finally, enter the command on the terminal to setup (on the checkout root directory):

    moat-iot-get-started-vagrant:$ vagrant up

NOTE that this would take at least 20 minutes or more depending on the network state at first time.
After the first trial, it would take 5 or more.

In order to set up the example applications, let's go to the [tutorial](http://dev.yourinventit.com/guides/get-started).

## Heads Up!

This tool does NOT perform;
> Building [MOAT IoT example apps](https://github.com/inventit/moat-iot-get-started) but checking out

Again, please follow the [instruction](http://dev.yourinventit.com/guides/get-started) for building.

## Installed Modules

These scripts install the following modules:

* `apt-get` Installation
 * [`openjdk-6-jdk`, Java Development Kit 6](http://openjdk.java.net/)
 * [`git`, Git](http://git-scm.com/)
 * [`build-essential`, Package building libraries](https://launchpad.net/ubuntu/precise/+package/build-essential)
 * [`libsqlite3-dev`, Used by Rails](https://launchpad.net/ubuntu/precise/+package/libsqlite3-dev)
 * [`ruby1.9.3`, Ruby 1.9.3](http://www.ruby-lang.org/en/)
 * [`ruby-bundler`, RubyGems management tool](http://gembundler.com/)
* Binary Installation
 * [Apache Maven 3, Java Building Tool](http://maven.apache.org/download.cgi)
 * [Android SDK r21.0.1 and Platform libraries(API Level 16)](http://developer.android.com/sdk/index.html)
* Source Installation
 * [Node.js v0.8.19](http://nodejs.org/)
 * [`nvm`, Node Version Manager](https://github.com/creationix/nvm)
 * [`npm`, Node Package Manager](https://npmjs.org/)
* `npm` Installation
 * [`moat`, MOAT js unit testing library](https://github.com/inventit/moatjs-stub)
 * [`sinon`, Mock/Stub testing library](http://sinonjs.org/)
 * [`nodeunit`, Unite testing library](https://github.com/caolan/nodeunit)

and

* [`iidn` Command Line Interface Tool](https://github.com/inventit/iidn-cli)
* [Getting Started Example Project](https://github.com/inventit/moat-iot-get-started)

## Misc

1. You can choose 64bit based Ubuntu 12.04 but it takes longer time to `vagrant up` because of more libraries are required than 32bit Ubuntu in Android SDK installation

## Source Code License

All program source codes are available under the MIT style License.

The use of IIDN service requires [our term of service](http://dev.yourinventit.com/legal/term-of-service).

Copyright (c) 2013 Inventit Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Change History

1.0.6 : February 19, 2013

* Fixes an issue where creating a project directory is skipped because of duplicate recipe resource name

1.0.5 : February 15, 2013

* Adds a new recipe to install node-v0.8.19

1.0.4 : February 13, 2013

* Fixes an issue where port forwarding settings is missing

1.0.3 : February 13, 2013

* Fixes issues where re-launching a created image fails on errors

1.0.2 : February 13, 2013

* Adds environment variables used in the [instruction](http://dev.yourinventit.com/guides/get-started) to .bashrc

1.0.1 : February 12, 2013

* Fixes an issue where android API level 16 is not installed

1.0.0 : February 12, 2013

* Initial Release.
