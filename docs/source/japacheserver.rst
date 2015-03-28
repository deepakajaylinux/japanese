==============
ApacheServer
==============

あらすじ
-----------

このモジュールを目指して Apache サーバーをインストールします。すべての要求なしインストール中 apache サーバの現在のバージョンに自動的にインストールされます。

ヘルプ コマンド
-----------------

Help コマンドは、目的とこのモジュールで使用できるコマンドについて説明します。また、特定のモジュールをインストールするコマンドについて説明します。

.. code-block:: bash

 		ptconfigure ApacheServer help


スクリーン ショットは、下図のように、このモジュールの下に help コマンドの使用状況を視覚的に表します。


.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  ApacheServer, apache-server, apacheserver

        - install
        Installs Apache HTTP Server
        example: ptconfigure apacheserver install

 ------------------------------
 End Help
 ******************************


インストール
---------------

それは、単に以下のコマンドを使用してptconfigureの下で、この特定のツールをインストールする方が簡単です、


.. code-block:: bash

		ptconfigure ApacheServer install

上記のコマンドを与えた後、ツールは確認します。

Install Apache Server? (Y/N)

Y として入力を与える場合、モジュールが正常にインストールします。

インストールでスクリーン ショット下記手順やコマンドについて視覚的に説明する必要があります。

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer install
 Install Apache Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
   php5-cli php5-readline
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  apache2-doc apache2-suexec-pristine apache2-suexec-custom apache2-utils
 The following NEW packages will be installed:
  apache2
 0 upgraded, 1 newly installed, 0 to remove and 39 not upgraded.
 Need to get 0 B/87.4 kB of archives.
 After this operation, 473 kB of additional disk space will be used.
 Selecting previously unselected package apache2.
 (Reading database ... 193457 files and directories currently installed.)
 Preparing to unpack .../apache2_2.4.7-1ubuntu4.4_amd64.deb ...
 Unpacking apache2 (2.4.7-1ubuntu4.4) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up apache2 (2.4.7-1ubuntu4.4) ...
 Enabling module mpm_event.
 Enabling module authz_core.
 Enabling module authz_host.
 Enabling module authn_core.
 Enabling module auth_basic.
 Enabling module access_compat.
 Enabling module authn_file.
 Enabling module authz_user.
 Enabling module alias.
 Enabling module dir.
 Enabling module autoindex.
 Enabling module env.
 Enabling module mime.
 Enabling module negotiation.
 Enabling module setenvif.
 Enabling module filter.
 Enabling module deflate.
 Enabling module status.
 Enabling conf charset.
 Enabling conf localized-error-pages.
 Enabling conf other-vhosts-access-log.
 Enabling conf security.
 Enabling conf serve-cgi-bin.
 Enabling site 000-default.
 * Starting web server apache2
 * 
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 [Pharaoh Logging] Adding Package apache2 from the Packager Apt executed correctly
 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ApacheServer: Success
 ------------------------------
 Installer Finished
 ******************************



オプション
------------

.. cssclass:: table-bordered

 +-----------------------+--------------------------------------------+---------------+-------------------------------------------+
 | パラメーター          | 代替パラメーター                           | 必要な        | コメント                                  |
 +=======================+============================================+===============+===========================================+
 |Install Apache         | の代わりに ApacheServer, Instead of        | Yes           | ユーザーとしてイエス入力を与えた場合は、  |
 |Server? (Y/N)          | ApacheServer, 我々は使用することができます |               | インストールを続行します                  | 
 |                       | apache-server, apacheserver また.          |               |                                           |
 +-----------------------+--------------------------------------------+---------------+-------------------------------------------+
 |Install Apache         | の代わりに ApacheServer, Instead of        | No            | ユーザーには、入力を与えない場合は、      |
 |Server? (Y/N)          | ApacheServer, 我々は使用することができます |               | インストールプロセスを終了します          |
 |                       | apache-server, apacheserver また.|         |               |                                           |
 +-----------------------+--------------------------------------------+---------------+-------------------------------------------+



バージョン
------------

ツールの処理中は最も最近の更新バージョンを自動的にグラブはおよびインストールの準備ができて得るためにそれを作る。


エンドユーザーへの利点
---------------------------

* このモジュールは apache サーバーをインストールすることができます。サーバーのインストール中にユーザーの作業が簡単になりますその
  apache サーバの現在のバージョンを自動的にチェックします。
* それは裕福なセント OS とも Ubuntu のように。
* 宣言で使用されるパラメーターは大文字と小文字を区別する加えられた利点であります。
