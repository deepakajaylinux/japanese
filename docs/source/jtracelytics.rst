==============
Tracelytics
==============


概要
-------------

TracelyticsはスケーラブルなWebアーキテクチャを理解するSaaS型アプリケーションのパフォーマンスソリューションです。アプリケーション、層、およびマシン間の境界を消去。トレースを開始。 Tracelyticsはソフトウェア層とマシン間でのリクエストのパフォーマンスと動作に関する情報を収集することにより、複雑な、分散型ウェブアプリケーションの可視性を提供します。 Tracelyticsは、パフォーマンス志向#devopsと他人を助ける#Java 、 #PHP 、 #Ruby 、および#Pythonにおけるクラウド＆分散型のアプリ、のトレースフルスタックのアプリケーションです。すべてをトレースします。


Helpコマンド
----------------

helpコマンドは、とだけでなく、 tracelyticsモジュールに含まれているオプションについての目的について、ユーザーをガイドします。また、 tracelyticsモジュールをインストールするための構文について説明します。 tracelyticsモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash

	ptconfigure tracelytics help


上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure tracelytics help

 ******************************


  This command allows you to update Tracelytics.

  Tracelytics

        - install
        Installs the latest version of tracelytics
        example: ptconfigure tracelytics install

 ------------------------------
 End Help
 *******************************


インストール
------------------


端末上tracelyticsモジュールをインストールするために使用されるコマンドは、以下に記載されている

