==============
Citadel
==============

Synopsis
-------------

Citadel is a complete and feature-rich open source groupware platform. The Citadel system is extremely versatile. It provides numerous front ends to present to users, such as a text-based interface, an AJAX-style web interface, and many popular PIM clients using SMTP/POP/IMAP. All of these can be used simultaneously.

It is also extremely scalable. Not only can a well-equipped Citadel server support a large number of concurrent users, but you can also build a distributed network of Citadel nodes that share rooms and their content.

Help Command
----------------------

This command helps to determine the usage of Citadel module. The user will come to know about the different ways/format to execute this module. This command guides the end user to know the purpose of this command. Below given are the command and the screenshot of the same. 

.. code-block:: bash
      	
		Cleapatra  Citadel help
                


Installation
----------------

When the user needs to install Citadel server in machine, you can issue the following commands to install the citadel-suite. The system will execute the process of installation.

.. code-block:: bash
        
	        Cleapatra Citadel  install

Options
-----------                               

.. cssclass:: table-bordered

 +-----------------------------+------------------------------------------+----------+--------------------------------------+
 |	Parameters   	       | Alternative Parameter                    | Options  | 		Comments	            |
 +=============================+==========================================+==========+======================================+
 |Cleopatra Citadel Install    |Either of the three alternative   	  |Y         |Once the user provides the option,    |
 |               	       |parameter can be used in command- Citadel,| 	     |System starts installation process    |
 |                             |citadel-server,  citadel		  |          |				            |
 |                             |eg: Cleopatra  citadel-server Install     |          |				            |
 +-----------------------------+------------------------------------------+----------+--------------------------------------+
 |Cleopatra Citadel Install    |Either of the three alternative		  |N         |Once the user provides the option,    |
 |		 	       |parameter can be used in command- Citadel,| 	     |System stops installation process     |
 |                             |citadel-server,  citadel	   	  |          |				            |
 |                             |eg: Cleopatra  citadel-server Install|    |          |				            |
 +-----------------------------+------------------------------------------+----------+--------------------------------------+




Configuration
--------------------

This command helps in configuring the Citadel server. Once the below given command is executed the system provides you with the default value for each section, if there are any changes to be done, the user can provide the data. 

.. code-block:: bash
         
	        Cleapatra Citadel configure

Benefits
--------------

* Email, calendaring/scheduling, address books 
* Bulletin boards, mailing list server, instant messaging 
* Multiple domain support 
* An intuitive, attractive AJAX-style web interface 
