vagrant-jantos
==============

Java Ant Node Tomcat Oracle Subversion on CentOS using [Vagrant](http://www.vagrantup.com) and headless VirtualBox
> :exclamation: This is a work in progress


## Default Add-ons:
- Subversion: latest (v1.8.9+)
- Node.js: latest (v0.10.26+)
- Java
	- JDK 6 update 45
- Tomcat
	- Tomcat 7.0.53


## Requirements
* Install VirtualBox from [virtualbox.org](https://www.virtualbox.org)
* Install Vagrant from [vagrantup.com](http://www.vagrantup.com)
* An internet connection is required to provision the box for the first time
* If JDK6 needs to be installed
	
	- Download Sun Java JDK 6 ( update 45 ) from [here](http://www.oracle.com/technetwork/java/javasebusiness/downloads/java-archive-downloads-javase6-419409.html#jdk-6u45-oth-JPR)
	- Put it in the folder `[projectroot]/tools/install/java/` (Create directories if required)


## Installation
* Check out this project:

        git clone https://github.com/abhishekdev/vagrant-jantos.git

* Install [vbguest]:

        vagrant plugin install vagrant-vbguest

* [Optional] Tweak configurations in `[projectroot]/Vagrantfile`, `[projectroot]/puppet/manifests/base.pp`

* Boot the machine from project root.
		
		vagrant up


## TODO:
- [x] Host Vagrant box on a file Server
- [x] Add SVN Support
- [x] Add Node Support
- [x] Add Java Support
- [x] Add Tomcat Support
- [ ] Add Ant Support
- [ ] Add Oracle Support