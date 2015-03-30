============
Cassandra
============

概要
-------

Apacheのカサンドラは、単一障害点のない高可用性を提供し、多くのコモディティサーバ間で大量のデータを処理するために設計分散データベース管理システムです。カサンドラは、すべてのクライアントのための低遅延動作が可能非同期マスター少ないレプリケーションで、複数のデータセンターにまたがるクラスタの堅牢なサポートを提供しています。

カサンドラのデータモデルは、調整可能な一貫性を持つパーティション行ストアです。行がテーブルに編成されます。テーブルの主キーの最初のコンポーネントは、パーティション·キーです。パーティション内で、行はキーの残りの列によってクラスタ化される。他の列は、主キーとは別にインデックス化することもできる。

helpコマンド
-------------------

このコマンドは、カサンドラモジュールの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

.. code-block:: bash
        
	        ptconfigure cassandra help

上記のコマンドの絵画表現は、以下の通りです

.. code-block:: bash

 kevell@corp:/# ptconfigure cassandra help

 ******************************


  This command allows you to update Cassandra.

  Cassandra, cassandra

        - install
        Installs the latest version of Cassandra
        example: ptconfigure cassandra install

 ------------------------------
 End Help
 ******************************

インストール
-------------------

このコマンドは、システム内のカサンドラを設置するのに役立ちます。以下のコマンドは、インストールのプロセスを実行します。

.. code-block:: bash

                ptconfigure cassandra install

上記のコマンドの絵画表現は、以下の通りです

