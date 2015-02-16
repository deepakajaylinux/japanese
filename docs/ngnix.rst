=============
NginxServer
=============



Synopsis
---------

Nginx, pronounced “Engine X”, is a high-performance Web server. The Nginx Web Server is a light weight and versatile server that can be configured for all the different tasks that many modern websites demand. Ngnix server acts as a facilitator to the users in configuring applications settings. Few examples for applications settings includes mysql admin user, host, pass. Nginx is making headlines as the new Web server of choice for many webmasters. The top reason for its popularity is its speed. Nginx is faster than Apache in non-testing environments because its architecture is event driven while Apache’s is process driven. The Cleopatra modules acts as a way through for installing this Nginx Server.

Help Command
------------

The help command leads the users regarding the purpose and as well as about the options that are included in the Ngnix server module. The help command lists out the alternative parameters of Ngnix server. It also describes the syntax for installing Ngnix server. The help command for Ngnix server is given below.

.. code-block:: bash

	cleopatra nginx-server help

The syntax for declaring the help command is not case sensitive which is an added advantage. The following screenshot visualize you about the help command under Nginx Server.

.. code-block:: bash


	kevells@corp:/# cleopatra NginxServer help
	******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

	NginxServer, nginx-server, nginxserver

        - install
        Installs Nginx HTTP Server
        example: cleopatra nginx-server install

	------------------------------
	End Help
	******************************


Installation
------------

Installing the Nginx server is simpler by using the following command as shown:

.. code-block:: bash

	cleopatra nginx-server install

After inputting the command above the following operations as shown in the tabular format occurs.

.. cssclass:: table-bordered

  +---------------------------------+-------------------------------+---------------+----------------------------------------------------+
  |   Paramaters 		    | Alternative Parameter         | Options	    |	comments			                 |
  +=================================+===============================+===============+====================================================+
  |Install PHP Code Sniffer ? (Y/N) |In Spite of Nginx Server, the  |		    |If the user wish to proceed the installation process|
  |				    |following alternatives can also|  Y(yes)       |they can input as Y.			    	 |
  |				    |be used: NginxServer, 	    |		    |							 |
  |				    |nginx-server, nginxserver.     |		    | 							 |
  +---------------------------------+-------------------------------+---------------+----------------------------------------------------+
  |Install PHP Code Sniffer ? (Y/N) |In Spite of Nginx Server, the  |		    |If the user wish to Quit the installation process   |
  |				    |following alternatives can also|  Y(yes)       |they can input as N.|			    	 |
  |				    |be used: NginxServer, 	    |		    |							 |
  |				    |nginx-server, nginxserver.     |		    || 							 |
  +---------------------------------+-------------------------------+---------------+----------------------------------------------------+

If the user proceeds the installation process, the Nginx HTTP Server will be installed. If the package of Nginx is already exists in the users machine, then a message will appear to instruct the user as Nginx is already exists in that machine. Finally reports are generated with clear results and status. The following screen shot explains the above mentioned process pictorially.

.. code-block:: bash
	

	Kevells@corp:/# cleopatra nginx-server install
	
	Install Nginx Server? (Y/N) 
	y	
	*******************************
	*        Pharaoh Tools        *
	*         Nginx Server!       *
	*******************************
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
	nginx-common nginx-core
	Suggested packages:
	fcgiwrap nginx-doc
	The following NEW packages will be installed:
	nginx nginx-common nginx-core
	0 upgraded, 3 newly installed, 0 to remove and 278 not upgraded.
	Need to get 347 kB of archives.
	After this operation, 1,295 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-common all 1.4.6-1ubuntu3.1 [17.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-core amd64 1.4.6-1ubuntu3.1 [324 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx all 1.4.6-1ubuntu3.1 [5,218 B]
	Fetched 347 kB in 3s (104 kB/s)
	Selecting previously unselected package nginx-common.
	(Reading database ... 168194 files and directories currently installed.)
	Preparing to unpack .../nginx-common_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx-common (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx-core.
	Preparing to unpack .../nginx-core_1.4.6-1ubuntu3.1_amd64.deb ...
	Unpacking nginx-core (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx.
	Preparing to unpack .../nginx_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	ureadahead will be reprofiled on next reboot
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Setting up nginx-common (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Setting up nginx-core (1.4.6-1ubuntu3.1) ...
	Setting up nginx (1.4.6-1ubuntu3.1) ...
	[Pharaoh Logging] Adding Package nginx from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	NginxServer: Success
	------------------------------
	Installer Finished
	******************************

Benefits
----------

* By using this Nginx Server the user can configure their application settings.
* The parameters used in help and installation operations are not case sensitive which is an added advantage while compared to others.
* Nginx is fast because it does not need to create a new process for each new request.
* Nginx uses very little memory, especially for static Web pages.
* Nginx can be used with a range of systems.
* Nginx is highly scalable, and performance is not dependent on hardware.
* Nginx is easy to install and configure.
* Like Apache, Nginx has all the features you would expect from a leading Web server:
* Static file serving.
* SSL/TLS support.
* Virtual hosts.
* Reverse proxying.
* Load balancing.
* Compression.
* Access controls.
* URL rewriting.
* Custom logging.
* Server-side includes.
* WebDAV.
* FLV streaming.
* FastCGI.
