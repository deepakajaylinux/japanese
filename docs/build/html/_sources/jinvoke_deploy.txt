=========
Invoke
=========

概要
----------

呼び出しベースのマシンから仮想マシンを特定の SSH ファイルをフェッチします。コンピューティングでは、SSH ファイル転送プロトコルもセキュリティで保護されたファイル転送プロトコル (SFTP) は任意の信頼性の高いデータ ストリーム上のファイルへのアクセス、ファイル転送、ファイル管理機能を提供するネットワーク プロトコルです。

Helpコマンド
--------------

このコマンドでの使用状況を確認できますモジュールを呼び出します。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash

	ptdeploy invoke help

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptdeploy invoke help 

 ****************************** 


  This command is part of Core and handles SSH Connection Functions. 

  Invoke, invoke, inv 

        - cli 
        Will ask you for details for servers, then open a shell for you to execute on multiple servers 
        example: ptdeploy invoke cli --environment-name=staging 

        - script 
        Will ask you for details for servers, then execute each line of a provided script file on the remote/s 
        example: ptdeploy invoke script --ssh-script="/var/www/project/script.sh" --environment-name=staging 

        - data 
        Execute php variable data on one or more remotes 
        example: ptdeploy invoke data --ssh-data="ls -lah" --environment-name=staging 

 ------------------------------ 
 End Help 
 ****************************** 


Cli
------

ユーザーは、cli を使用してクライアント システムにサーバーからデータをフェッチする必要がある場合、以下のコマンドはすべての情報取得、シェルを開くとき

.. code-block:: bash

	ptdeploy Invoke cli

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptdeploy Invoke cli

 Invoke SSH Shell on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 2
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.14
 Please Enter SSH User
 karthik
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SSH connections...
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful.
 Last login: Thu Mar 19 19:09:01 2015 from 192.168.1.29
 echo "Pharaoh Remote SSH on ...192.168.1.14"
 Pharaoh Remote SSH on ...192.168.1.14
 Opening CLI...
 Enter command to be executed on remote servers? Enter none to close connection and end program
 ls
 [192.168.1.14] Executing ls...
 ls
 build			       Music
 comp.tar.gz		       nagios-4.0.8
 deon			       nagios-4.0.8.tar.gz
 Desktop			       nagios-plugins-2.0.3
 Documents		       nagios-plugins-2.0.3.tar.gz
 Downloads		       openstackgeek
 error			       papyrusfile
 error~			       Pictures
 examples.desktop	       Public
 fil			       selenium-server-standalone-2.44.0.jar
 file			       Templates
 http			       test
 kibana-4.0.1-linux-x64	       Untitled Document 2
 kibana-4.0.1-linux-x64.tar.gz  Videos
 kkkk
 [192.168.1.14] ls Completed...
 Enter command to be executed on remote servers? Enter none to close connection and end program
 mkdir nithin
 [192.168.1.14] Executing mkdir nithin...
 mkdir nithin
 [192.168.1.14] mkdir nithin Completed...
 Enter command to be executed on remote servers? Enter none to close connection and end program
 
 Shell Completed******************************

 Shell Result: Success
 Invoke Shell Cli

 ------------------------------
 Installer Finished
 ******************************

	 
script
-----------

ユーザーはスクリプトを使用してクライアント システムにサーバーからデータをフェッチする必要がある場合、以下のコマンドは、リモートで提供されているスクリプト ファイルの各行を実行

.. code-block:: bash

        ptdeploy Invoke script

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptdeploy Invoke script

 Invoke SSH Script on Server group? (Y/N) 
 y
 Enter Location of bash script to execute
 /opt/script
 Please Enter SSH Timeout in seconds
 5
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.14
 Please Enter SSH User
 karthik
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SSH connections...
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful.
 Last login: Thu Mar 19 19:35:38 2015 from 192.168.1.29
 echo "Pharaoh Remote SSH on ...192.168.1.14"
 Pharaoh Remote SSH on ...192.168.1.14
 [192.168.1.14] Executing ls...
 ls
 build			       Music
 comp.tar.gz		       nagios-4.0.8
 deon			       nagios-4.0.8.tar.gz
 Desktop			       nagios-plugins-2.0.3
 Documents		       nagios-plugins-2.0.3.tar.gz
 Downloads		       nithin
 error			       openstackgeek
 error~			       papyrusfile
 examples.desktop	       Pictures
 fil			       Public
 file			       selenium-server-standalone-2.44.0.jar
 http			       Templates
 kibana-4.0.1-linux-x64	       test
 kibana-4.0.1-linux-x64.tar.gz  Untitled Document 2
 kkkk			       Videos
 [192.168.1.14] ls Completed...
 [192.168.1.14] Executing ...
  [192.168.1.14]  Completed...
 Script by SSH Completed******************************

 Shell Result: Success
 Invoke Script

 ------------------------------
 Installer Finished
 ******************************


Data
---------

ユーザー データを使用してクライアント システムにサーバーからデータをフェッチする必要がある場合、1 つまたは複数のリモコン上で php 変数以下のコマンドを実行します。