.. code-block:: bash


 kevell@corp:/# ptconfigure cassandra install
 Install Cassandra? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Cassandra!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-68300758613.sh
 chmod 755 /tmp/ptconfigure-temp-script-68300758613.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-68300758613.sh Permissions
 Executing /tmp/ptconfigure-temp-script-68300758613.sh
 gpg: directory `/home/karunakaran/.gnupg' created
 gpg: new configuration file `/home/karunakaran/.gnupg/gpg.conf' created
 gpg: WARNING: options in `/home/karunakaran/.gnupg/gpg.conf' are not yet active during this run
 gpg: keyring `/home/karunakaran/.gnupg/secring.gpg' created
 gpg: keyring `/home/karunakaran/.gnupg/pubring.gpg' created
 gpg: requesting key 8D77295D from hkp server pgp.mit.edu
 gpg: /home/karunakaran/.gnupg/trustdb.gpg: trustdb created
 gpg: key 8D77295D: public key "Eric Evans <eevans@sym-link.com>" imported
 gpg: no ultimately trusted keys found
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 gpg: requesting key 2B5C1B00 from hkp server pgp.mit.edu
 gpg: key 2B5C1B00: public key "Sylvain Lebresne (pcmanus) <sylvain@datastax.com>" imported
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 gpg: requesting key 0353B12C from hkp server pgp.mit.edu
 gpg: key 0353B12C: public key "T Jake Luciani <jake@apache.org>" imported
 gpg: no ultimately trusted keys found
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 deb-src http://www.apache.org/dist/cassandra/debian 21x main
 OK
 OK
 OK
 Ign http://dl.google.com stable InRelease
 Hit http://downloads.hipchat.com stable InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://dl.google.com stable Release.gpg
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://downloads.hipchat.com stable/main amd64 Packages
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Hit http://dl.google.com stable Release
 Hit http://dl.google.com stable/main amd64 Packages
 Hit http://dl.google.com stable/main i386 Packages
 Hit http://downloads.hipchat.com stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://dl.google.com stable/main Translation-en_IN
 Ign http://dl.google.com stable/main Translation-en
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://packages.elasticsearch.org stable Release.gpg
 Get:1 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Ign http://archive.canonical.com precise InRelease
 Hit http://packages.elasticsearch.org stable Release
 Hit http://archive.canonical.com precise Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Hit http://archive.canonical.com precise Release
 Hit http://packages.elasticsearch.org stable Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://archive.canonical.com precise/partner Sources
 Hit http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://us.archive.ubuntu.com precise InRelease
 Hit http://archive.canonical.com precise/partner amd64 Packages
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://archive.ubuntu.com trusty InRelease
 Ign http://extras.ubuntu.com precise InRelease
 Ign http://us.archive.ubuntu.com precise-security InRelease
 Get:2 http://oss.oracle.com unstable/main amd64 Packages
 Hit http://archive.canonical.com precise/partner i386 Packages
 Get:3 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Ign http://archive.ubuntu.com trusty-updates InRelease
 Hit http://extras.ubuntu.com precise Release.gpg
 Ign http://downloads.hipchat.com stable/main Translation-en_IN
 Ign http://us.archive.ubuntu.com precise-updates InRelease
 Get:4 http://security.ubuntu.com trusty-security Release [63.5 kB]
 Ign http://archive.ubuntu.com trusty-proposed InRelease
 Hit http://extras.ubuntu.com precise Release
 Ign http://us.archive.ubuntu.com precise-backports InRelease
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Ign http://downloads.hipchat.com stable/main Translation-en
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex
 Hit http://us.archive.ubuntu.com precise Release.gpg
 Ign http://archive.ubuntu.com trusty-backports InRelease
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://extras.ubuntu.com precise/main Sources
 Hit http://mirror.stshosting.co.uk precise InRelease
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex
 Get:5 http://us.archive.ubuntu.com precise-security Release.gpg [198 B]
 Ign http://archive.canonical.com precise/partner Translation-en
 Hit http://archive.ubuntu.com trusty Release.gpg
 Hit http://extras.ubuntu.com precise/main amd64 Packages
 Get:6 http://us.archive.ubuntu.com precise-updates Release.gpg [198 B]
 Get:7 http://archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://extras.ubuntu.com precise/main i386 Packages
 Ign http://downloads-distro.mongodb.org dist InRelease
 Hit http://us.archive.ubuntu.com precise-backports Release.gpg
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:8 http://archive.ubuntu.com trusty-proposed Release.gpg [933 B]
 Hit http://us.archive.ubuntu.com precise Release
 Hit http://archive.ubuntu.com trusty-backports Release.gpg
 Get:9 http://us.archive.ubuntu.com precise-security Release [54.3 kB]
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://archive.ubuntu.com trusty Release
 Get:10 http://archive.ubuntu.com trusty-updates Release [63.5 kB]
 Hit http://repo.mysql.com trusty InRelease
 Ign http://apt.newrelic.com newrelic InRelease
 Hit http://oss.oracle.com unstable/main i386 Packages
 Hit http://oss.oracle.com unstable/non-free i386 Packages
 Get:11 http://oss.oracle.com unstable/main Translation-en_IN
 Ign http://extras.ubuntu.com precise/main Translation-en_IN
 Ign http://extras.ubuntu.com precise/main Translation-en
 Get:12 http://archive.ubuntu.com trusty-proposed Release [211 kB]
 Get:13 http://security.ubuntu.com trusty-security/universe amd64 Packages [89.7 kB]
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Get:14 http://us.archive.ubuntu.com precise-updates Release [196 kB]
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Get:15 http://www.apache.org 21x InRelease [3,167 B]
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Err http://oss.oracle.com unstable/main amd64 Packages
  HttpError404
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Err http://oss.oracle.com unstable/non-free amd64 Packages
  HttpError404
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Ign http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://mirror.stshosting.co.uk precise/main amd64 Packages
 Ign http://oss.oracle.com unstable/main Translation-en
 Hit http://mirror.stshosting.co.uk precise/main i386 Packages
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN
 Ign http://oss.oracle.com unstable/non-free Translation-en
 Hit http://downloads-distro.mongodb.org dist Release.gpg
 Hit http://repo.mysql.com trusty/mysql-5.6 Sources
 Hit http://repo.mysql.com trusty/mysql-5.6 amd64 Packages
 Hit http://repo.mysql.com trusty/mysql-5.6 i386 Packages
 Hit http://archive.ubuntu.com trusty-backports Release
 Hit http://archive.ubuntu.com trusty/main Sources
 Hit http://archive.ubuntu.com trusty/universe Sources
 Hit http://archive.ubuntu.com trusty/restricted Sources
 Hit http://archive.ubuntu.com trusty/multiverse Sources
 Hit http://archive.ubuntu.com trusty/main amd64 Packages
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty/universe i386 Packages
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages
 Get:16 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:17 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [3,459 B]
 Hit http://us.archive.ubuntu.com precise-backports Release
 Hit http://archive.ubuntu.com trusty/main Translation-en
 Get:18 http://security.ubuntu.com trusty-security/main amd64 Packages [251 kB]
 Hit http://us.archive.ubuntu.com precise/main Sources
 Hit http://us.archive.ubuntu.com precise/restricted Sources
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise/universe Sources
 Hit http://us.archive.ubuntu.com precise/multiverse Sources
 Hit http://archive.ubuntu.com trusty/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty/universe Translation-en
 Hit http://us.archive.ubuntu.com precise/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/restricted i386 Packages
 Get:19 http://archive.ubuntu.com trusty-updates/universe amd64 Packages [260 kB]
 Hit http://us.archive.ubuntu.com precise/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise/main Translation-en
 Hit http://apt.newrelic.com newrelic Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Get:20 http://ppa.launchpad.net trusty Release.gpg [316 B]
 Hit http://us.archive.ubuntu.com precise/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise/restricted Translation-en
 Get:21 http://www.apache.org 21x/main amd64 Packages [698 B]
 Get:22 http://www.apache.org 21x/main i386 Packages [698 B]
 Hit http://us.archive.ubuntu.com precise/universe Translation-en
 Get:23 http://us.archive.ubuntu.com precise-security/main Sources [125 kB]
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://downloads-distro.mongodb.org dist Release
 Get:24 http://security.ubuntu.com trusty-security/universe i386 Packages [89.6 kB]
 Get:25 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:26 http://security.ubuntu.com trusty-security/multiverse i386 Packages [3,628 B]
 Get:27 http://security.ubuntu.com trusty-security/main i386 Packages [241 kB]
 Hit http://apt.newrelic.com newrelic Release
 Hit http://ppa.launchpad.net trusty Release
 Get:28 http://ppa.launchpad.net trusty Release [15.1 kB]
 Get:29 http://us.archive.ubuntu.com precise-security/restricted Sources [3,759 B]
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Get:30 http://us.archive.ubuntu.com precise-security/universe Sources [34.2 kB]
 Hit http://downloads-distro.mongodb.org dist/10gen amd64 Packages
 Hit http://downloads-distro.mongodb.org dist/10gen i386 Packages
 Get:31 http://us.archive.ubuntu.com precise-security/multiverse Sources [1,815 B]
 Get:32 http://us.archive.ubuntu.com precise-security/main amd64 Packages [492 kB]
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Get:33 http://ppa.launchpad.net trusty/main amd64 Packages [3,376 B]
 Get:34 http://ppa.launchpad.net trusty/main i386 Packages [3,376 B]
 Get:35 http://ppa.launchpad.net trusty/main Translation-en [1,556 B]
 Get:36 http://archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:37 http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.2 kB]
 Get:38 http://archive.ubuntu.com trusty-updates/main amd64 Packages [488 kB]
 Get:39 http://us.archive.ubuntu.com precise-security/restricted amd64 Packages [8,943 B]
 Get:40 http://us.archive.ubuntu.com precise-security/universe amd64 Packages [108 kB]
 Ign http://mirror.stshosting.co.uk precise/main Translation-en_IN
 Get:41 http://us.archive.ubuntu.com precise-security/multiverse amd64 Packages [2,463 B]
 Get:42 http://us.archive.ubuntu.com precise-security/main i386 Packages [531 kB]
 Ign http://mirror.stshosting.co.uk precise/main Translation-en
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en_IN
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en
 Ign http://www.apache.org 21x/main Translation-en_IN
 Ign http://www.apache.org 21x/main Translation-en
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en_IN
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Get:43 http://us.archive.ubuntu.com precise-security/restricted i386 Packages [8,939 B]
 Get:44 http://us.archive.ubuntu.com precise-security/universe i386 Packages [116 kB]
 Get:45 http://us.archive.ubuntu.com precise-security/multiverse i386 Packages [2,652 B]
 Hit http://us.archive.ubuntu.com precise-security/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-security/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-security/universe Translation-en
 Get:46 http://us.archive.ubuntu.com precise-updates/main Sources [487 kB]
 Get:47 http://us.archive.ubuntu.com precise-updates/restricted Sources [7,981 B]
 Get:48 http://us.archive.ubuntu.com precise-updates/universe Sources [112 kB]
 Get:49 http://us.archive.ubuntu.com precise-updates/multiverse Sources [9,417 B]
 Get:50 http://us.archive.ubuntu.com precise-updates/main amd64 Packages [884 kB]
 Get:51 http://us.archive.ubuntu.com precise-updates/restricted amd64 Packages [13.6 kB]
 Get:52 http://us.archive.ubuntu.com precise-updates/universe amd64 Packages [255 kB]
 Get:53 http://us.archive.ubuntu.com precise-updates/multiverse amd64 Packages [16.4 kB]
 Get:54 http://us.archive.ubuntu.com precise-updates/main i386 Packages [922 kB]
 Get:55 http://archive.ubuntu.com trusty-updates/universe i386 Packages [262 kB]
 Get:56 http://archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:57 http://archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.3 kB]
 Get:58 http://archive.ubuntu.com trusty-updates/main i386 Packages [477 kB]
 Get:59 http://us.archive.ubuntu.com precise-updates/restricted i386 Packages [13.6 kB]
 Get:60 http://us.archive.ubuntu.com precise-updates/universe i386 Packages [264 kB]
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en
 Get:61 http://archive.ubuntu.com trusty-proposed/universe amd64 Packages [26.4 kB]
 Get:62 http://archive.ubuntu.com trusty-proposed/restricted amd64 Packages [28 B]
 Get:63 http://archive.ubuntu.com trusty-proposed/multiverse amd64 Packages [1,134 B]
 Get:64 http://archive.ubuntu.com trusty-proposed/main amd64 Packages [154 kB]
 Get:65 http://us.archive.ubuntu.com precise-updates/multiverse i386 Packages [16.6 kB]
 Hit http://us.archive.ubuntu.com precise-updates/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/universe Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/main Sources
 Hit http://us.archive.ubuntu.com precise-backports/restricted Sources
 Hit http://us.archive.ubuntu.com precise-backports/universe Sources
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Sources
 Hit http://us.archive.ubuntu.com precise-backports/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted i386 Packages
 Get:66 http://archive.ubuntu.com trusty-proposed/universe i386 Packages [26.4 kB]
 Hit http://us.archive.ubuntu.com precise-backports/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse i386 Packages
 Get:67 http://archive.ubuntu.com trusty-proposed/restricted i386 Packages [28 B]
 Hit http://us.archive.ubuntu.com precise-backports/main Translation-en
 Get:68 http://archive.ubuntu.com trusty-proposed/multiverse i386 Packages [1,133 B]
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/universe Translation-en
 Get:69 http://archive.ubuntu.com trusty-proposed/main i386 Packages [150 kB]
 Hit http://archive.ubuntu.com trusty-proposed/main Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/multiverse Translation-en
 Ign http://us.archive.ubuntu.com precise/main Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/multiverse Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/restricted Translation-en_IN
 Hit http://archive.ubuntu.com trusty-proposed/restricted Translation-en
 Ign http://us.archive.ubuntu.com precise/universe Translation-en_IN
 Hit http://archive.ubuntu.com trusty-proposed/universe Translation-en
 Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-backports/universe Translation-en
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 7,641 kB in 10min 18s (12.4 kB/s)
 Temp File /tmp/ptconfigure-temp-script-68300758613.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
   cabextract fonts-horai-umefont libasn1-8-heimdal:i386 libexif12:i386
  libgd3:i386 libgif4:i386 libgphoto2-6:i386 libgphoto2-port10:i386
  libgssapi3-heimdal:i386 libgstreamer-plugins-base0.10-0:i386
  libgstreamer0.10-0:i386 libhcrypto4-heimdal:i386 libheimbase1-heimdal:i386
  libheimntlm0-heimdal:i386 libhx509-5-heimdal:i386 libieee1284-3:i386
  libkrb5-26-heimdal:i386 liblcms2-2:i386 libldap-2.4-2:i386 libltdl7:i386
  libmpg123-0 libmpg123-0:i386 libodbc1 libp11-kit-gnome-keyring:i386
  libroken18-heimdal:i386 libsane:i386 libsasl2-2:i386
  libsasl2-modules-db:i386 libusb-1.0-0:i386 libv4l-0:i386 libv4lconvert0:i386
  libvpx1:i386 libwind0-heimdal:i386 libxcomposite1:i386 libxcursor1:i386
  libxinerama1:i386 libxpm4:i386 libxrandr2:i386 odbcinst odbcinst1debian2
  wine-gecko2.21
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
   libopts25 ntp python-support
 Suggested packages:
  cassandra-tools ntp-doc
 The following NEW packages will be installed:
  cassandra libopts25 ntp python-support
 0 upgraded, 4 newly installed, 0 to remove and 16 not upgraded.
 Need to get 19.2 MB of archives.
 After this operation, 23.0 MB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main libopts25 amd64 1:5.18-2ubuntu2 [55.3 kB]
 Get:2 http://security.ubuntu.com/ubuntu/ trusty-security/main ntp amd64 1:4.2.6.p5+dfsg-3ubuntu2.14.04.2 [418 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/universe python-support all 1.0.15 [26.7 kB]
 Get:4 http://www.apache.org/dist/cassandra/debian/ 21x/main cassandra all 2.1.3 [18.7 MB]
 Fetched 19.2 MB in 7min 10s (44.5 kB/s)
 Selecting previously unselected package libopts25:amd64.
 (Reading database ... 363575 files and directories currently installed.)
 Preparing to unpack .../libopts25_1%3a5.18-2ubuntu2_amd64.deb ...
 Unpacking libopts25:amd64 (1:5.18-2ubuntu2) ...
 Selecting previously unselected package ntp.
 Preparing to unpack .../ntp_1%3a4.2.6.p5+dfsg-3ubuntu2.14.04.2_amd64.deb ...
 Unpacking ntp (1:4.2.6.p5+dfsg-3ubuntu2.14.04.2) ...
 Selecting previously unselected package python-support.
 Preparing to unpack .../python-support_1.0.15_all.deb ...
 Unpacking python-support (1.0.15) ...
 Selecting previously unselected package cassandra.
 Preparing to unpack .../cassandra_2.1.3_all.deb ...
 Unpacking cassandra (2.1.3) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up libopts25:amd64 (1:5.18-2ubuntu2) ...
 Setting up ntp (1:4.2.6.p5+dfsg-3ubuntu2.14.04.2) ...
 * Starting NTP server ntpd
   ...done.
 Setting up python-support (1.0.15) ...
 Setting up cassandra (2.1.3) ...
 Adding group `cassandra' (GID 138) ...
 Done.
 vm.max_map_count = 1048575
 net.ipv4.tcp_keepalive_time = 300
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for python-support (1.0.15) ...
 [Pharaoh Logging] Adding Package cassandra from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Cassandra: Success
 ------------------------------
 Installer Finished
 ****************************** 


