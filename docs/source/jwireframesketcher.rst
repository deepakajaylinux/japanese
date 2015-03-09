====================
Wireframe sketcher
====================

あらすじ
-------------

Wireframing は、任意の画面のデザイン プロセスで重要なステップです。主に、容易にあなたのユーザー情報を処理する方法に応じてレイアウトを計画するため、設計の情報の階層を定義することができます。

デザイナーのレイアウトと色、書体の選択またはさらにコピー気を取らされることがなくインターフェイスの相互作用を計画することができますので、Wireframing は重要です。ユーザーは、黒と白のワイヤ フレームに行く場所を把握できない場合、問題ではない最終的に使用する色はどのような私のクライアントに説明したいです。ボタンは、光沢のあるまたは鮮やかな色ではない場合でも明らかな必要があります。

ヘルプ コマンド
----------------------

このコマンドは、Wireframing のためのワイヤ フレーム スケッチャーをインストールすることができます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。


.. code-block:: bash
        
		ptconfigure wireframe-sketcher help


 Kevell@Corp:/# ptconfigure WireframeSketcher help

 ******************************

  This command allows you to install Wireframe Sketcher, for Wireframing

  WireframeSketcher, wireframe-sketcher, wireframesketcher

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure wireframe-sketcher install

 ------------------------------
 End Help
 ******************************


インストール
----------------

とき、ユーザーはマシンでワイヤ フレーム スケッチャーをインストールする必要があります。以下に、コマンドと、インストール プロセスのスクリーン ショット。


