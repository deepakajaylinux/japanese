=========
Tomcat
=========


概要
------------------

TomcatはPHPを実行し、PHPのコーディングを含むWebページをレンダリングするptconfigureからアプリケーションサーバです。 Tomcatは、開発の結果であり、バイナリとソースの両方のバージョンでは、PHPのWebサイトから入手できます。 Tomcatは、自身の内部Webサーバーまたは一緒に他のWebサーバとのスタンドアロン製品のいずれかとして使用することができる。 TomcatはUbuntuとセントのOSをサポートしています。

Helpコマンド
------------------------

このコマンドは、目的とTomcatモジュールの下で利用可能なコマンドについて、機能することができます。また、Tomcatをインストールするコマンドを説明します。インストールを開始する前に、ユーザーがこのhelpコマンドをお読みください。

.. code-block:: bash 

	ptconfigure tomcat help 

以下のスクリーンショットは、その機能を説明して


.. code-block:: bash 

 kevell@corp:/# ptconfigure Tomcat help 

 ****************************** 


  This command allows you to update tomcat. 

  Tomcat, tomcat, tom-cat 

        - install 
        Installs the latest version of awstats 
        example: ptconfigure tomcat install 

 ------------------------------ 
 End Help 
 ****************************** 

インストール
------------------

PHPからUbuntu Linuxのシステム上でTomcatをインストールするには、このモジュールを使用します。 Ubuntuは独自のTomcatを含むが、公式のTomcatサーバは、一般に、より最新である。

.. code-block:: bash 

	ptconfigure tomcat install 

Install tomcat?(Y/N) 

はい自動的にデフォルトですべてdepenciesをインストールし、また更新されたバージョンをインストールするようにユーザーが入力を与えたとき。次のスクリーンショットは、それを説明します。