オプション
-----------------

.. cssclass:: table-bordered

 +-------------------------------+---------------------------------------------+-------------+---------------------------------------+
 | パラメータ                    | 代替パラメータ                              | オプション  | 注釈                                  |
 +===============================+=============================================+=============+=======================================+
 |ptconfigure cassandra Install  | コマンドラインで使用することができる2つの   | Y           | システムは、インストールプロセスを開  |
 |                               | 別のパラメータがある。Cassandra , cassandra |             | 始します                              |
 |                               | 例えば：ptconfigure cassandra install,      |             |                                       |
 |                               | ptconfigure Cassandra install               |             |                                       |
 +-------------------------------+---------------------------------------------+-------------+---------------------------------------+
 |ptconfigure cassandra Install  | コマンドラインで使用することができる2つの   | N           | システムは、インストール·プロセス     |
 |                               | 別のパラメータがある。Cassandra , cassandra |             | を停止し、                            |
 |                               | 例えば：ptconfigure cassandra install,      |             |                                       |
 |                               | ptconfigure Cassandra install|              |             |                                       |
 +-------------------------------+---------------------------------------------+-------------+---------------------------------------+


メリット
------------

* 分権 – クラスタ内のすべてのノードが同じ役割を持っています。単一障害点があ りません。データは、クラスター（ので、各ノードは異なるデータを含む）   に分散されますが、すべての要求にサービスを提供することができ、すべてのノードと全くマスターはありません。-
* 複製およびマルチデータセンターのレプリケーションをサポート - レプリケーション戦略は設定可能です。カサンドラは、複数のデータセンター間で、多数   のノードを展開するために、分散システムとして設計されている。カサンドラの分散アーキテクチャの主な機能は、
  具体的にフェールオーバーおよび災害復旧   のために、冗長性を確保するため、複数データセンターの展開に合わせて調整されている。
* スケーラビリティ - 読み、スループット、新しいマシンがアプリケーションへのダウンタイムなしまたは中断、追加された直線的に、両方の増加を書きます
* フォールトトレラント - データは、自動的にフォールトトレランスのために複数のノードに複製されます。複数のデータセンター間のレプリケーションがサ   ポートされています。失敗したノードは、ダウンタイムなしで置き換えることができる。
* 調整可能な一貫性 - 書き込み、一貫性の調整可能なレベルを提供読み込み、からのすべての方法は、真ん中の定足数レベルで、「すべてのレプリカのための   ブロック読み出しを可能にするには」を「失敗することはありません書き込み」。
