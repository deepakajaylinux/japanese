============
RubyRVM
============

あらすじ
------------

Ruby Ruby バージョン Manager(RVM)、しばしば RVM, と略記はルビー、同じデバイス上の複数のインストールを管理するために設計された unix のようなソフトウェア プラットフォームです。Ruby インタプリタ、インストールされている RubyGems、およびドキュメントを含む ruby 環境全体を分割します。Mruby を触っています、JRuby にはこれらが含まれています MacRuby、IronRuby、リニアモーターカー、Rubinius、トパーズ。それはユーザーフレンドリー Ubuntu とセント OS。.

ヘルプ コマンド
--------------------

このコマンドは目標と Ruby RVM モジュールの下に利用可能なコマンドについて機能することができます。また、Ruby RVM モジュールへのコマンドについて説明します。インストールの前にこのヘルプ コマンドは、その機能を説明を読めば。

.. code-block:: bash
        
		ptconfigure RubyRVM help

次のイメージはまた、このモジュールを明確に理解することができます。


.. code-block:: bash

 kevell@corp:/# ptconfigure RubyRVM help
 ******************************


  This command allows you to install Ruby RVM.

  RubyRVM, rubyrvm, ruby-rvm, rubyRVM

        - install
        Installs Ruby RVM
        example: ptconfigure ruby-rvm install

  Ruby is installed the recommended per-user way. To use ruby after the install
  first run "source ~/.rvm/scripts/rvm" to get access to the Ruby install for
  your user, then "rvm install 1.9.3" (to install, specify version as needed)
  then "rvm use 1.9.3" (to select your default version for the session)

 ------------------------------
 End Help
 ******************************




インストール
-----------------

それはモジュールをインストールする RubyRVM ptconfigure の下でちょうど、下記のコマンドを使用して明白なプロセス


.. code-block:: bash

	        ptconfigure RubyRVM install

コマンド キーの後に求めることができます。


Install RubyRVM?(Y/N)


