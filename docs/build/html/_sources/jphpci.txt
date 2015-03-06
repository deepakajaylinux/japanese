===============
Phpci
===============

あらすじ
--------------

PHPCI は、ptconfigure に適したオープン ソース継続的な統合ツールです。ユーザーが念頭に置いてシンプルに構築してので、セットアップして使用する微風であるジェンキンスを行うことができますすべてはしない、しながら。これは Ubuntu とセントと使いやすさです OS。

ヘルプ コマンド
-----------------------

このコマンドのヘルプガイド Phpci モジュールに関する特定の操作を実行するユーザー。これは、企業のユーザーのすべてのタイプに適しています。

.. code-block:: bash
   
                ptconfigure PHPCI help

ヘルプ コマンド Phpci モジュールに組み込まれたコマンドの短いリストが表示されます。次のスクリーン ショットはそれを視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCI help
 ******************************


  This command allows you to install PHPCI, the popular Build Server.

  PHPCI, phpci

        - install
        Installs PHPCI through git, with its dependencies
        example: ptconfigure phpci install

        - config-default, default-config
        Installs a default config.yml file for PHPCI
        example: ptconfigure phpci config-default --yes --guess

        - install-default-database
        Installs a default database and user for PHPCI
        example: ptconfigure phpci install-default-database --yes --guess
            --mysql-admin-user="root" # guess will provide root
            --mysql-admin-pass="some-pass" # guess will provide ptconfigure

  You can install a complete local version of PHPCI with the following:

  sudo ptconfigure phpci install --yes --guess
  sudo ptconfigure phpci install-default-database --yes --guess
  sudo ptconfigure phpci config-default --yes --guess

 ------------------------------
 End Help
 ******************************


インストール
-----------------

このモジュールは phpci をインストールするのに役立ちます。このモジュールは作曲家を点検しなければならない最初のステップは、システムかどうか。それがない場合、システムで自動的に、それをインストールします。


.. code-block:: bash

                   ptconfigure Phpci install



上記のコマンドを入力した後、次のプロセス関与しているインストールのプロセス中に表形式で示されています。

.. cssclass:: table-bordered

 +---------------------+-------------------------------------------+------------+-------------------------------------------------------+
 | パラメーター        | 代替パラメーター                          | オプション | コメント                                              |
 +=====================+===========================================+============+=======================================================+
 |Install PHPCI? (Y/N) | その代わりPHPCIの、我々はまた、phpci      | Y(Yes)     | ユーザーは、Yと入力することができ、インストールプ     |
 |                     | 使用することができます                    |            | ロセスを続行したい場合                                |
 +---------------------+-------------------------------------------+------------+-------------------------------------------------------+
 |Install PHPCI? (Y/N) | その代わりPHPCIの、我々はまた、phpci      | N(No)      | ユーザーは、Nと入力することができ、インストールプ     |
 |                     | 使用することができます                    |            | ロセスを終了したい場合は|                             |
 +---------------------+-------------------------------------------+------------+-------------------------------------------------------+


場合はインストールを続行すると、インストールの処理中に、次の手順、

* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リスト アウト、余分なパッケージを自動的にインストールされます。
* リスト アウトは、インストールする提案のパッケージ。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。



表形式で表した、ユーザーからの入力が要求されます。



.. cssclass:: table-bordered

 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 | パラメーター       | パス                     | オプション            | コメント                                                       |
 +====================+==========================+=======================+================================================================+
 |Program data        | “/opt/phpunit(対応す     | Yes                   | ユーザーがデフォルトのプログラムのデータディレクトリを使用     |
 |directory (Default) | るモジュール)”           |                       | してインストールを続行する場合、それらはYESと入力をするこ      |
 |                    |                          |                       | とができます                                                   |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 |Program data        | User Specific            | No(エンドスラッシュ)  | ユーザーが自分自身のプログラムデータディレクトリを続行したい   |
 |directory           |                          |                       | 場合は、入力Nとして、そして手に、彼らは場所を所有指定するこ    |
 |                    |                          |                       | とができます。                                                 |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 |Program executor    | “/usr/bin”               | Yes                   | ユーザーがデフォルトのプログラム実行ディレクトリを使用         |
 |directory (Default) |                          |                       | してインストールを続行する場合、それらはYESと入力をすることが  |
 |                    |                          |                       | できます                                                       |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+
 |Program executor    | User specific            | No(エンドスラッシュ)  | ユーザーが独自のプログラム実行ディレクトリを続行したい場合は、 |
 |directory           |                          |                       | 入力Nとして、そして手に、彼らは場所を所有指定すること          |
 |                    |                          |                       | ができます。|                                                  |
 +--------------------+--------------------------+-----------------------+----------------------------------------------------------------+



