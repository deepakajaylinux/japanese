============
Zephir
============


概要
--------------------

Zephir - Ze(nd Engine) Ph(p) I(nt)r(mediate) - PHP用の拡張機能の作成と保守性を緩和し、高レベルの言語である。 ZEPHIR拡張は++などのgcc /打ち鳴らす/ VCなどの主要なCコンパイラでコンパイルし、最適化することができるCコードに輸出されている。機能は、 PHP言語にさらされる。 ZEPHIRはオープンソースであり、高レベルの開発者は低レベルのPHP拡張を行うことができます。


helpコマンド
---------------

このコマンドは、 ZEPHIRモジュールの使用方法について説明します。それはZEPHIRのパラメータとZEPHIRモジュールの機能の構文を示しています。ザ·
ZEPHIRモジュールのhelpコマンドは、以下の通りである

.. code-block:: bash

	ptconfigure Zephir help

上記のコマンドの絵画表現は、以下に記載されている


.. code-block:: bash

 kevvell@corp:/# ptconfigure Zephir help
 ******************************


  This command allows you to update Zephir.

  Zephir, zephir

        - install
        Installs the latest version of zephir
        example: ptconfigure zephir install

 ------------------------------
 End Help
 ******************************


インストール
--------------

端末上ZEPHIRモジュールをインストールするために使用されるコマンドは、以下に記載されている


.. code-block:: bash

	ptconfigure zephir install

上記のコマンドの絵画表現は、以下に記載されている