.. code-block:: bash

 kevell@corp:/# ptconfigure RubyRVM install
 Install Ruby RVM? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          !Ruby RVM!!        *
 *******************************
 Enter User To Install As:
 kevell
 Enter Install User Home Dir:
 /home/kevell   
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libtinfo-dev
 The following NEW packages will be installed:
  libreadline6-dev libtinfo-dev
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 289 kB of archives.
 After this operation, 1,280 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libtinfo-dev amd64 5.9+20140118-1ubuntu1 [76.3 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libreadline6-dev amd64 6.3-4ubuntu2 [213 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main libreadline6-dev amd64 6.3-4ubuntu2 [213 kB]
 Fetched 192 kB in 2min 21s (1,358 B/s)
 Selecting previously unselected package libtinfo-dev:amd64.
 (Reading database ... 212798 files and directories currently installed.)
 Preparing to unpack .../libtinfo-dev_5.9+20140118-1ubuntu1_amd64.deb ...
 Unpacking libtinfo-dev:amd64 (5.9+20140118-1ubuntu1) ...
 Selecting previously unselected package libreadline6-dev:amd64.
 Preparing to unpack .../libreadline6-dev_6.3-4ubuntu2_amd64.deb ...
 Unpacking libreadline6-dev:amd64 (6.3-4ubuntu2) ...
 Processing triggers for install-info (5.2.0.dfsg.1-2) ...
 Setting up libtinfo-dev:amd64 (5.9+20140118-1ubuntu1) ...
 Setting up libreadline6-dev:amd64 (6.3-4ubuntu2) ...
 [Pharaoh Logging] Adding Package libreadline6-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libyaml-0-2
 The following NEW packages will be installed:
  libyaml-0-2 libyaml-dev
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 104 kB of archives.
 After this operation, 438 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libyaml-0-2 amd64 0.1.4-3ubuntu3.1 [48.1 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libyaml-dev amd64 0.1.4-3ubuntu3.1 [55.9 kB]
 Err http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libyaml-dev amd64 0.1.4-3ubuntu3.1
  Connection failed [IP: 91.189.92.200 80]
 Get:3 http://security.ubuntu.com/ubuntu/ trusty-security/main libyaml-dev amd64 0.1.4-3ubuntu3.1 [55.9 kB]
 Fetched 75.9 kB in 2min 18s (550 B/s)
 Selecting previously unselected package libyaml-0-2:amd64.
 (Reading database ... 212839 files and directories currently installed.)
 Preparing to unpack .../libyaml-0-2_0.1.4-3ubuntu3.1_amd64.deb ...
 Unpacking libyaml-0-2:amd64 (0.1.4-3ubuntu3.1) ...
 Selecting previously unselected package libyaml-dev:amd64.
 Preparing to unpack .../libyaml-dev_0.1.4-3ubuntu3.1_amd64.deb ...
 Unpacking libyaml-dev:amd64 (0.1.4-3ubuntu3.1) ...
 Setting up libyaml-0-2:amd64 (0.1.4-3ubuntu3.1) ...
 Setting up libyaml-dev:amd64 (0.1.4-3ubuntu3.1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package libyaml-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  sqlite3-doc
 The following NEW packages will be installed:
  libsqlite3-dev
 0 upgraded, 1 newly installed, 0 to remove and 17 not upgraded.
 Need to get 439 kB of archives.
 After this operation, 1,491 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libsqlite3-dev amd64 3.8.2-1ubuntu2 [439 kB]
 Fetched 439 kB in 7s (60.6 kB/s)
 Selecting previously unselected package libsqlite3-dev:amd64.
 (Reading database ... 212853 files and directories currently installed.)
 Preparing to unpack .../libsqlite3-dev_3.8.2-1ubuntu2_amd64.deb ...
 Unpacking libsqlite3-dev:amd64 (3.8.2-1ubuntu2) ...
 Setting up libsqlite3-dev:amd64 (3.8.2-1ubuntu2) ...
 [Pharaoh Logging] Adding Package libsqlite3-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  sqlite3-doc
 The following NEW packages will be installed:
  sqlite3
 0 upgraded, 1 newly installed, 0 to remove and 17 not upgraded.
 Need to get 28.9 kB of archives.
 After this operation, 165 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main sqlite3 amd64 3.8.2-1ubuntu2 [28.9 kB]
 Fetched 28.9 kB in 1s (15.4 kB/s)
 Selecting previously unselected package sqlite3.
 (Reading database ... 212862 files and directories currently installed.)
 Preparing to unpack .../sqlite3_3.8.2-1ubuntu2_amd64.deb ...
 Unpacking sqlite3 (3.8.2-1ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up sqlite3 (3.8.2-1ubuntu2) ...
 [Pharaoh Logging] Adding Package sqlite3 from the Packager Apt executed correctly
 [Pharaoh Logging] Package libxml2-dev from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libxslt1-dev
 0 upgraded, 1 newly installed, 0 to remove and 17 not upgraded.
 Need to get 407 kB of archives.
 After this operation, 2,450 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libxslt1-dev amd64 1.1.28-2build1 [407 kB]
 Fetched 407 kB in 10s (40.4 kB/s)
 Selecting previously unselected package libxslt1-dev:amd64.
 (Reading database ... 212867 files and directories currently installed.)
 Preparing to unpack .../libxslt1-dev_1.1.28-2build1_amd64.deb ...
 Unpacking libxslt1-dev:amd64 (1.1.28-2build1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Setting up libxslt1-dev:amd64 (1.1.28-2build1) ...
 [Pharaoh Logging] Adding Package libxslt1-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libbison-dev libsigsegv2 m4
 Suggested packages:
  bison-doc
 The following NEW packages will be installed:
  bison libbison-dev libsigsegv2 m4
 0 upgraded, 4 newly installed, 0 to remove and 17 not upgraded.
 Need to get 805 kB of archives.
 After this operation, 2,220 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libsigsegv2 amd64 2.10-2 [15.0 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main m4 amd64 1.4.17-2ubuntu1 [195 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main libbison-dev amd64 2:3.0.2.dfsg-2 [338 kB]
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/main bison amd64 2:3.0.2.dfsg-2 [257 kB]
 Fetched 805 kB in 16s (47.8 kB/s)
 Selecting previously unselected package libsigsegv2:amd64.
 (Reading database ... 213011 files and directories currently installed.)
 Preparing to unpack .../libsigsegv2_2.10-2_amd64.deb ...
 Unpacking libsigsegv2:amd64 (2.10-2) ...
 Selecting previously unselected package m4.
 Preparing to unpack .../m4_1.4.17-2ubuntu1_amd64.deb ...
 Unpacking m4 (1.4.17-2ubuntu1) ...
 Selecting previously unselected package libbison-dev:amd64.
 Preparing to unpack .../libbison-dev_2%3a3.0.2.dfsg-2_amd64.deb ...
 Unpacking libbison-dev:amd64 (2:3.0.2.dfsg-2) ...
 Selecting previously unselected package bison.
 Preparing to unpack .../bison_2%3a3.0.2.dfsg-2_amd64.deb ...
 Unpacking bison (2:3.0.2.dfsg-2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for install-info (5.2.0.dfsg.1-2) ...
 Setting up libsigsegv2:amd64 (2.10-2) ...
 Setting up m4 (1.4.17-2ubuntu1) ...
 Setting up libbison-dev:amd64 (2:3.0.2.dfsg-2) ...
 Setting up bison (2:3.0.2.dfsg-2) ...
 update-alternatives: using /usr/bin/bison.yacc to provide /usr/bin/yacc (yacc) in auto mode
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package bison from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libffi-dev
 0 upgraded, 1 newly installed, 0 to remove and 17 not upgraded.
 Need to get 99.8 kB of archives.
 After this operation, 323 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libffi-dev amd64 3.1~rc1+r3.0.13-12 [99.8 kB]
 Fetched 99.8 kB in 2s (43.9 kB/s)
 Selecting previously unselected package libffi-dev:amd64.
 (Reading database ... 213131 files and directories currently installed.)
 Preparing to unpack .../libffi-dev_3.1~rc1+r3.0.13-12_amd64.deb ...
 Unpacking libffi-dev:amd64 (3.1~rc1+r3.0.13-12) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for install-info (5.2.0.dfsg.1-2) ...
 Setting up libffi-dev:amd64 (3.1~rc1+r3.0.13-12) ...
 [Pharaoh Logging] Adding Package libffi-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  zlib1g-dev
 The following NEW packages will be installed:
  libmysqlclient-dev zlib1g-dev
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 1,046 kB of archives.
 After this operation, 6,048 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main zlib1g-dev amd64 1:1.2.8.dfsg-1ubuntu1 [183 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libmysqlclient-dev amd64 5.5.41-0ubuntu0.14.04.1 [862 kB]
 Fetched 1,046 kB in 28s (37.2 kB/s)
 Selecting previously unselected package zlib1g-dev:amd64.
 (Reading database ... 213164 files and directories currently installed.)
 Preparing to unpack .../zlib1g-dev_1%3a1.2.8.dfsg-1ubuntu1_amd64.deb ...
 Unpacking zlib1g-dev:amd64 (1:1.2.8.dfsg-1ubuntu1) ...
 Selecting previously unselected package libmysqlclient-dev.
 Preparing to unpack .../libmysqlclient-dev_5.5.41-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking libmysqlclient-dev (5.5.41-0ubuntu0.14.04.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up zlib1g-dev:amd64 (1:1.2.8.dfsg-1ubuntu1) ...
 Setting up libmysqlclient-dev (5.5.41-0ubuntu0.14.04.1) ...
 [Pharaoh Logging] Adding Package libmysqlclient-dev from the Packager Apt executed correctly
 [Pharaoh Logging] Package libmysql-ruby from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libgdbm-dev
 0 upgraded, 1 newly installed, 0 to remove and 17 not upgraded.
 Need to get 24.9 kB of archives.
 After this operation, 144 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgdbm-dev amd64 1.8.3-12build1 [24.9 kB]
 Fetched 24.9 kB in 1s (20.8 kB/s)
 Selecting previously unselected package libgdbm-dev.
 (Reading database ... 213260 files and directories currently installed.)
 Preparing to unpack .../libgdbm-dev_1.8.3-12build1_amd64.deb ...
 Unpacking libgdbm-dev (1.8.3-12build1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libgdbm-dev (1.8.3-12build1) ...
 [Pharaoh Logging] Adding Package libgdbm-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  ncurses-doc
 The following NEW packages will be installed:
  libncurses5-dev
 0 upgraded, 1 newly installed, 0 to remove and 17 not upgraded.
 Need to get 170 kB of archives.
 After this operation, 1,056 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libncurses5-dev amd64 5.9+20140118-1ubuntu1 [170 kB]
 Fetched 170 kB in 3s (48.0 kB/s)
 Selecting previously unselected package libncurses5-dev:amd64.
 (Reading database ... 213306 files and directories currently installed.)
 Preparing to unpack .../libncurses5-dev_5.9+20140118-1ubuntu1_amd64.deb ...
 Unpacking libncurses5-dev:amd64 (5.9+20140118-1ubuntu1) ...
 Setting up libncurses5-dev:amd64 (5.9+20140118-1ubuntu1) ...
 [Pharaoh Logging] Adding Package libncurses5-dev from the Packager Apt executed correctly
 [Pharaoh Logging] Package g++ from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   libssl-doc
 The following NEW packages will be installed:
   libssl-dev libssl-doc
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 2,038 kB of archives.
 After this operation, 7,809 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libssl-dev amd64 1.0.1f-1ubuntu2.8 [1,071 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libssl-doc all 1.0.1f-1ubuntu2.8 [967 kB]
 Fetched 2,038 kB in 58s (34.6 kB/s)
 Selecting previously unselected package libssl-dev:amd64.
 (Reading database ... 213343 files and directories currently installed.)
 Preparing to unpack .../libssl-dev_1.0.1f-1ubuntu2.8_amd64.deb ...
 Unpacking libssl-dev:amd64 (1.0.1f-1ubuntu2.8) ...
 Selecting previously unselected package libssl-doc.
 Preparing to unpack .../libssl-doc_1.0.1f-1ubuntu2.8_all.deb ...
 Unpacking libssl-doc (1.0.1f-1ubuntu2.8) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libssl-dev:amd64 (1.0.1f-1ubuntu2.8) ...
 Setting up libssl-doc (1.0.1f-1ubuntu2.8) ...
 [Pharaoh Logging] Adding Package libssl-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  automake autotools-dev
 Suggested packages:
  autoconf2.13 autoconf-archive gnu-standards autoconf-doc libtool
 The following NEW packages will be installed:
  autoconf automake autotools-dev
 0 upgraded, 3 newly installed, 0 to remove and 17 not upgraded.
 Need to get 877 kB of archives.
 After this operation, 3,653 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main autoconf all 2.69-6 [322 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main autotools-dev all 20130810.1 [44.3 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main automake all 1:1.14.1-2ubuntu1 [510 kB]
 Fetched 877 kB in 15s (57.6 kB/s)
 Selecting previously unselected package autoconf.
 (Reading database ... 214752 files and directories currently installed.)
 Preparing to unpack .../autoconf_2.69-6_all.deb ...
 Unpacking autoconf (2.69-6) ...
 Selecting previously unselected package autotools-dev.
 Preparing to unpack .../autotools-dev_20130810.1_all.deb ...
 Unpacking autotools-dev (20130810.1) ...
 Selecting previously unselected package automake.
 Preparing to unpack .../automake_1%3a1.14.1-2ubuntu1_all.deb ...
 Unpacking automake (1:1.14.1-2ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for install-info (5.2.0.dfsg.1-2) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Setting up autoconf (2.69-6) ...
 Setting up autotools-dev (20130810.1) ...
 Setting up automake (1:1.14.1-2ubuntu1) ...
 update-alternatives: using /usr/bin/automake-1.14 to provide /usr/bin/automake (automake) in auto mode
 [Pharaoh Logging] Adding Package autoconf from the Packager Apt executed correctly
 [Pharaoh Logging] Package automake from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libltdl-dev
 Suggested packages:
   libtool-doc gfortran fortran95-compiler gcj-jdk
 The following NEW packages will be installed:
  libltdl-dev libtool
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 345 kB of archives.
 After this operation, 2,400 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libltdl-dev amd64 2.4.2-1.7ubuntu1 [157 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libtool amd64 2.4.2-1.7ubuntu1 [188 kB]
 Fetched 345 kB in 10s (33.3 kB/s)
 Selecting previously unselected package libltdl-dev:amd64.
 (Reading database ... 214971 files and directories currently installed.)
 Preparing to unpack .../libltdl-dev_2.4.2-1.7ubuntu1_amd64.deb ...
 Unpacking libltdl-dev:amd64 (2.4.2-1.7ubuntu1) ...
 Selecting previously unselected package libtool.
 Preparing to unpack .../libtool_2.4.2-1.7ubuntu1_amd64.deb ...
 Unpacking libtool (2.4.2-1.7ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libltdl-dev:amd64 (2.4.2-1.7ubuntu1) ...
 Setting up libtool (2.4.2-1.7ubuntu1) ...
 [Pharaoh Logging] Adding Package libtool from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-25544965900.sh
 chmod 755 /tmp/ptconfigure-temp-script-25544965900.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-25544965900.sh Permissions
 Executing /tmp/ptconfigure-temp-script-25544965900.sh
 Temp File /tmp/ptconfigure-temp-script-25544965900.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 RubyRVM: Success
 ------------------------------
 Installer Finished
 ******************************


場合に、ユーザー入力の Y として、Rubysystem パッケージからインストールします。その他に、それは、画面を終了できます。次のスクリーン ショットを説明することができます。
それは。


.. code-block:: bash

 [Pharaoh Logging] Package libreadline6-dev from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package libyaml-dev from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package libsqlite3-dev from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package sqlite3 from the Packager Apt is already installed, so not installing

Libreadline6 開発、libyaml 開発、libsqlites3 dev これらのパッケージは自動的にインストールされます。


オプション
------------


.. cssclass:: table-bordered
 

 +-------------------------+-------------------------------------------------------+------------+----------------------------------------+
 | パラメーター            | パラメーターの代替                                    | オプション | コメント                               |
 +=========================+=======================================================+=====================================================+
 |ptconfigure RubyRVM      | 我々は使用することができますRubyRVM, rubyrvm,         | Y          | システムは、インストールプロセスを     |
 |Install                  | ruby-rvm, rubyRvm.                                    |            | 開始します                             |
 +-------------------------+-------------------------------------------------------+------------+----------------------------------------+
 |ptconfigure RubyRVM      | 我々は使用することができますRubyRVM, rubyrvm,         | N          | システムは、インストール·プロセス      |
 |Install                  | ruby-rvm, rubyRvm.                                    |            | を停止し、|                            |
 +-------------------------+-------------------------------------------------------+------------+----------------------------------------+



利点
-------------

* RVM は同時に複数のバージョンをインストールしたくない場合でも便利です。
* パッケージ マネージャーからそれを得る （少なくとも ubuntu で) からのインストール ディレクトリを変更、更新されたバージョンを与える、
  既定値です。
* ソースコードからビルド依存関係の負荷を取得し、オプションを構成する必要があります。
* RVM は素晴らしいこれにより、Ruby インストールのデフォルトをお使いのシステムに触れることがなく異なるバージョンをインストールします。
* RVM を持つもう一つの大きな利点は、gemsets - ことは、バージョンに固有のパッチ ・ レベル、できるだけ多くの gemsets を作成することができます。
  ルビー。
* Ruby のシステムは、迅速かつ簡単なオブジェクト指向プログラミング (OOP) の動的な反射、高度なスクリプト言語です。
* Ruby のシステムでは多くの便利で楽しいツールです。展開プロセスで使用されているツールを含みます。
* の平均ルビー システムは通常既に web 開発と一般に極端な知識を持つ経験豊富な専門家
  ソフトウェア エンジニア リングのスキル。
* Ruby プログラミング言語 Ruby システムの主な利点は、開発のスピードと見なされます。
* キャッシュのプロジェクト-主要なインター ネット プロジェクトの開発で最も重要な手順の 1 つ。PHP では、データのさまざまなオプションがあります。
  キャッシュ。
 