.. code-block:: bash
        
	        ptconfigure wireframe-sketcher install


 kevell@corp:/: ptconfigure wireframe-sketcher install
 PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open 
 shared object file: No such file or directory in Unknown on line 0
 Install Wireframe Sketcher? (Y/N) 
 y 
 *******************************
 *        Pharaoh Tools        *
 *         Wireframe Sketcher        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-6527022738.sh
 chmod 755 /tmp/ptconfigure-temp-script-6527022738.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-6527022738.sh Permissions
 Executing /tmp/ptconfigure-temp-script-6527022738.sh
 Cloning into 'wireframe-sketcher'...
 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 dpkg: dependency problems prevent configuration of wireframesketcherstudio:
 wireframesketcherstudio depends on default-jre | java5-runtime | java6-runtime; however:
  Package default-jre is not installed.
  Package java5-runtime is not installed.
  Package java6-runtime is not installed.
 wireframesketcherstudio depends on libwebkitgtk-1.0-0 | libwebkit-1.0-2; however:
  Package libwebkitgtk-1.0-0 is not installed.
  Package libwebkit-1.0-2 is not installed.

 dpkg: error processing package wireframesketcherstudio (--install):
 dependency problems - leaving unconfigured
 Errors were encountered while processing:
 wireframesketcherstudio
 Selecting previously unselected package wireframesketcherstudio.
 (Reading database ... 211803 files and directories currently installed.)
 Preparing to unpack .../WireframeSketcher-4.3.1_amd64.deb ...
 Unpacking wireframesketcherstudio (4.3.1-1) ...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Correcting dependencies... Done
 The following packages were automatically installed and are no longer required:
  libaio1 libframework2-zend-server libicu36 libmcrypt4 liboci-us-locales-zend
  libsqlite0 libssl0.9.8 lighttpd-zend-server php-5.3-bcmath-zend-server
  php-5.3-bz2-zend-server php-5.3-calendar-zend-server
  php-5.3-ctype-zend-server php-5.3-curl-zend-server php-5.3-exif-zend-server
  php-5.3-fcgi-zend-server php-5.3-fileinfo-zend-server
  php-5.3-ftp-zend-server php-5.3-gettext-zend-server php-5.3-imap-zend-server
  php-5.3-intl-zend-server php-5.3-ldap-zend-server php-5.3-loader-zend-server
  php-5.3-mbstring-zend-server php-5.3-mcrypt-zend-server
  php-5.3-oci8-zend-server php-5.3-pdo-mysql-zend-server
  php-5.3-pdo-pgsql-zend-server php-5.3-pgsql-zend-server
  php-5.3-phar-zend-server php-5.3-posix-zend-server php-5.3-soap-zend-server
  php-5.3-sockets-zend-server php-5.3-sqlite-zend-server
  php-5.3-tidy-zend-server php-5.3-tokenizer-zend-server
  php-5.3-xsl-zend-server php-5.3-zip-zend-server sqlite sqlite3
  ttf-dejavu-core zend-server-doc
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
  default-jre fonts-dejavu-extra libatk-wrapper-java libatk-wrapper-java-jni
  libbonobo2-0 libbonobo2-common libgconf2-4 libgif4 libgnome2-0 libgnome2-bin
  libgnome2-common libgnomevfs2-0 libgnomevfs2-common libidl-common libidl0
  libjavascriptcoregtk-1.0-0 liborbit-2-0 liborbit2 libwebkitgtk-1.0-0
  libwebkitgtk-1.0-common openjdk-7-jre
 Suggested packages:
  libbonobo2-bin desktop-base libgnomevfs2-bin libgnomevfs2-extra
  gnome-mime-data icedtea-7-plugin
 The following NEW packages will be installed:
  default-jre fonts-dejavu-extra libatk-wrapper-java libatk-wrapper-java-jni
  libbonobo2-0 libbonobo2-common libgconf2-4 libgif4 libgnome2-0 libgnome2-bin
  libgnome2-common libgnomevfs2-0 libgnomevfs2-common libidl-common libidl0
  libjavascriptcoregtk-1.0-0 liborbit-2-0 liborbit2 libwebkitgtk-1.0-0
  libwebkitgtk-1.0-common openjdk-7-jre
 0 upgraded, 21 newly installed, 0 to remove and 11 not upgraded.
 1 not fully installed or removed.
 Need to get 11.9 MB of archives.
 After this operation, 53.1 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgif4 amd64 4.1.6-11 [28.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libatk-wrapper-java all 0.30.4-4 [30.2 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main libatk-wrapper-java-jni amd64 0.30.4-4 [25.2 kB]
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main openjdk-7-jre amd64 7u71-2.5.3-0ubuntu0.14.04.1 [171 kB]
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/main default-jre amd64 2:1.7-51 [940 B]
 Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libjavascriptcoregtk-1.0-0 amd64 2.4.7-1~ubuntu1 [1,820 kB]
 Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libwebkitgtk-1.0-common all 2.4.7-1~ubuntu1 [107 kB]
 Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libwebkitgtk-1.0-0 amd64 2.4.7-1~ubuntu1 [7,229 kB]
 Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/main libbonobo2-common all 2.32.1-0ubuntu5 [34.2 kB]
 Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/main libidl-common all 0.8.14-0.2ubuntu4 [8,196 B]
 Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty/main libidl0 amd64 0.8.14-0.2ubuntu4 [65.9 kB]
 Get:12 http://in.archive.ubuntu.com/ubuntu/ trusty/main liborbit-2-0 amd64 1:2.14.19-0.3 [138 kB]
 Get:13 http://in.archive.ubuntu.com/ubuntu/ trusty/main liborbit2 amd64 1:2.14.19-0.3 [14.7 kB]
 Get:14 http://in.archive.ubuntu.com/ubuntu/ trusty/main libbonobo2-0 amd64 2.32.1-0ubuntu5 [214 kB]
 Get:15 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgnomevfs2-common amd64 1:2.24.4-1ubuntu6 [22.8 kB]
 Get:16 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgnomevfs2-0 amd64 1:2.24.4-1ubuntu6 [210 kB]
 Get:17 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgnome2-common all 2.32.1-4ubuntu1 [33.3 kB]
 Get:18 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgnome2-bin amd64 2.32.1-4ubuntu1 [15.0 kB]
 Get:19 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgnome2-0 amd64 2.32.1-4ubuntu1 [43.2 kB]
 Get:20 http://in.archive.ubuntu.com/ubuntu/ trusty/main fonts-dejavu-extra all 2.34-1ubuntu1 [1,736 kB]
 Get:21 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgconf2-4 amd64 3.2.6-0ubuntu2 [2,042 B]
 Fetched 11.9 MB in 6min 51s (29.1 kB/s)
 Selecting previously unselected package libgif4:amd64.
 (Reading database ... 212686 files and directories currently installed.)
 Preparing to unpack .../libgif4_4.1.6-11_amd64.deb ...
 Unpacking libgif4:amd64 (4.1.6-11) ...
 Selecting previously unselected package libatk-wrapper-java.
 Preparing to unpack .../libatk-wrapper-java_0.30.4-4_all.deb ...
 Unpacking libatk-wrapper-java (0.30.4-4) ...
 Selecting previously unselected package libatk-wrapper-java-jni:amd64.
 Preparing to unpack .../libatk-wrapper-java-jni_0.30.4-4_amd64.deb ...
 Unpacking libatk-wrapper-java-jni:amd64 (0.30.4-4) ...
 Selecting previously unselected package openjdk-7-jre:amd64.
 Preparing to unpack .../openjdk-7-jre_7u71-2.5.3-0ubuntu0.14.04.1_amd64.deb ...
 Unpacking openjdk-7-jre:amd64 (7u71-2.5.3-0ubuntu0.14.04.1) ...
 Selecting previously unselected package default-jre.
 Preparing to unpack .../default-jre_2%3a1.7-51_amd64.deb ...
 Unpacking default-jre (2:1.7-51) ...
 Selecting previously unselected package libjavascriptcoregtk-1.0-0:amd64.
 Preparing to unpack .../libjavascriptcoregtk-1.0-0_2.4.7-1~ubuntu1_amd64.deb ...
 Unpacking libjavascriptcoregtk-1.0-0:amd64 (2.4.7-1~ubuntu1) ...
 Selecting previously unselected package libwebkitgtk-1.0-common.
 Preparing to unpack .../libwebkitgtk-1.0-common_2.4.7-1~ubuntu1_all.deb ...
 Unpacking libwebkitgtk-1.0-common (2.4.7-1~ubuntu1) ...
 Selecting previously unselected package libwebkitgtk-1.0-0:amd64.
 Preparing to unpack .../libwebkitgtk-1.0-0_2.4.7-1~ubuntu1_amd64.deb ...
 Unpacking libwebkitgtk-1.0-0:amd64 (2.4.7-1~ubuntu1) ...
 Selecting previously unselected package libbonobo2-common.
 Preparing to unpack .../libbonobo2-common_2.32.1-0ubuntu5_all.deb ...
 Unpacking libbonobo2-common (2.32.1-0ubuntu5) ...
 Selecting previously unselected package libidl-common.
 Preparing to unpack .../libidl-common_0.8.14-0.2ubuntu4_all.deb ...
 Unpacking libidl-common (0.8.14-0.2ubuntu4) ...
 Selecting previously unselected package libidl0:amd64.
 Preparing to unpack .../libidl0_0.8.14-0.2ubuntu4_amd64.deb ...
 Unpacking libidl0:amd64 (0.8.14-0.2ubuntu4) ...
 Selecting previously unselected package liborbit-2-0:amd64.
 Preparing to unpack .../liborbit-2-0_1%3a2.14.19-0.3_amd64.deb ...
 Unpacking liborbit-2-0:amd64 (1:2.14.19-0.3) ...
 Selecting previously unselected package liborbit2:amd64.
 Preparing to unpack .../liborbit2_1%3a2.14.19-0.3_amd64.deb ...
 Unpacking liborbit2:amd64 (1:2.14.19-0.3) ...
 Selecting previously unselected package libbonobo2-0:amd64.
 Preparing to unpack .../libbonobo2-0_2.32.1-0ubuntu5_amd64.deb ...
 Unpacking libbonobo2-0:amd64 (2.32.1-0ubuntu5) ...
 Selecting previously unselected package libgnomevfs2-common.
 Preparing to unpack .../libgnomevfs2-common_1%3a2.24.4-1ubuntu6_amd64.deb ...
 Unpacking libgnomevfs2-common (1:2.24.4-1ubuntu6) ...
 Selecting previously unselected package libgnomevfs2-0:amd64.
 Preparing to unpack .../libgnomevfs2-0_1%3a2.24.4-1ubuntu6_amd64.deb ...
 Unpacking libgnomevfs2-0:amd64 (1:2.24.4-1ubuntu6) ...
 Selecting previously unselected package libgnome2-common.
 Preparing to unpack .../libgnome2-common_2.32.1-4ubuntu1_all.deb ...
 Unpacking libgnome2-common (2.32.1-4ubuntu1) ...
 Selecting previously unselected package libgnome2-bin.
 Preparing to unpack .../libgnome2-bin_2.32.1-4ubuntu1_amd64.deb ...
 Unpacking libgnome2-bin (2.32.1-4ubuntu1) ...
 Selecting previously unselected package libgnome2-0:amd64.
 Preparing to unpack .../libgnome2-0_2.32.1-4ubuntu1_amd64.deb ...
 Unpacking libgnome2-0:amd64 (2.32.1-4ubuntu1) ...
 Selecting previously unselected package fonts-dejavu-extra.
 Preparing to unpack .../fonts-dejavu-extra_2.34-1ubuntu1_all.deb ...
 Unpacking fonts-dejavu-extra (2.34-1ubuntu1) ...
 Selecting previously unselected package libgconf2-4:amd64.
 Preparing to unpack .../libgconf2-4_3.2.6-0ubuntu2_amd64.deb ...
 Unpacking libgconf2-4:amd64 (3.2.6-0ubuntu2) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for gconf2 (3.2.6-0ubuntu2) ...
 Processing triggers for fontconfig (2.11.0-0ubuntu4.1) ...
 Setting up libgif4:amd64 (4.1.6-11) ...
 Setting up libjavascriptcoregtk-1.0-0:amd64 (2.4.7-1~ubuntu1) ...
 Setting up libwebkitgtk-1.0-common (2.4.7-1~ubuntu1) ...
 Setting up libwebkitgtk-1.0-0:amd64 (2.4.7-1~ubuntu1) ...
 Setting up libbonobo2-common (2.32.1-0ubuntu5) ...
 Setting up libidl-common (0.8.14-0.2ubuntu4) ...
 Setting up libidl0:amd64 (0.8.14-0.2ubuntu4) ...
 Setting up liborbit-2-0:amd64 (1:2.14.19-0.3) ...
 Setting up liborbit2:amd64 (1:2.14.19-0.3) ...
 Setting up libbonobo2-0:amd64 (2.32.1-0ubuntu5) ...
 Setting up libgnomevfs2-common (1:2.24.4-1ubuntu6) ...
 Setting up libgnomevfs2-0:amd64 (1:2.24.4-1ubuntu6) ...
 Setting up libgnome2-common (2.32.1-4ubuntu1) ...
 Setting up fonts-dejavu-extra (2.34-1ubuntu1) ...
 Setting up libgconf2-4:amd64 (3.2.6-0ubuntu2) ...
 Setting up default-jre (2:1.7-51) ...
 Setting up wireframesketcherstudio (4.3.1-1) ...
 Setting up libatk-wrapper-java (0.30.4-4) ...
 Setting up libatk-wrapper-java-jni:amd64 (0.30.4-4) ...
 Setting up openjdk-7-jre:amd64 (7u71-2.5.3-0ubuntu0.14.04.1) ...
 update-alternatives: using /usr/lib/jvm/java-7-openjdk-amd64/jre/bin/policytool to provide /usr/bin/policytool (policytool) in auto mode
 Setting up libgnome2-bin (2.32.1-4ubuntu1) ...
 Setting up libgnome2-0:amd64 (2.32.1-4ubuntu1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 Temp File /tmp/ptconfigure-temp-script-6527022738.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 WireframeSketcher: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
------------
                               


.. cssclass:: table-bordered


 +-------------------------------+--------------------------------------------------+-------------+------------------------------------+
 | パラメーター                  | 代替パラメーター                                 | オプション  | コメント                           |
 +===============================+==================================================+=============+====================================+
 |ptconfigure WireframeSketcher  | 2代替パラメータのいずれかがコマンド -            | Y           | ユーザがオプションを提供すると、   |
 |Install                        | で使用することができますWireframeSketcher,       |             | システムはインストールプロセスを   |
 |                               | wireframe-sketcher, wireframesketcher            |             | 開始します                         |
 |                               | eg: ptconfigure wireframe-sketcher Install       |             |                                    |
 +-------------------------------+--------------------------------------------------+-------------+------------------------------------+
 |ptconfigure WireframeSketcher  | 2代替パラメータのいずれかがコマンド -            | N           | ユーザがオプションを提供すると、   | 
 |Install                        | で使用することができますWireframeSketcher,       |             | システムはインストールプロセス     |
 |                               | wireframe-sketcher, wireframesketcher            |             | を停止します                       |
 |                               | eg: ptconfigure wireframe-sketcher Install|      |             |                                    |
 +-------------------------------+--------------------------------------------------+-------------+------------------------------------+




利点
--------------

* 利用可能な機能の範囲
* 情報や機能の相対的な優先順位
* 特定の種類の情報を表示するための規則
* ディスプレイ上のさまざまなシナリオの効果
 