.. code-block:: bash


 kevell@corp:/# ptconfigure zephir install

 Install Zephir? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Zephir!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-19147788395.sh
 chmod 755 /tmp/ptconfigure-temp-script-19147788395.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-19147788395.sh Permissions
 Executing /tmp/ptconfigure-temp-script-19147788395.sh
 W: GPG error: http://oss.oracle.com unstable Release: The following signatures were invalid: KEYEXPIRED 1378511808 KEYEXPIRED 1378511808  
 KEYEXPIRED 1378511808
 W: Failed to fetch http://apt.appneta.com/murali/dists/trusty/main/binary-amd64/Packages  404  Not Found [IP: 107.20.222.96 80]

 W: Failed to fetch http://apt.appneta.com/murali/dists/trusty/main/binary-i386/Packages  404  Not Found [IP: 107.20.222.96 80]

 W: Failed to fetch http://oss.oracle.com/debian/dists/unstable/main/binary-amd64/Packages  HttpError404

 W: Failed to fetch http://oss.oracle.com/debian/dists/unstable/non-free/binary-amd64/Packages  HttpError404

 E: Some index files failed to download. They have been ignored, or old ones used instead.
 Ign http://archive.ubuntu.com trusty InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://archive.ubuntu.com trusty-updates InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://apt.appneta.com trusty InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://packages.dotdeb.org squeeze InRelease
 Hit http://packages.elasticsearch.org stable Release.gpg
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Ign http://archive.ubuntu.com trusty-backports InRelease
 Get:1 http://extras.ubuntu.com trusty Release.gpg [72 B]
 Ign http://apt.appneta.com trusty Release.gpg
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Ign http://archive.ubuntu.com trusty-security InRelease
 Ign http://apt.appneta.com trusty Release
 Hit http://extras.ubuntu.com trusty Release
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://archive.ubuntu.com trusty Release.gpg
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Get:2 http://archive.ubuntu.com trusty-updates Release.gpg [933 B] 

 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://archive.ubuntu.com trusty-backports Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Get:3 http://archive.ubuntu.com trusty-security Release.gpg [933 B]
 Hit http://ppa.launchpad.net trusty Release
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://archive.ubuntu.com trusty Release
 Hit http://ppa.launchpad.net trusty Release
 Get:4 http://archive.ubuntu.com trusty-updates Release [63.5 kB]
 Hit http://ppa.launchpad.net trusty Release
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-backports Release
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Get:5 http://archive.ubuntu.com trusty-security Release [63.5 kB]
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Get:6 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Err http://apt.appneta.com trusty/main amd64 Packages
  404  Not Found [IP: 107.20.222.96 80]
 Err http://apt.appneta.com trusty/main i386 Packages
  404  Not Found [IP: 107.20.222.96 80]
 Hit http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Ign http://apt.appneta.com trusty/main Translation-en_IN
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Ign http://apt.appneta.com trusty/main Translation-en

 Get:7 http://oss.oracle.com unstable/main amd64 Packages
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex
 Hit http://archive.ubuntu.com trusty/main Sources
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex
 Hit http://archive.ubuntu.com trusty/restricted Sources
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Hit http://archive.ubuntu.com trusty/universe Sources
 Hit http://archive.ubuntu.com trusty/multiverse Sources
 Hit http://archive.ubuntu.com trusty/main amd64 Packages
 Ign http://ppa.launchpad.net trusty/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages
 Ign http://ppa.launchpad.net trusty/main Translation-en
 Hit http://oss.oracle.com unstable/main i386 Packages
 Hit http://oss.oracle.com unstable/non-free i386 Packages
 Get:8 http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty/universe i386 Packages
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty/main Translation-en
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty/restricted Translation-en
 Hit http://archive.ubuntu.com trusty/universe Translation-en
 Get:9 http://archive.ubuntu.com trusty-updates/main Sources [189 kB]
 Err http://oss.oracle.com unstable/main amd64 Packages
  HttpError404
 Err http://oss.oracle.com unstable/non-free amd64 Packages
  HttpError404

 Ign http://oss.oracle.com unstable/main Translation-en_IN
 Ign http://oss.oracle.com unstable/main Translation-en
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN
 Ign http://oss.oracle.com unstable/non-free Translation-en
 Get:10 http://archive.ubuntu.com trusty-updates/restricted Sources [2,564 B]
 Get:11 http://archive.ubuntu.com trusty-updates/universe Sources [107 kB]
 Get:12 http://archive.ubuntu.com trusty-updates/multiverse Sources [4,765 B]
 Get:13 http://archive.ubuntu.com trusty-updates/main amd64 Packages [489 kB]
 Get:14 http://archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:15 http://archive.ubuntu.com trusty-updates/universe amd64 Packages [260 kB]
 Get:16 http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.7 kB]
 Get:17 http://archive.ubuntu.com trusty-updates/main i386 Packages [478 kB]
 Get:18 http://archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:19 http://archive.ubuntu.com trusty-updates/universe i386 Packages [262 kB]
 Get:20 http://archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.9 kB]
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://archive.ubuntu.com trusty-backports/main Sources
 Hit http://archive.ubuntu.com trusty-backports/restricted Sources
 Hit http://archive.ubuntu.com trusty-backports/universe Sources
 Hit http://archive.ubuntu.com trusty-backports/multiverse Sources
 Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-backports/universe Translation-en
 Get:21 http://archive.ubuntu.com trusty-security/main Sources [76.1 kB]
 Get:22 http://archive.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Get:23 http://archive.ubuntu.com trusty-security/universe Sources [18.0 kB]
 Get:24 http://archive.ubuntu.com trusty-security/multiverse Sources [1,905 B]
 Get:25 http://archive.ubuntu.com trusty-security/main amd64 Packages [251 kB]
 Get:26 http://archive.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:27 http://archive.ubuntu.com trusty-security/universe amd64 Packages [89.7 kB]
 Get:28 http://archive.ubuntu.com trusty-security/multiverse amd64 Packages [3,459 B]
 Get:29 http://archive.ubuntu.com trusty-security/main i386 Packages [242 kB]
 Get:30 http://archive.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:31 http://archive.ubuntu.com trusty-security/universe i386 Packages [89.7 kB]
 Get:32 http://archive.ubuntu.com trusty-security/multiverse i386 Packages [3,628 B]
 Hit http://archive.ubuntu.com trusty-security/main Translation-en
 Hit http://archive.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-security/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-security/universe Translation-en
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN 

 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 2,759 kB in 1min 53s (24.4 kB/s)
 Temp File /tmp/ptconfigure-temp-script-19147788395.sh Removed
 W: Duplicate sources.list entry http://oss.oracle.com/debian/ unstable/main i386 Packages (/var/lib/apt/lists/
 oss.oracle.com_debian_dists_unstable_main_binary-i386_Packages)
 W: Duplicate sources.list entry http://oss.oracle.com/debian/ unstable/non-free i386 Packages (/var/lib/apt/lists
 oss.oracle.com_debian_dists_unstable_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/	
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/  
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/  	
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/\
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/ 
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package gcc from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package make from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package re2c from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package php5 from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package php5-json from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  debhelper dh-apparmor libmail-sendmail-perl pkg-php-tools po-debconf shtool

 Suggested packages:
  dh-make libmail-box-perl
 The following NEW packages will be installed:
  debhelper dh-apparmor libmail-sendmail-perl php5-dev pkg-php-tools
  po-debconf shtool
 0 upgraded, 7 newly installed, 0 to remove and 263 not upgraded.
 Need to get 1,380 kB of archives.
 After this operation, 6,097 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main po-debconf all 1.0.16+nmu2ubuntu1 [210 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty-updates/main dh-apparmor all 2.8.95~2430-0ubuntu5.1 [11.5 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main debhelper all 9.20131227ubuntu1 [604 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main libmail-sendmail-perl all 0.79.16-1 [26.5 kB]
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main shtool all 2.0.8-6 [149 kB]
 Get:6 http://archive.ubuntu.com/ubuntu/ trusty-updates/main php5-dev amd64 5.5.9+dfsg-1ubuntu4.7 [357 kB]
 Get:7 http://archive.ubuntu.com/ubuntu/ trusty/main pkg-php-tools all 1.11 [21.6 kB]
 Fetched 1,276 kB in 28s (44.6 kB/s)
 Selecting previously unselected package po-debconf.
 (Reading database ... 233467 files and directories currently installed.)
 Preparing to unpack .../po-debconf_1.0.16+nmu2ubuntu1_all.deb ...
 Unpacking po-debconf (1.0.16+nmu2ubuntu1) ...
 Selecting previously unselected package dh-apparmor.
 Preparing to unpack .../dh-apparmor_2.8.95~2430-0ubuntu5.1_all.deb ...
 Unpacking dh-apparmor (2.8.95~2430-0ubuntu5.1) ...
 Selecting previously unselected package debhelper.
 Preparing to unpack .../debhelper_9.20131227ubuntu1_all.deb ...
 Unpacking debhelper (9.20131227ubuntu1) ...
 Selecting previously unselected package libmail-sendmail-perl.
 Preparing to unpack .../libmail-sendmail-perl_0.79.16-1_all.deb ...
 Unpacking libmail-sendmail-perl (0.79.16-1) ...
 Selecting previously unselected package shtool.
 Preparing to unpack .../shtool_2.0.8-6_all.deb ...
 Unpacking shtool (2.0.8-6) ...
 Selecting previously unselected package php5-dev.
 Preparing to unpack .../php5-dev_5.5.9+dfsg-1ubuntu4.7_amd64.deb ...
 Unpacking php5-dev (5.5.9+dfsg-1ubuntu4.7) ...

 Selecting previously unselected package pkg-php-tools.
 Preparing to unpack .../pkg-php-tools_1.11_all.deb ...
 Unpacking pkg-php-tools (1.11) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Registering documents with scrollkeeper...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up po-debconf (1.0.16+nmu2ubuntu1) ...
 Setting up dh-apparmor (2.8.95~2430-0ubuntu5.1) ...
 Setting up debhelper (9.20131227ubuntu1) ...
 Setting up libmail-sendmail-perl (0.79.16-1) ...
 Setting up shtool (2.0.8-6) ...
 Setting up php5-dev (5.5.9+dfsg-1ubuntu4.7) ...
 update-alternatives: using /usr/bin/php-config5 to provide /usr/bin/php-config (php-config) in auto mode
 update-alternatives: using /usr/bin/phpize5 to provide /usr/bin/phpize (phpize) in auto mode
 Setting up pkg-php-tools (1.11) ...
 [Pharaoh Logging] Adding Package php5-dev from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   libpcrecpp0
 The following NEW packages will be installed:
  libpcre3-dev libpcrecpp0
 0 upgraded, 2 newly installed, 0 to remove and 263 not upgraded.
 Need to get 237 kB/251 kB of archives.
 After this operation, 951 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main libpcre3-dev amd64 1:8.31-2ubuntu2 [237 kB]
 Fetched 237 kB in 12s (19.5 kB/s)
 Selecting previously unselected package libpcrecpp0:amd64.
 (Reading database ... 234310 files and directories currently installed.)
 Preparing to unpack .../libpcrecpp0_1%3a8.31-2ubuntu2_amd64.deb ...
 Unpacking libpcrecpp0:amd64 (1:8.31-2ubuntu2) ...
 Selecting previously unselected package libpcre3-dev:amd64.
 Preparing to unpack .../libpcre3-dev_1%3a8.31-2ubuntu2_amd64.deb ...
 Unpacking libpcre3-dev:amd64 (1:8.31-2ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libpcrecpp0:amd64 (1:8.31-2ubuntu2) ...
 Setting up libpcre3-dev:amd64 (1:8.31-2ubuntu2) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package libpcre3-dev from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-37330975073.sh
 chmod 755 /tmp/ptconfigure-temp-script-37330975073.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-37330975073.sh Permissions
 Executing /tmp/ptconfigure-temp-script-37330975073.sh
 Cloning into 'zephir'...
 remote: Counting objects: 22313, done.
 remote: Compressing objects: 100% (194/194), done.
 remote: Total 22313 (delta 118), reused 0 (delta 0), pack-reused 22119
 Receiving objects: 100% (22313/22313), 12.33 MiB | 40.00 KiB/s, done.
 Resolving deltas: 100% (16296/16296), done.
 Checking connectivity... done.
 Cloning into 'json-c'...
 remote: Counting objects: 1531, done.
 remote: Total 1531 (delta 0), reused 0 (delta 0), pack-reused 1531
 Receiving objects: 100% (1531/1531), 941.13 KiB | 59.00 KiB/s, done.
 Resolving deltas: 100% (828/828), done.
 Checking connectivity... done.
 autoreconf: Entering directory `.'
 autoreconf: configure.ac: not using Gettext
 autoreconf: running: aclocal 
 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from...
 configure.ac:43: the top level
 autoreconf: configure.ac: tracing

 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from...
 configure.ac:43: the top level
 autoreconf: running: libtoolize --copy
 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from... 
 configure.ac:43: the top level
 autoreconf: running: /usr/bin/autoconf
 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from...
 configure.ac:43: the top level
 autoreconf: running: /usr/bin/autoheader
 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from...
 configure.ac:43: the top level
 autoreconf: running: automake --add-missing --copy --no-force
 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from...
 configure.ac:43: the top level
 configure.ac:15: installing './compile'
 configure.ac:57: installing './config.guess'
 configure.ac:57: installing './config.sub'
 configure.ac:6: installing './install-sh'
 configure.ac:6: installing './missing'
 Makefile.am: installing './INSTALL' 

 Makefile.am: installing './depcomp'
 parallel-tests: installing './test-driver'
 autoreconf: Leaving directory `.'
 configure.ac:43: warning: AC_LANG_CONFTEST: no AC_LANG_SOURCE call detected in body
 ../../lib/autoconf/lang.m4:193: AC_LANG_CONFTEST is expanded from...
 ../../lib/autoconf/general.m4:2661: _AC_LINK_IFELSE is expanded from...
 ../../lib/autoconf/general.m4:2678: AC_LINK_IFELSE is expanded from...
 configure.ac:43: the top level
 Submodule 'json-c' (git://github.com/phalcon/json-c.git) registered for path 'json-c'
 Submodule path 'json-c': checked out 'aa31af396a5b928ac29ba30f960f3d6f7072c5ae'
 libtoolize: putting auxiliary files in `.'.
 libtoolize: copying file `./ltmain.sh'
 libtoolize: Consider adding `AC_CONFIG_MACRO_DIR([m4])' to configure.ac and
 libtoolize: rerunning libtoolize, to keep the correct libtool macros in-tree.
 libtoolize: Consider adding `-I m4' to ACLOCAL_AMFLAGS in Makefile.am.
 checking for a BSD-compatible install... /usr/bin/install -c
 checking whether build environment is sane... yes
 checking for a thread-safe mkdir -p... /bin/mkdir -p
 checking for gawk... gawk
 checking whether make sets $(MAKE)... yes
 checking whether make supports nested variables... yes
 checking whether make sets $(MAKE)... (cached) yes
 checking for style of include used by make... GNU
 checking for gcc... gcc
 checking whether the C compiler works... yes
 checking for C compiler default output file name... a.out
 checking for suffix of executables... 
 checking whether we are cross compiling... no
 checking for suffix of object files... o
 checking whether we are using the GNU C compiler... yes
 checking whether gcc accepts -g... yes
 checking for gcc option to accept ISO C89... none needed 

 checking whether gcc understands -c and -o together... yes
 checking dependency style of gcc... gcc3
 checking how to run the C preprocessor... gcc -E
 checking for grep that handles long lines and -e... /bin/grep
 checking for egrep... /bin/grep -E
 checking for ANSI C header files... yes
 checking for sys/types.h... yes
 checking for sys/stat.h... yes
 checking for stdlib.h... yes
 checking for string.h... yes
 checking for memory.h... yes
 checking for strings.h... yes
 checking for inttypes.h... yes
 checking for stdint.h... yes
 checking for unistd.h... yes
 checking fcntl.h usability... yes
 checking fcntl.h presence... yes
 checking for fcntl.h... yes
 checking limits.h usability... yes
 checking limits.h presence... yes
 checking for limits.h... yes
 checking for strings.h... (cached) yes
 checking syslog.h usability... yes
 checking syslog.h presence... yes
 checking for syslog.h... yes
 checking for unistd.h... (cached) yes
 checking sys/cdefs.h usability... yes
 checking sys/cdefs.h presence... yes
 checking for sys/cdefs.h... yes
 checking sys/param.h usability... yes
 checking sys/param.h presence... yes
 checking for sys/param.h... yes
 checking stdarg.h usability... yes
 checking stdarg.h presence... yes 

 checking for stdarg.h... yes
 checking locale.h usability... yes
 checking locale.h presence... yes
 checking for locale.h... yes
 checking for inttypes.h... (cached) yes
 checking for an ANSI C-conforming const... yes
 checking for size_t... yes
 checking for vprintf... yes
 checking for _doprnt... no
 checking for working memcmp... yes
 checking for stdlib.h... (cached) yes
 checking for GNU libc compatible malloc... yes
 checking for stdlib.h... (cached) yes
 checking for GNU libc compatible realloc... yes
 checking for strcasecmp... yes
 checking for strdup... yes
 checking for strerror... yes
 checking for snprintf... yes
 checking for vsnprintf... yes
 checking for vasprintf... yes
 checking for open... yes
 checking for vsyslog... yes
 checking for strncasecmp... yes
 checking for setlocale... yes
 checking whether INFINITY is declared... yes
 checking whether nan is declared... yes
 checking whether isnan is declared... yes
 checking whether isinf is declared... yes
 checking whether _isnan is declared... no
 checking whether _finite is declared... no
 checking if .gnu.warning accepts long strings... no
 checking build system type... x86_64-unknown-linux-gnu 

 checking host system type... x86_64-unknown-linux-gnu
 checking how to print strings... printf
 checking for a sed that does not truncate output... /bin/sed
 checking for fgrep... /bin/grep -F
 checking for ld used by gcc... /usr/bin/ld
 checking if the linker (/usr/bin/ld) is GNU ld... yes
 checking for BSD- or MS-compatible name lister (nm)... /usr/bin/nm -B
 checking the name lister (/usr/bin/nm -B) interface... BSD nm
 checking whether ln -s works... yes
 checking the maximum length of command line arguments... 1572864
 checking whether the shell understands some XSI constructs... yes
 checking whether the shell understands "+="... yes
 checking how to convert x86_64-unknown-linux-gnu file names to x86_64-unknown-linux-gnu format... func_convert_file_noop
 checking how to convert x86_64-unknown-linux-gnu file names to toolchain format... func_convert_file_noop
 checking for /usr/bin/ld option to reload object files... -r
 checking for objdump... objdump
 checking how to recognize dependent libraries... pass_all
 checking for dlltool... no
 checking how to associate runtime and link libraries... printf %s\n
 checking for ar... ar
 checking for archiver @FILE support... @
 checking for strip... strip
 checking for ranlib... ranlib
 checking command to parse /usr/bin/nm -B output from gcc object... ok
 checking for sysroot... no
 checking for mt... mt
 checking if mt is a manifest tool... no
 checking for dlfcn.h... yes
 checking for objdir... .libs
 checking if gcc supports -fno-rtti -fno-exceptions... no
 checking for gcc option to produce PIC... -fPIC -DPIC
 checking if gcc PIC flag -fPIC -DPIC works... yes
 checking if gcc static flag -static works... yes
 checking if gcc supports -c -o file.o... yes
 checking if gcc supports -c -o file.o... (cached) yes
 checking whether the gcc linker (/usr/bin/ld -m elf_x86_64) supports shared libraries... yes
 checking whether -lc should be explicitly linked in... no
 checking dynamic linker characteristics... GNU/Linux ld.so
 checking how to hardcode library paths into programs... immediate

 checking whether stripping libraries is possible... yes
 checking if libtool supports shared libraries... yes
 checking whether to build shared libraries... yes
 checking whether to build static libraries... yes
 checking for -Bsymbolic-functions linker flag... yes
 checking that generated files are newer than configure... done
 configure: creating ./config.status
 config.status: creating Makefile
 config.status: creating json-c.pc
 config.status: creating tests/Makefile
 config.status: creating json-c-uninstalled.pc
 config.status: creating config.h
 config.status: creating json_config.h
 config.status: executing depfiles commands
 config.status: executing libtool commands
 (CDPATH="${ZSH_VERSION+.}:" && cd . && /bin/bash /home/murali/zephir/json-c/missing autoheader)
 rm -f stamp-h1
 touch config.h.in
 cd . && /bin/bash ./config.status config.h
 config.status: creating config.h
 config.status: config.h is unchanged
 make  all-recursive
 make[1]: Entering directory `/home/murali/zephir/json-c'
 Making all in .
 make[2]: Entering directory `/home/murali/zephir/json-c'
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -  
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT arraylist.lo -MD -MP -MF .deps/arraylist.Tpo -c -o arraylist.lo arraylist.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT  
 - g -O2 -MT arraylist.lo -MD -MP -MF .deps/arraylist.Tpo -c arraylist.c  -fPIC -DPIC -o .libs/arraylist.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT arraylist.lo -MD -MP -MF .deps/arraylist.Tpo -c arraylist.c -o arraylist.o >/dev/null 2>&1
 mv -f .deps/arraylist.Tpo .deps/arraylist.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT debug.lo -MD -MP -MF .deps/debug.Tpo -c -o debug.lo debug.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT debug.lo -MD -MP -MF .deps/debug.Tpo -c debug.c  -fPIC -DPIC -o .libs/debug.o
 l ibtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 -g -O2 -MT debug.lo -MD -MP -MF .deps/debug.Tpo -c debug.c -o debug.o >/dev/null 2>&1
 mv -f .deps/debug.Tpo .deps/debug.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT json_c_version.lo -MD -MP -MF .deps/json_c_version.Tpo -c -o json_c_version.lo  
 json_c_version.c

 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -
 MT json_c_version.lo -MD -MP -MF .deps/json_c_version.Tpo -c json_c_version.c  -fPIC -DPIC -o .libs/json_c_version.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT json_c_version.lo -MD -MP -MF .deps/json_c_version.Tpo -c json_c_version.c -o json_c_version.o >/dev/null 2>&1
 mv -f .deps/json_c_version.Tpo .deps/json_c_version.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT json_object.lo -MD -MP -MF .deps/json_object.Tpo -c -o json_object.lo json_object.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT json_object.lo -MD -MP -MF .deps/json_object.Tpo -c json_object.c  -fPIC -DPIC -o .libs/json_object.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT json_object.lo -MD -MP -MF .deps/json_object.Tpo -c json_object.c -o json_object.o >/dev/null 2>&1
 mv -f .deps/json_object.Tpo .deps/json_object.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT json_object_iterator.lo -MD -MP -MF .deps/json_object_iterator.Tpo -c -o  
 json_object_iterator.lo json_object_iterator.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT  
 - g -O2 -MT json_object_iterator.lo -MD -MP -MF .deps/json_object_iterator.Tpo -c json_object_iterator.c  -fPIC -DPIC -o .libs/ 
 json_object_iterator.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT  
 - g -O2 -MT json_object_iterator.lo -MD -MP -MF .deps/json_object_iterator.Tpo -c json_object_iterator.c -o json_object_iterator.o >/dev/ 
 null  2>&1
 mv -f .deps/json_object_iterator.Tpo .deps/json_object_iterator.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT json_tokener.lo -MD -MP -MF .deps/json_tokener.Tpo -c -o json_tokener.lo json_tokener.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT  
 - g -O2 -MT json_tokener.lo -MD -MP -MF .deps/json_tokener.Tpo -c json_tokener.c  -fPIC -DPIC -o .libs/json_tokener.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT json_tokener.lo -MD -MP -MF .deps/json_tokener.Tpo -c json_tokener.c -o json_tokener.o >/dev/null 2>&1
 mv -f .deps/json_tokener.Tpo .deps/json_tokener.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT json_util.lo -MD -MP -MF .deps/json_util.Tpo -c -o json_util.lo json_util.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT json_util.lo -MD -MP -MF .deps/json_util.Tpo -c json_util.c  -fPIC -DPIC -o .libs/json_util.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT json_util.lo -MD -MP -MF .deps/json_util.Tpo -c json_util.c -o json_util.o >/dev/null 2>&1
 mv -f .deps/json_util.Tpo .deps/json_util.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT linkhash.lo -MD -MP -MF .deps/linkhash.Tpo -c -o linkhash.lo linkhash.c
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT linkhash.lo -MD -MP -MF .deps/linkhash.Tpo -c linkhash.c  -fPIC -DPIC -o .libs/linkhash.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT linkhash.lo -MD -MP -MF .deps/linkhash.Tpo -c linkhash.c -o linkhash.o >/dev/null 2>&1
 mv -f .deps/linkhash.Tpo .deps/linkhash.Plo
 /bin/bash ./libtool  --tag=CC   --mode=compile gcc -DHAVE_CONFIG_H -I.    -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter - 
 std=gnu99 -D_GNU_SOURCE -D_REENTRANT -g -O2 -MT printbuf.lo -MD -MP -MF .deps/printbuf.Tpo -c -o printbuf.lo printbuf.c

 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT printbuf.lo -MD -MP -MF .deps/printbuf.Tpo -c printbuf.c  -fPIC -DPIC -o .libs/printbuf.o
 libtool: compile:  gcc -DHAVE_CONFIG_H -I. -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE -D_REENTRANT 
 - g -O2 -MT printbuf.lo -MD -MP -MF .deps/printbuf.Tpo -c printbuf.c -o printbuf.o >/dev/null 2>&1
 mv -f .deps/printbuf.Tpo .deps/printbuf.Plo
 /bin/bash ./libtool  --tag=CC   --mode=link gcc -Wall -Werror -Wextra -Wwrite-strings -Wno-unused-parameter -std=gnu99 -D_GNU_SOURCE - 
 D_REENTRANT -g -O2 -version-info 2:0:0 -no-undefined -Wl,-Bsymbolic-functions  -o libjson-c.la -rpath /usr/local/lib arraylist.lo debug.lo  
 json_c_version.lo json_object.lo json_object_iterator.lo json_tokener.lo json_util.lo linkhash.lo printbuf.lo  
 libtool: link: gcc -shared  -fPIC -DPIC  .libs/arraylist.o .libs/debug.o .libs/json_c_version.o .libs/json_object.o .libs/ 
 json_object_iterator.o .libs/json_tokener.o .libs/json_util.o .libs/linkhash.o .libs/printbuf.o    -O2 -Wl,-Bsymbolic-functions   -Wl,-
 soname  -Wl,libjson-c.so.2 -o .libs/libjson-c.so.2.0.0
 libtool: link: (cd ".libs" && rm -f "libjson-c.so.2" && ln -s "libjson-c.so.2.0.0" "libjson-c.so.2")
 libtool: link: (cd ".libs" && rm -f "libjson-c.so" && ln -s "libjson-c.so.2.0.0" "libjson-c.so")
 libtool: link: ar cru .libs/libjson-c.a  arraylist.o debug.o json_c_version.o json_object.o json_object_iterator.o json_tokener.o json_util.o 
 linkhash.o printbuf.o
 libtool: link: ranlib .libs/libjson-c.a
 libtool: link: ( cd ".libs" && rm -f "libjson-c.la" && ln -s "../libjson-c.la" "libjson-c.la" )
 make[2]: Leaving directory `/home/murali/zephir/json-c'
 Making all in tests
 make[2]: Entering directory `/home/murali/zephir/json-c/tests'
 make[2]: Nothing to be done for `all'.
 make[2]: Leaving directory `/home/murali/zephir/json-c/tests'
 make[1]: Leaving directory `/home/murali/zephir/json-c'
 Making install in .
 make[1]: Entering directory `/home/murali/zephir/json-c'
 make[2]: Entering directory `/home/murali/zephir/json-c'
 /bin/mkdir -p '/usr/local/lib'
 /bin/bash ./libtool   --mode=install /usr/bin/install -c   libjson-c.la '/usr/local/lib'
 libtool: install: /usr/bin/install -c .libs/libjson-c.so.2.0.0 /usr/local/lib/libjson-c.so.2.0.0
 libtool: install: (cd /usr/local/lib && { ln -s -f libjson-c.so.2.0.0 libjson-c.so.2 || { rm -f libjson-c.so.2 && ln -s libjson-c.so.2.0.0  
 libjson-c.so.2; }; })
 libtool: install: (cd /usr/local/lib && { ln -s -f libjson-c.so.2.0.0 libjson-c.so || { rm -f libjson-c.so && ln -s libjson-c.so.2.0.0 
 libjson-c.so; }; })

 libtool: install: /usr/bin/install -c .libs/libjson-c.lai /usr/local/lib/libjson-c.la
 libtool: install: /usr/bin/install -c .libs/libjson-c.a /usr/local/lib/libjson-c.a
 libtool: install: chmod 644 /usr/local/lib/libjson-c.a
 libtool: install: ranlib /usr/local/lib/libjson-c.a
 libtool: finish: PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/sbin" ldconfig -n /usr/local/lib
 ----------------------------------------------------------------------
 Libraries have been installed in:
   /usr/local/lib

 If you ever happen to want to link against installed libraries
 in a given directory, LIBDIR, you must either use libtool, and
 specify the full pathname of the library, or use the `-LLIBDIR'
 flag during linking and do at least one of the following:
   - add LIBDIR to the `LD_LIBRARY_PATH' environment variable
     during execution
   - add LIBDIR to the `LD_RUN_PATH' environment variable
     during linking
   - use the `-Wl,-rpath -Wl,LIBDIR' linker flag
   - have your system administrator add LIBDIR to `/etc/ld.so.conf'

 See any operating system documentation about shared libraries for
 more information, such as the ld(1) and ld.so(8) manual pages.
 ----------------------------------------------------------------------
 /bin/mkdir -p '/usr/local/include/json-c'
 /usr/bin/install -c -m 644 arraylist.h bits.h debug.h json.h json_config.h json_c_version.h json_inttypes.h json_object.h  
 json_object_iterator.h json_object_private.h json_tokener.h json_util.h linkhash.h printbuf.h '/usr/local/include/json-c'
  /bin/mkdir -p '/usr/local/lib/pkgconfig'
 /usr/bin/install -c -m 644 json-c.pc '/usr/local/lib/pkgconfig'
 make[2]: Leaving directory `/home/murali/zephir/json-c'
 make[1]: Leaving directory `/home/murali/zephir/json-c'

 Making install in tests
 make[1]: Entering directory `/home/murali/zephir/json-c/tests'
 make[2]: Entering directory `/home/murali/zephir/json-c/tests'
 make[2]: Nothing to be done for `install-exec-am'.
 make[2]: Nothing to be done for `install-data-am'.
 make[2]: Leaving directory `/home/murali/zephir/json-c/tests'
 make[1]: Leaving directory `/home/murali/zephir/json-c/tests'
 Parser statistics: 124 terminals, 99 nonterminals, 449 rules
                    925 states, 0 parser table entries, 0 conflicts
 Temp File /tmp/ptconfigure-temp-script-37330975073.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Zephir: Success
 ------------------------------
 Installer Finished
 ******************************

別のパラメータ
------------------------

コマンドラインで使用することができる2つの別のパラメータがある。

Zephir, zephir

メリット
------------

* ZEPHIRは、コンパイルされた両方の利点だけでなく、インタープリタ言語を提供しています
* メモリの安全性
* どちらの動的/静的型付け、など。