.. code-block:: bash 

 kevell@corp:/# ptconfigure Tomcat install 
 Install Tomcat? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Tomcat!        * 
 ******************************* 
 
 Creating config file /etc/default/tomcat7 with new version 
 Adding system user `tomcat7' (UID 117) ... 
 Adding new user `tomcat7' (UID 117) with group `tomcat7' ... 
 Not creating home directory `/usr/share/tomcat7'. 
 Creating config file /etc/logrotate.d/tomcat7 with new version 
 * Starting Tomcat servlet engine tomcat7                                                                                               [ OK ] 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following extra packages will be installed: 
  authbind libcommons-collections3-java libcommons-dbcp-java 
  libcommons-pool-java libecj-java libgeronimo-jta-1.1-spec-java 
  libservlet3.0-java libtomcat7-java tomcat7-common 
 Suggested packages: 
  libcommons-collections3-java-doc libcommons-dbcp-java-doc ecj ant 
  libecj-java-gcj libgeronimo-jta-java-doc tomcat7-docs tomcat7-admin 
  tomcat7-examples tomcat7-user libtcnative-1 
 The following NEW packages will be installed: 
  authbind libcommons-collections3-java libcommons-dbcp-java 
  libcommons-pool-java libecj-java libgeronimo-jta-1.1-spec-java 
  libservlet3.0-java libtomcat7-java tomcat7 tomcat7-common 
 0 upgraded, 10 newly installed, 0 to remove and 15 not upgraded. 
 Need to get 6,266 kB of archives. 
 After this operation, 8,097 kB of additional disk space will be used. 
 Get:1 http://us.archive.ubuntu.com/ubuntu/ trusty/main libcommons-collections3-java all 3.2.1-6 [602 kB] 
 Get:2 http://us.archive.ubuntu.com/ubuntu/ trusty/main libcommons-pool-java all 1.6-2 [105 kB] 
 Get:3 http://us.archive.ubuntu.com/ubuntu/ trusty/main libcommons-dbcp-java all 1.4-3ubuntu1 [149 kB] 
 Get:4 http://us.archive.ubuntu.com/ubuntu/ trusty/main libecj-java all 3.9.0-1 [1,352 kB] 
 Get:5 http://us.archive.ubuntu.com/ubuntu/ trusty/main libgeronimo-jta-1.1-spec-java all 1.1.1-3ubuntu1 [12.4 kB] 
 Get:6 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main libservlet3.0-java all 7.0.52-1ubuntu0.1 [293 kB] 
 Get:7 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main libtomcat7-java all 7.0.52-1ubuntu0.1 [3,649 kB] 
 Get:8 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main tomcat7-common all 7.0.52-1ubuntu0.1 [47.9 kB] 
 Get:9 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main tomcat7 all 7.0.52-1ubuntu0.1 [35.6 kB] 
 Get:10 http://us.archive.ubuntu.com/ubuntu/ trusty/main authbind amd64 2.1.1 [19.6 kB] 
 Preconfiguring packages ... 
 Fetched 6,266 kB in 8min 28s (12.3 kB/s) 
 Selecting previously unselected package libcommons-collections3-java. 
 (Reading database ... 199303 files and directories currently installed.) 
 Preparing to unpack .../libcommons-collections3-java_3.2.1-6_all.deb ... 
 Unpacking libcommons-collections3-java (3.2.1-6) ... 
 Selecting previously unselected package libcommons-pool-java. 
 Preparing to unpack .../libcommons-pool-java_1.6-2_all.deb ... 
 Unpacking libcommons-pool-java (1.6-2) ... 
 Selecting previously unselected package libcommons-dbcp-java. 
 Preparing to unpack .../libcommons-dbcp-java_1.4-3ubuntu1_all.deb ... 
 Unpacking libcommons-dbcp-java (1.4-3ubuntu1) ... 
 Selecting previously unselected package libecj-java. 
 Preparing to unpack .../libecj-java_3.9.0-1_all.deb ... 
 Unpacking libecj-java (3.9.0-1) ... 
 Selecting previously unselected package libgeronimo-jta-1.1-spec-java. 
 Preparing to unpack .../libgeronimo-jta-1.1-spec-java_1.1.1-3ubuntu1_all.deb ... 
 Unpacking libgeronimo-jta-1.1-spec-java (1.1.1-3ubuntu1) ... 
 Selecting previously unselected package libservlet3.0-java. 
 Preparing to unpack .../libservlet3.0-java_7.0.52-1ubuntu0.1_all.deb ... 
 Unpacking libservlet3.0-java (7.0.52-1ubuntu0.1) ... 
 Selecting previously unselected package libtomcat7-java. 
 Preparing to unpack .../libtomcat7-java_7.0.52-1ubuntu0.1_all.deb ... 
 Unpacking libtomcat7-java (7.0.52-1ubuntu0.1) ... 
 Selecting previously unselected package tomcat7-common. 
 Preparing to unpack .../tomcat7-common_7.0.52-1ubuntu0.1_all.deb ... 
 Unpacking tomcat7-common (7.0.52-1ubuntu0.1) ... 
 Selecting previously unselected package tomcat7. 
 Preparing to unpack .../tomcat7_7.0.52-1ubuntu0.1_all.deb ... 
 Unpacking tomcat7 (7.0.52-1ubuntu0.1) ... 
 Selecting previously unselected package authbind. 
 Preparing to unpack .../authbind_2.1.1_amd64.deb ... 
 Unpacking authbind (2.1.1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 ureadahead will be reprofiled on next reboot 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up libcommons-collections3-java (3.2.1-6) ... 
 Setting up libcommons-pool-java (1.6-2) ... 
 Setting up libcommons-dbcp-java (1.4-3ubuntu1) ... 
 Setting up libecj-java (3.9.0-1) ... 
 Setting up libgeronimo-jta-1.1-spec-java (1.1.1-3ubuntu1) ... 
 Setting up libservlet3.0-java (7.0.52-1ubuntu0.1) ... 
 Setting up libtomcat7-java (7.0.52-1ubuntu0.1) ... 
 Setting up tomcat7-common (7.0.52-1ubuntu0.1) ... 
 Setting up tomcat7 (7.0.52-1ubuntu0.1) ... 
 Setting up authbind (2.1.1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 [Pharaoh Logging] Adding Package tomcat7 from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Tomcat: Success 
 ------------------------------ 
 Installer Finished 

 ****************************** 


オプション
-------------

.. cssclass:: table-bordered 

 +---------------------------+-----------------------------------+---------------+---------------------------------------------------+
 | パラメータ                | 代替パラメータ                    | オプション    | コメント                                          |
 +===========================+===================================+===============+===================================================+
 |Install tomcat (Y/N)       | tomcat, Tomcat, tom-cat           | Y             | それはptconfigure下にTomcatをインストールします   |
 +---------------------------+-----------------------------------+---------------+---------------------------------------------------+
 |Install tomcat (Y/N)       | tomcat, Tomcat, tom-cat           | N             | システム出口インストール|                         |
 +---------------------------+-----------------------------------+---------------+---------------------------------------------------+



メリット
----------------

* などのPHP、Pythonの、のようなものを実行するためのモジュールとのかなり拡張可能
* これは、UbuntuとセントのOSに快適さ。
* 非大文字と小文字の区別がハイライトされた利点がある。
* Tomcatは論理処理の大部分が起こるアプリケーション層である。
* 最後に、そのTomcatの協議は、データベース層があるでしょう。

