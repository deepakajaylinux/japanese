==============
StandardTools
==============

あらすじ
----------------

このモジュールは、システムで標準的なツールをインストールするのに役立ちます。それは vim のようなすべてのツールをインストールすることができますなど、郵便番号します。自動化が可能です。それはあなたの環境の標準化を指定します。それはユーザーフレンドリー Ubuntu とセント OS。

ヘルプ コマンド
---------------------

Help コマンドは、指定されたコマンドに関する情報を見つけるために使用します。標準のツールについての詳細。我々 はこのヘルプ コマンドを使用することができます。


.. code-block:: bash

		ptconfigure StandardTools help

次のスクリーン ショットは、あなたをご案内いたします。


.. code-block:: bash

 kevell@corp:/# ptconfigure StandardTools help
 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  StandardTools, standard-tools, standardtools, stdtools, std-tools

        - install
        Installs some standard tools
        example: ptconfigure stdtools install

 ------------------------------
 End Help
 ******************************


インストール
------------------

会社として、そして個人として、標準的なツールの要件を満たすと、彼らのビジネス目標を満たすユーザーの課題を満たすために専用されています。それはモジュールをインストールする標準的なツール ptconfigure の下でちょうど、下記のコマンドを使用して明白なプロセス


.. code-block:: bash

                ptconfigure stdtools install


コマンドを入力した後


Install standard tools? (Y/N)


場合は、ユーザーとして y 値

すべて、更新された標準的なツールをインストールします。

場合は、ユーザーとして N 値

それは、画面を終了します

スクリーン ショットに示します。



.. code-block:: bash


 kevell@corp:/# ptconfigure stdtools install
 Install Standard Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Std. Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 curl is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package curl from the Packager Apt is already installed, so not installing.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 vim is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package vim from the Packager Apt is already installed, so not installing.

 Creating config file /etc/php5/mods-available/mysql.ini with new version
 php5_invoke: Enable module mysql for cli SAPI
 php5_invoke: Enable module mysql for fpm SAPI
 php5_invoke: Enable module mysql for apache2 SAPI

 Creating config file /etc/php5/mods-available/mysqli.ini with new version
 php5_invoke: Enable module mysqli for cli SAPI
 php5_invoke: Enable module mysqli for fpm SAPI
 php5_invoke: Enable module mysqli for apache2 SAPI
 
 Creating config file /etc/php5/mods-available/pdo_mysql.ini with new version
 php5_invoke: Enable module pdo_mysql for cli SAPI
 php5_invoke: Enable module pdo_mysql for fpm SAPI
 php5_invoke: Enable module pdo_mysql for apache2 SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   php-console-table php5-mysql
 Suggested packages:
   drupal7
 Recommended packages:
  php-console-color
 The following NEW packages will be installed:
  drush php-console-table php5-mysql
 0 upgraded, 3 newly installed, 0 to remove and 13 not upgraded.
 Need to get 430 kB of archives.
 After this operation, 1,800 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main php5-mysql amd64 5.5.9痻1ubuntu4.5 [62.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php-console-table all 1.1.6-1 [14.7 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe drush all 5.10.0-2 [353 kB]
 Fetched 430 kB in 1min 4s (6,634 B/s)
 Selecting previously unselected package php5-mysql.
 (Reading database ... 212663 files and directories currently installed.)
 Preparing to unpack .../php5-mysql_5.5.9痻1ubuntu4.5_amd64.deb ...
 Unpacking php5-mysql (5.5.9痻1ubuntu4.5) ...
 Selecting previously unselected package php-console-table.
 Preparing to unpack .../php-console-table_1.1.6-1_all.deb ...
 Unpacking php-console-table (1.1.6-1) ...
 Selecting previously unselected package drush.
 Preparing to unpack .../drush_5.10.0-2_all.deb ...
 Unpacking drush (5.10.0-2) ...
 Processing triggers for libapache2-mod-php5 (5.5.9痻1ubuntu4.5) ...
 Processing triggers for php5-fpm (5.5.9痻1ubuntu4.5) ...
 php5-fpm stop/waiting
 php5-fpm start/running, process 5110
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up php5-mysql (5.5.9痻1ubuntu4.5) ...
 Setting up php-console-table (1.1.6-1) ...
 Setting up drush (5.10.0-2) ...
 Processing triggers for libapache2-mod-php5 (5.5.9痻1ubuntu4.5) ...
 Processing triggers for php5-fpm (5.5.9痻1ubuntu4.5) ...
 php5-fpm stop/waiting
 php5-fpm start/running, process 6189
 [Pharaoh Logging] Adding Package drush from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 zip is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package zip from the Packager Apt is already installed, so not installing.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 StandardTools: Success
 ------------------------------
 Installer Finished
 ******************************



代替パラメーター
----------------------------------

代替パラメーターを次に示します。StandardTools、stdtools、std ツール、standardtools、標準的なツールです。


利点
-------------

* 利用可能なインストールの更新されたバージョンです。
* の場合、既存のそれを上書きすることができます。
* 非大文字小文字を区別


 