.. code-block:: bash

        ptdeploy Invoke data

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptdeploy Invoke data

 Invoke SSH Data on Server group? (Y/N) 
 y
 Enter data to execute via SSH
 ls -la
 Please Enter SSH Timeout in seconds
 4
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.14
 Please Enter SSH User
 karthik
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SSH connections...
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful.
 Last login: Thu Mar 19 19:20:11 2015 from 192.168.1.29
 echo "Pharaoh Remote SSH on ...192.168.1.14"
 Pharaoh Remote SSH on ...192.168.1.14
 [192.168.1.14] Executing ls -la...
 ls -la
 total 55112
 drwxr-xr-x 31 karthik karthik     4096 Mar 19 19:16 .
 drwxr-xr-x  4 root    root        4096 Feb 24 11:52 ..
 drwx------  3 karthik karthik     4096 Feb 24 18:23 .adobe
 -rw-------  1 karthik karthik    12029 Mar 19 19:20 .bash_history
 -rw-rw-r--  1 karthik karthik       25 Mar 19 19:21 .bash_login
 -rw-r--r--  1 karthik karthik      220 Feb 24 05:16 .bash_logout
 -rw-r--r--  1 karthik karthik     3637 Feb 24 05:16 .bashrc
 drwxr-xr-x  3 root    root        4096 Mar 18 17:18 build
 drwx------ 25 karthik karthik     4096 Mar 17 00:38 .cache
 drwx------  3 karthik karthik     4096 Feb 24 01:34 .compiz
 -rw-r--r--  1 karthik karthik  2836036 Feb 26 21:22 comp.tar.gz
 drwx------ 26 karthik karthik     4096 Mar 19 14:26 .config
 drwx------  3 root    root        4096 Feb 24 11:21 .dbus
 -rw-r--r--  1 root    root           0 Mar 19 14:58 deon
 drwxr-xr-x  5 karthik karthik     4096 Mar 19 19:05 Desktop
 -rw-r--r--  1 karthik karthik       25 Feb 24 05:22 .dmrc
 drwxr-xr-x  2 karthik karthik     4096 Mar 10 10:47 Documents
 drwxr-xr-x  3 karthik karthik     4096 Mar 19 19:02 Downloads
 -rw-rw-r--  1 karthik karthik    48711 Mar 18 19:46 error
 -rw-rw-r--  1 karthik karthik    48464 Mar 18 19:45 error~
 -rw-r--r--  1 karthik karthik     8980 Feb 24 05:16 examples.desktop
 drwxr-xr-x  2 root    root        4096 Mar 18 18:24 fil
 -rwxr-xr-x  1 root    root         395 Mar 18 18:23 file
 drwx------  3 karthik karthik     4096 Mar 19 10:18 .gconf
 -rw-r--r--  1 root    root          61 Mar  3 14:29 .gitconfig
 -rw-r--r--  1 root    root           0 Mar 19 14:59 http
 -rw-------  1 karthik karthik    11270 Mar 19 10:18 .ICEauthority
 drwxr-xr-x  7     501 staff       4096 Mar  4 21:42 kibana-4.0.1-linux-x64
 -rw-r--r--  1 root    root    13625479 Mar  4 21:42 kibana-4.0.1-linux-x64.tar.gz
 drwxrwxr-x  2 karthik karthik     4096 Mar 18 15:24 kkkk
 drwxr-xr-x  3 karthik karthik     4096 Feb 24 05:22 .local
 drwx------  3 karthik karthik     4096 Feb 24 18:23 .macromedia
 drwx------  4 karthik karthik     4096 Feb 24 00:51 .mozilla
 drwxr-xr-x  2 karthik karthik     4096 Feb 24 05:22 Music
 drwxrwxr-x 18 root    root        4096 Feb 24 11:57 nagios-4.0.8
 -rw-r--r--  1 root    root     1805059 Aug 12  2014 nagios-4.0.8.tar.gz
 drwxr-xr-x 15 root    root        4096 Feb 24 12:03 nagios-plugins-2.0.3
 -rw-r--r--  1 root    root     2659772 Jun 26  2014 nagios-plugins-2.0.3.tar.gz
 drwxrwxr-x  2 karthik karthik     4096 Mar 19 19:16 nithin
 drwxr-xr-x  7 root    root        4096 Feb 27 11:00 openstackgeek
 -rw-r--r--  1 root    root         458 Mar 18 19:29 papyrusfile
 drwxr-xr-x  2 karthik karthik     4096 Mar 19 12:08 Pictures
 -rw-r--r--  1 karthik karthik      675 Feb 24 05:16 .profile
 drwxr-xr-x  2 karthik karthik     4096 Feb 24 05:22 Public
 -rw-------  1 root    root        1024 Mar 12 17:46 .rnd
 -rw-r--r--  1 karthik karthik 35169724 Feb 27 10:49 selenium-server-standalone-2.44.0.jar
 drwx------  2 karthik karthik     4096 Mar 12 18:51 .ssh
 drwxr-xr-x  2 karthik karthik     4096 Feb 24 05:22 Templates
 drwxrwxr-x  2 karthik karthik     4096 Mar 18 15:25 test
 drwx------  4 karthik karthik     4096 Feb 26 04:48 .thunderbird
 -rw-rw-r--  1 karthik karthik      619 Mar  4 05:45 Untitled Document 2
 drwxr-xr-x  2 karthik karthik     4096 Mar 18 11:41 Videos
 drwxr-xr-x  2 root    root        4096 Mar 18 12:20 .vim
 -rw-------  1 root    root        9238 Mar 19 14:26 .viminfo
 -rw-------  1 karthik karthik       52 Mar 19 10:18 .Xauthority
 -rw-------  1 karthik karthik      820 Mar 19 11:26 .xsession-errors
 -rw-------  1 karthik karthik     1353 Mar 18 20:38 .xsession-errors.old
 [192.168.1.14] ls -la Completed...
 Data by SSH Completed
 ******************************
 
 Invoke SSH Data Result: Success
 
 ------------------------------
 Installer Finished
 ******************************



代替パラメータ
-------------------------

2 つの代替パラメーターをコマンドラインで使用することができますがあります。

Invoke, invoke, inv


メリット
-------------

* このコマンドによってフェッチ SSH ファイルまたはディレクトリに 
* ソースから 1 つのコマンドを使用して宛先にファイルまたはディレクトリをフェッチ