.. code-block:: bash

	ptconfigure tracelytics install

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

                                                                                                                               [ OK
 kevell@corp:/# ptconfigure tracelytics install

 Install Tracelytics? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Tracelytics!        *
 *******************************
 Enter Your Licence Key:
  9899c7f8-a71f-4e9a-b1e3-c88e198af0ae
 Creating /tmp/ptconfigure-temp-script-85765161565.sh
 chmod 755 /tmp/ptconfigure-temp-script-85765161565.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-85765161565.sh Permissions
 Executing /tmp/ptconfigure-temp-script-85765161565.sh
 --2015-04-06 12:07:21--  https://files.appneta.com/install_appneta.sh
 Resolving files.appneta.com (files.appneta.com)... 54.235.148.241, 107.20.222.96
 Connecting to files.appneta.com (files.appneta.com)|54.235.148.241|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 18477 (18K) [application/octet-stream]
 Saving to: â€˜install_appneta.sh.2â€™ 

 100%[============================================================================================>] 18,477      55.3KB/s   in 0.3s   

 2015-04-06 12:07:23 (55.3 KB/s) - â€˜install_appneta.sh.2â€™ saved [18477/18477]

 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive  
 globally to suppress this message
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive 
 globally to suppress this message
 === Welcome to the AppNeta TraceView installer.
 === This script will now install the tracelyzer, which collects performance data for TraceView.
 === Adding AppNeta APT package repository to system list.
 === Downloading AppNeta package signature public key.
 --2015-04-06 12:07:24--  https://apt.appneta.com/appneta-apt-key.pub
 Resolving apt.appneta.com (apt.appneta.com)... 54.235.148.241, 107.20.222.96
 Connecting to apt.appneta.com (apt.appneta.com)|54.235.148.241|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 1695 (1.7K) [application/octet-stream]
 Saving to: â€˜appneta-apt-key.pubâ€™

     0K .                                                     100% 5.87M=0s

 2015-04-06 12:07:25 (5.87 MB/s) - â€˜appneta-apt-key.pubâ€™ saved [1695/1695]

 === Adding AppNeta package signature public key to system list.
 OK
 Testing connectivity to package repository...done.
 === Downloading AppNeta package index.
 Ign http://archive.ubuntu.com trusty InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://archive.ubuntu.com trusty-updates InRelease
 Ign http://archive.ubuntu.com trusty-backports InRelease
 Ign http://packages.dotdeb.org squeeze InRelease
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://dl.hhvm.com trusty InRelease
 Hit http://extras.ubuntu.com trusty Release.gpg
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Ign http://archive.ubuntu.com trusty-security InRelease
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://extras.ubuntu.com trusty Release
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Hit http://archive.ubuntu.com trusty Release.gpg
 Get:1 http://apt.appneta.com trusty InRelease [9,175 B]
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Get:2 http://apt.appneta.com trusty/main amd64 Packages [8,431 B]
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports Release.gpg
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Get:3 http://apt.appneta.com trusty/main i386 Packages [8,425 B]
 Hit http://archive.ubuntu.com trusty-security Release.gpg
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://archive.ubuntu.com trusty Release
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://archive.ubuntu.com trusty-updates Release
 Get:4 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://ppa.launchpad.net trusty Release
 Hit http://archive.ubuntu.com trusty-backports Release
 Hit http://archive.ubuntu.com trusty-security Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://archive.ubuntu.com trusty/main Sources
 Hit http://ppa.launchpad.net trusty Release
 Hit http://archive.ubuntu.com trusty/restricted Sources
 Hit http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Hit http://archive.ubuntu.com trusty/universe Sources
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://archive.ubuntu.com trusty/multiverse Sources
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty/main amd64 Packages
 Get:5 http://oss.oracle.com unstable/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://apt.appneta.com trusty/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages
 Ign http://us.archive.ubuntu.com precise InRelease
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Ign http://apt.appneta.com trusty/main Translation-en
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex
 Ign http://dl.hhvm.com trusty/main Translation-en
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise Release.gpg
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty/main i386 Packages
 Hit http://us.archive.ubuntu.com precise Release
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Hit http://archive.ubuntu.com trusty/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty/main Translation-en
 Hit http://us.archive.ubuntu.com precise/universe i386 Packages
 Hit http://oss.oracle.com unstable/main i386 Packages
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://us.archive.ubuntu.com precise/main Translation-en
 Hit http://oss.oracle.com unstable/non-free i386 Packages
 Get:6 http://oss.oracle.com unstable/main Translation-en_IN
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Hit http://archive.ubuntu.com trusty/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise/universe Translation-en
 Hit http://archive.ubuntu.com trusty/universe Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Hit http://archive.ubuntu.com trusty-updates/main Sources
 Hit http://archive.ubuntu.com trusty-updates/restricted Sources
 Hit http://archive.ubuntu.com trusty-updates/universe Sources
 Hit http://archive.ubuntu.com trusty-updates/multiverse Sources
 Hit http://archive.ubuntu.com trusty-updates/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/restricted amd64 Packages
 Ign http://us.archive.ubuntu.com precise/main Translation-en_IN
 Ign http://ppa.launchpad.net trusty/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-updates/universe amd64 Packages
 Ign http://us.archive.ubuntu.com precise/universe Translation-en_IN
 Ign http://ppa.launchpad.net trusty/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/main i386 Packages
 Hit http://archive.ubuntu.com trusty-updates/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-updates/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-updates/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en
 Err http://oss.oracle.com unstable/main amd64 Packages
  HttpError404
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://archive.ubuntu.com trusty-backports/main Sources
 Err http://oss.oracle.com unstable/non-free amd64 Packages
  HttpError404
 Hit http://archive.ubuntu.com trusty-backports/restricted Sources
 Ign http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-backports/universe Sources
 Ign http://oss.oracle.com unstable/main Translation-en
 Hit http://archive.ubuntu.com trusty-backports/multiverse Sources
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN
 Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages
 Ign http://oss.oracle.com unstable/non-free Translation-en 
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
 Hit http://archive.ubuntu.com trusty-security/main Sources
 Hit http://archive.ubuntu.com trusty-security/restricted Sources
 Hit http://archive.ubuntu.com trusty-security/universe Sources
 Hit http://archive.ubuntu.com trusty-security/multiverse Sources
 Hit http://archive.ubuntu.com trusty-security/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-security/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty-security/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-security/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-security/main i386 Packages
 Hit http://archive.ubuntu.com trusty-security/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-security/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-security/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-security/main Translation-en
 Hit http://archive.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-security/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-security/universe Translation-en
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 26.2 kB in 28s (929 B/s)
 W: GPG error: http://oss.oracle.com unstable Release: The following signatures were invalid: KEYEXPIRED 1378511808 KEYEXPIRED 1378511808  
 KEYEXPIRED 1378511808
 W: Failed to fetch http://oss.oracle.com/debian/dists/unstable/main/binary-amd64/Packages  HttpError404

 W: Failed to fetch http://oss.oracle.com/debian/dists/unstable/non-free/binary-amd64/Packages  HttpError404

 E: Some index files failed to download. They have been ignored, or old ones used instead.
 === Executing 'apt-get update' failed; continuing anyway.
 === Installing common library and development headers (liboboe).
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  liboboe-dev liboboe0
 0 upgraded, 2 newly installed, 0 to remove and 281 not upgraded.
 Need to get 60.4 kB of archives.
 After this operation, 280 kB of additional disk space will be used.
 Get:1 http://apt.appneta.com/9899c7f8-a71f-4e9a-b1e3-c88e198af0ae/ trusty/main liboboe0 amd64 1.1.5-trusty1 [24.6 kB]
 Get:2 http://apt.appneta.com/9899c7f8-a71f-4e9a-b1e3-c88e198af0ae/ trusty/main liboboe-dev amd64 1.1.5-trusty1 [35.7 kB]
 Fetched 60.4 kB in 2s (23.2 kB/s)
 Selecting previously unselected package liboboe0.
 (Reading database ... 242145 files and directories currently installed.)
 Preparing to unpack .../liboboe0_1.1.5-trusty1_amd64.deb ...
 Unpacking liboboe0 (1.1.5-trusty1) ...
 Selecting previously unselected package liboboe-dev.
 Preparing to unpack .../liboboe-dev_1.1.5-trusty1_amd64.deb ...
 Unpacking liboboe-dev (1.1.5-trusty1) ...
 Setting up liboboe0 (1.1.5-trusty1) ...
 Setting up liboboe-dev (1.1.5-trusty1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 W: Duplicate sources.list entry http://oss.oracle.com/debian/ unstable/main i386 Packages (/var/lib/apt/lists/ 
 oss.oracle.com_debian_dists_unstable_main_binary-i386_Packages)
 W: Duplicate sources.list entry http://oss.oracle.com/debian/ unstable/non-free i386 Packages (/var/lib/apt/lists/ 
 oss.oracle.com_debian_dists_unstable_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/  
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/ 
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/ 
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/ 
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/
 packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 === Installing the tracelyzer (performance aggregator daemon).
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  tracelyzer
 0 upgraded, 1 newly installed, 0 to remove and 281 not upgraded.
 Need to get 567 kB of archives.
 After this operation, 2,372 kB of additional disk space will be used.
 Get:1 http://apt.appneta.com/9899c7f8-a71f-4e9a-b1e3-c88e198af0ae/ trusty/main tracelyzer amd64 1.1.10-trusty1 [567 kB]
 Fetched 567 kB in 4s (138 kB/s)
 Download complete and in download only mode
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  tracelyzer
 0 upgraded, 1 newly installed, 0 to remove and 281 not upgraded.
 Need to get 0 B/567 kB of archives.
 After this operation, 2,372 kB of additional disk space will be used.
 Selecting previously unselected package tracelyzer.
 (Reading database ... 242164 files and directories currently installed.)
 Preparing to unpack .../tracelyzer_1.1.10-trusty1_amd64.deb ...
 Unpacking tracelyzer (1.1.10-trusty1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up tracelyzer (1.1.10-trusty1) ...
 Adding group `appneta' (GID 147) ...
 Done.
 Adding system user `appneta' (UID 135) ...
 Adding new user `appneta' (UID 135) with group `appneta' ...
 Not creating home directory `/var/log/tracelyzer'. 

 Welcome to the AppNeta configuration utility.

 Reading access_key from /etc/tracelytics.conf...
 Testing system compatibility...
 System passed tests.
 Downloading configuration settings 1/5...
 Downloading configuration settings 2/5...
 Downloading configuration settings 3/5...
 Downloading configuration settings 4/5...
 Downloading configuration settings 5/5... 

 Configuration was successful.
 Starting tracelyzer...done.
 Testing connection (might take couple minutes):
   Testing SSH connection...success.
  Testing Tracelyzer TCP connection and UDP listening...success.
  Testing UDP connection to Tracelyzer...success.
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 === AppNeta TraceView agent extensions are available for the following packages
 === installed on this system: php5-common
 === 
 === To install instrumentation for these components, run as root:
 === 
 ===     apt-get install php-oboe
 === 
 === For help instrumenting other components in your stack (such as Ruby,
 === Python, etc), you may visit:
 ===     http://support.tv.appneta.com/support/solutions/articles/86353-installation-overview
 === 
 === Installation was successful.
 === Please visit your dashboard at https://login.tv.appneta.com to continue the setup process.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 tracelyzer is already the newest version.
 The following NEW packages will be installed:
   libapache2-mod-oboe mod-oboe-ps
 0 upgraded, 2 newly installed, 0 to remove and 281 not upgraded.
 Need to get 2,254 kB of archives.
 After this operation, 12.8 MB of additional disk space will be used.
 Get:1 http://apt.appneta.com/9899c7f8-a71f-4e9a-b1e3-c88e198af0ae/ trusty/main mod-oboe-ps amd64 1.7.30.5-trusty3 [2,241 kB]
 Get:2 http://apt.appneta.com/9899c7f8-a71f-4e9a-b1e3-c88e198af0ae/ trusty/main libapache2-mod-oboe amd64 1.2.3-trusty2 [12.6 kB]
 Fetched 2,254 kB in 21s (104 kB/s)
 Selecting previously unselected package mod-oboe-ps.
 (Reading database ... 242186 files and directories currently installed.)
 Preparing to unpack .../mod-oboe-ps_1.7.30.5-trusty3_amd64.deb ...
 Unpacking mod-oboe-ps (1.7.30.5-trusty3) ...
 Selecting previously unselected package libapache2-mod-oboe.
 Preparing to unpack .../libapache2-mod-oboe_1.2.3-trusty2_amd64.deb ...
 Unpacking libapache2-mod-oboe (1.2.3-trusty2) ...
 Setting up mod-oboe-ps (1.7.30.5-trusty3) ...
 Enabling module oboe_ps.
 To activate the new configuration, you need to run:
  service apache2 restart
 Setting up libapache2-mod-oboe (1.2.3-trusty2) ...
 Enabling module oboe.
 To activate the new configuration, you need to run:
  service apache2 restart
 * Restarting web server apache2
   ...done.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  php-oboe
 0 upgraded, 1 newly installed, 0 to remove and 281 not upgraded.
 Need to get 78.2 kB of archives.
 After this operation, 453 kB of additional disk space will be used.
 Get:1 http://apt.appneta.com/9899c7f8-a71f-4e9a-b1e3-c88e198af0ae/ trusty/main php-oboe amd64 1.5.1-trusty1 [78.2 kB]
 Fetched 78.2 kB in 1s (49.0 kB/s)
 Selecting previously unselected package php-oboe.
 (Reading database ... 242200 files and directories currently installed.)
 Preparing to unpack .../php-oboe_1.5.1-trusty1_amd64.deb ...
 Unpacking php-oboe (1.5.1-trusty1) ...
 Setting up php-oboe (1.5.1-trusty1) ...
 * Restarting web server apache2
   ...done.
 Temp File /tmp/ptconfigure-temp-script-85765161565.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Tracelytics: Success
 ------------------------------
 Installer Finished
 ******************************


メリット
------------

* が系統的から騒々しいを別々のために一箇所に要求パターンを可視化。
* トランザクションに関与するすべてのマシンをトレース＆シングルクリックでボトルネックを特定。
* クロスホスト、分散トランザクションのトレース
* 実ユーザ監視、など。