次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。


.. code-block:: bash

 kevell@corp:/#  ptconfigure phpci install
 Install PHPCI? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libmcrypt4
 Suggested packages:
  libmcrypt-dev mcrypt
 The following NEW packages will be installed:
  libmcrypt4 php5-mcrypt
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 77.3 kB of archives.
 After this operation, 324 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmcrypt4 amd64 2.5.8-3.1ubuntu1 [61.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php5-mcrypt amd64 5.4.6-0ubuntu5 [15.4 kB]
 Fetched 77.3 kB in 4s (19.1 kB/s)
 Selecting previously unselected package libmcrypt4.
 (Reading database ... 182037 files and directories currently installed.)
 Preparing to unpack .../libmcrypt4_2.5.8-3.1ubuntu1_amd64.deb ...
 Unpacking libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Selecting previously unselected package php5-mcrypt.
 Preparing to unpack .../php5-mcrypt_5.4.6-0ubuntu5_amd64.deb ...
 Unpacking php5-mcrypt (5.4.6-0ubuntu5) ...
 Setting up libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Setting up php5-mcrypt (5.4.6-0ubuntu5) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package php5-mcrypt from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-82480901916.sh
 chmod 755 /tmp/ptconfigure-temp-script-82480901916.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-82480901916.sh Permissions
 Executing /tmp/ptconfigure-temp-script-82480901916.sh
 Temp File /tmp/ptconfigure-temp-script-82480901916.sh Removed
 Creating /tmp/ptconfigure-temp-script-43828918328.sh
 chmod 755 /tmp/ptconfigure-temp-script-43828918328.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-43828918328.sh Permissions
 Executing /tmp/ptconfigure-temp-script-43828918328.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-43828918328.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: composer: not found
 [Pharaoh Logging] Module Composer reports itself as Not Installed
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...


 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 Creating /tmp/ptconfigure-temp-script-34508236330.sh
 chmod 755 /tmp/ptconfigure-temp-script-34508236330.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-34508236330.sh Permissions
 Executing /tmp/ptconfigure-temp-script-34508236330.sh
 #!/usr/bin/env php
 Installing block8/phpci (1.5.2)
  - Installing block8/phpci (1.5.2)
    Downloading: 100%

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
 Warning: The lock file is not up to date with the latest changes in composer.json. You may be getting outdated dependencies. Run update to update them.
 Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - The requested PHP extension ext-pdo_mysql * is missing from your system.

 Temp File /tmp/ptconfigure-temp-script-34508236330.sh Removed
 Creating /tmp/ptconfigure-temp-script-28990655696.sh
 chmod 755 /tmp/ptconfigure-temp-script-28990655696.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-28990655696.sh Permissions
 Executing /tmp/ptconfigure-temp-script-28990655696.sh
 sudo: dapperstrano: command not found
 Temp File /tmp/ptconfigure-temp-script-28990655696.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCI: Success
 ------------------------------
 Installer Finished
 ******************************


利点
--------

* PHPCI の構成とデータベース ファイルをインストールするために使用します。一方、既存の任意のファイルがある場合、インストール内容を上書きします。
* 新しいバージョンを自動的に更新することができます。
* それはユーザーのデータベース インストール願いごとを受け入れることができます。
* 継続的な統合が可能です。
* 複数の環境
* PDO、mysql、sqlite のような別の亜種と php の構築、debug... など。
* 自動フィーチャ検知。
 

