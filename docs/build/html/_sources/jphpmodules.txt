===========
PHPModules
===========

あらすじ
-------------

このモジュールを目指してのインストールといくつかの一般的なと役立つサポート Php モジュールを包みます。いくつかの例は： php5 gd イメージ ライブラリ、php5 imagick イメージ libs、php5 カール リモート ファイル処理 libs、php5 mysql の mysql 接続を処理するためのライブラリ。今後のテーマでのインストールのプロセスはこのモジュールを使用する方法を見てみましょう。

ヘルプ コマンド
----------------------

Help コマンドと同様、目的に関するユーザー ガイドとして Php モジュールとして含まれているオプションについて。それは Php モジュールの代替パラメーターが一覧表示されます。また、Php モジュールをインストールするための構文について説明します。Php モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash
	
		ptconfigure PHPModules help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、Php モジュールの下に、help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************



インストール
--------------

ユーザーのコンピューターで php モジュールをインストールするために使用するコマンドを次に示します。

.. code-block:: bash

		ptconfigure phpmods install

上記のコマンドを入力した後、次のプロセスが発生します表形式で表示されます。


.. cssclass:: table-bordered

 +------------------------+-----------------------------------------------+---------------+------------------------------------------------+
 | パラメーター           | 代替パラメーター                              | オプション    | コメント                                       |
 +========================+===============================================+===============+================================================+
 |Install PHP Modules?    | の代わりに phpmods, 我々は使用することがで    | Y(Yes)        | ユーザーは、Yと入力することができ、            |
 |(Y/N)                   | きますPHPModules, php-mods, php-modules,      |               | インストールプロセスを続行したい場合           |
 |                        | phpmodules.                                   |               |                                                |
 +------------------------+-----------------------------------------------+---------------+------------------------------------------------+
 |Install PHP Modules?    | の代わりに phpmods, 我々は使用することがで    | N(No)         | ユーザーは、Nと入力することができ、            |
 |(Y/N)                   | きますPHPModules, php-mods, php-modules,      |               | インストールプロセスを終了したい場合は         |
 |                        | phpmodules.|                                  |               |                                                |
 +------------------------+-----------------------------------------------+---------------+------------------------------------------------+


場合は、インストールを続行すると、インストールのプロセス中に記載されて、リストの下：


* 依存関係ツリーを構築します。
* 状態情報を読み込みます。
* リスト アウトは自動的にインストールされているパッケージ。
* リスト アウト、新しいパッケージをインストールしています。
* ファイルの数に関する詳細情報はアップグレード新しくインストール、削除、アップグレードされません。



次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。

.. code-block:: bash


 kevell@corp:/# ptconfigure phpmods install

 Install PHP Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 /packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists 
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 php5_invoke: Enable module apcu for cgi SAPI
 php5_invoke: Enable module apcu for cli SAPI
 rmdir: failed to remove â€˜/usr/share/doc/php-apcâ€™: Directory not empty
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  php5-apcu
 Suggested packages:
  php5-gd
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 0 to remove and 252 not upgraded.
 Need to get 75.9 kB of archives.
 After this operation, 344 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe php5-apcu amd64 4.0.2-2build1 [73.2 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe php-apc all 4.0.2-2build1 [2,762 B]
 Fetched 75.9 kB in 42s (1,783 B/s)
 Selecting previously unselected package php5-apcu.
 (Reading database ... 233423 files and directories currently installed.)
 Preparing to unpack .../php5-apcu_4.0.2-2build1_amd64.deb ...
 Unpacking php5-apcu (4.0.2-2build1) ...
 Selecting previously unselected package php-apc.
 Preparing to unpack .../php-apc_4.0.2-2build1_all.deb ...
 Unpacking php-apc (4.0.2-2build1) ...
 Setting up php5-apcu (4.0.2-2build1) ...
 Setting up php-apc (4.0.2-2build1) ...
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt executed correctly
 php5_invoke: Enable module gd for cgi SAPI
 php5_invoke: Enable module gd for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
   php5-gd
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 0 B/28.0 kB of archives.
 After this operation, 163 kB of additional disk space will be used.
 Selecting previously unselected package php5-gd.
 (Reading database ... 233448 files and directories currently installed.)
 Preparing to unpack .../php5-gd_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-gd (5.5.9+dfsg-1ubuntu4.7) ...
 Setting up php5-gd (5.5.9+dfsg-1ubuntu4.7) ...
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt executed correctly
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation: 

 The following packages have unmet dependencies:
  php5-imagick : Depends: libmagickcore3 (>= 8:6.6.0.4) but it is not installable
                Depends: libmagickwand3 (>= 8:6.6.0.4) but it is not installable
                Depends: libtiff4 but it is not installable
                Depends: php5-common (= 5.3.29-1~dotdeb.0) but 5.5.9+dfsg-1ubuntu4.7 is to be installed
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 php5_invoke: Enable module curl for cgi SAPI
 php5_invoke: Enable module curl for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php5-curl
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 0 B/27.4 kB of archives.
 After this operation, 142 kB of additional disk space will be used.
 Selecting previously unselected package php5-curl.
 (Reading database ... 233455 files and directories currently installed.)
 Preparing to unpack .../php5-curl_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-curl (5.5.9+dfsg-1ubuntu4.7) ...
 Setting up php5-curl (5.5.9+dfsg-1ubuntu4.7) ...
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 php5-mysql is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 252 not upgraded.
 [Pharaoh Logging] Package php5-mysql from the Packager Apt is already installed, so not installing.
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation: 

 The following packages have unmet dependencies:
 php5-memcache : Depends: php5-common (= 5.3.29-1~dotdeb.0) but 5.5.9+dfsg-1ubuntu4.7 is to be installed
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   php5-memcached
 0 upgraded, 0 newly installed, 0 to remove and 251 not upgraded.
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 php5_invoke: Enable module mongo for cgi SAPI
 php5_invoke: Enable module mongo for cli SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php5-mongo
 0 upgraded, 1 newly installed, 0 to remove and 252 not upgraded.
 Need to get 94.5 kB of archives.
 After this operation, 334 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe php5-mongo amd64 1.4.5-1build1 [94.5 kB]
 Fetched 94.5 kB in 45s (2,096 B/s)
 Selecting previously unselected package php5-mongo.
 (Reading database ... 233462 files and directories currently installed.)
 Preparing to unpack .../php5-mongo_1.4.5-1build1_amd64.deb ...
 Unpacking php5-mongo (1.4.5-1build1) ...
 Setting up php5-mongo (1.4.5-1build1) ...
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************


利点
------------

* ヘルプとインストールで使用されるパラメーター大文字小文字が区別されません中に他の人に比べて、追加の利点は。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* すべての頻繁に使用する php モジュールのインストールを取得する単一のプロセスの下で包まれていた。
 

