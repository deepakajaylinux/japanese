===============
ApacheModules
===============

あらすじ
--------

このモジュールは Apache モジュールをインストールする容易にします。それはあなたの環境の構成を指定します。モジュールのチェック可用性が可能です。それはセント OS のようにも Ubuntu で快適です。

ヘルプ コマンド
------------

このヘルプ コマンドは、特定のモジュールの目的について説明します。インストールの構文ヘルプ コマンドの下で描かれています。また、宣言に使用できる代替のパラメーターを一覧表示されます。Help コマンドは、エンドユーザーが動作するように簡単です。次のコマンドはこのモジュールの使用についてユーザーをガイドします。

.. code-block:: bash

	 cleopatra apache modules help

コマンドを与えた後、コマンドはヘルプ オプションをリストアップします。次のスクリーン ショットは、このモジュールの使用のための視覚効果を与えます。

.. code-block:: bash

 kevell@corp:/# cleopatra ApacheModules help
 ******************************


  This command is part of Core and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  ApacheModules, apachemods, apache-modules, apachemodules

        - install
        Installs common apache Modules
        example: cleopatra apache-modules install

 ------------------------------
 End Help
 ******************************

インストール
------------

インストールは、モジュールをインストールするこのクレオパトラの下、下記コマンドを使用するだけで困難なプロセスではありません。


.. code-block:: bash

	Install apache-modules install

それを聞いてきます、コマンドを与えた後

.. code-block:: bash

	Install Apache module? (Y/N)

'Y' と入力を与えると、モジュールが正常にインストールされます。
場合として入力を与える ' ñ '、インストール出てくるし、。

次のスクリーン ショットは、このモジュールのインストールの視覚効果を与えます。

.. code-block:: bash

 kevell@corp:/#  cleopatra apache-modules install
 Install Apache Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Mods!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libxml2-dev
 0 upgraded, 1 newly installed, 0 to remove and 229 not upgraded.
 Need to get 630 kB of archives.
 After this operation, 2,928 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libxml2-dev amd64 2.9.1+dfsg1-3ubuntu4.4 [630 kB]
 Fetched 630 kB in 2min 38s (3,990 B/s)
 Selecting previously unselected package libxml2-dev:amd64.
 (Reading database ... 181481 files and directories currently installed.)
 Preparing to unpack .../libxml2-dev_2.9.1+dfsg1-3ubuntu4.4_amd64.deb ...
 Unpacking libxml2-dev:amd64 (2.9.1+dfsg1-3ubuntu4.4) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up libxml2-dev:amd64 (2.9.1+dfsg1-3ubuntu4.4) ...
 [Pharaoh Logging] Adding Package libxml2-dev from the Packager Apt executed correctly
 Creating /tmp/cleopatra-temp-script-11435369770.sh
 chmod 755 /tmp/cleopatra-temp-script-11435369770.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-11435369770.sh Permissions
 Executing /tmp/cleopatra-temp-script-11435369770.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-11435369770.sh Removed
 Creating /tmp/cleopatra-temp-script-95277456152.sh
 chmod 755 /tmp/cleopatra-temp-script-95277456152.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-95277456152.sh Permissions
 Executing /tmp/cleopatra-temp-script-95277456152.sh
 Considering dependency filter for deflate:
 Module filter already enabled
 Module deflate already enabled
 Temp File /tmp/cleopatra-temp-script-95277456152.sh Removed
 Creating /tmp/cleopatra-temp-script-1351048337.sh
 chmod 755 /tmp/cleopatra-temp-script-1351048337.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-1351048337.sh Permissions
 Executing /tmp/cleopatra-temp-script-1351048337.sh
 Considering dependency setenvif for ssl:
 Module setenvif already enabled
 Considering dependency mime for ssl:
 Module mime already enabled
 Considering dependency socache_shmcb for ssl:
 Enabling module socache_shmcb.
 Enabling module ssl.
 See /usr/share/doc/apache2/README.Debian.gz on how to configure SSL and create self-signed certificates.
 To activate the new configuration, you need to run:
   service apache2 restart
 Temp File /tmp/cleopatra-temp-script-1351048337.sh Removed
 [Pharaoh Logging] Package libapache2-mod-php5 from the Packager Apt is already installed, so not installing
 Creating /tmp/cleopatra-temp-script-89813944614.sh
 chmod 755 /tmp/cleopatra-temp-script-89813944614.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-89813944614.sh Permissions
 Executing /tmp/cleopatra-temp-script-89813944614.sh
 Module php5 already enabled
 Temp File /tmp/cleopatra-temp-script-89813944614.sh Removed
 [Pharaoh Logging] Restarting apache2 service
 Output of config test was:
 apache2: Syntax error on line 214 of /etc/apache2/apache2.conf: Could not open configuration file /etc/apache2/httpd.conf: No such file or 
 directory 
 Action 'configtest' failed.
 The Apache error log may have more information.
 * Restarting web server apache2
   ...fail!
 * The apache2 configtest failed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 ApacheModules: Success
 ------------------------------
 Installer Finished
 ****************************** 


.. cssclass:: table-bordered



利点
--------

* モジュールは、クレオパトラとリンクへの援助です。
* インストール中に Apache モジュール、それは構成ファイルが黙認されます。
* 構成ファイルが、システムで利用可能なない場合このモジュールは自動的にインストールされます。

