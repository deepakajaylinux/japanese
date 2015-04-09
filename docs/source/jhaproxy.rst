===========
HAProxy
===========


あらすじ
-------------

HAProxy はフリー、オープン ソースの高可用性ソリューションでは、TCP および HTTP ベースのアプリケーションの複数のサーバー要求を広めることで負荷分散とプロキシを提供することです。高速かつ (プロセッサとメモリの使用量） の面で効率的であるという評判をしています。

ヘルプ コマンド
----------------------

このコマンドは HAProxy モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドは、エンド ユーザー ガイドをいつ、どのように知っているに使用されるコマンドです。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        ptconfigure HAproxy help



上記のコマンドの絵の表現は以下します。

.. code-block:: bash


 kevell@corp:/# ptconfigure HAProxy help

 ******************************


  This module provides installs HA Proxy Server

  HAProxy, ha-proxy, haproxy

        - install
        Installs HA Proxy Server
        example: ptconfigure haproxy install

        - configure
        Configure Load Balancing with HA Proxy Server
        example: ptconfigure haproxy configure

 ------------------------------
 End Help
 ******************************




インストール
----------------

私たちのディストリビューションのパッケージ マネージャーを使用して HAProxy をインストールできます。とき、ユーザーはマシンで HAproxy モジュールをインストールする必要があります。特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash
        
	        ptconfigure HAproxy install

上記のコマンドの絵の表現は以下します。



.. code-block:: bash

 
 kevell@corp:/# ptconfigure haproxy install
 Install HA Proxy Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *       HA Proxy Server!      *
 *******************************
 Creating /tmp/ptconfigure-temp-script-25680166743.sh
 chmod 755 /tmp/ptconfigure-temp-script-25680166743.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-25680166743.sh Permissions
 Executing /tmp/ptconfigure-temp-script-25680166743.sh
 gpg: keyring `/tmp/tmpxs_xtdw1/secring.gpg' created
 gpg: keyring `/tmp/tmpxs_xtdw1/pubring.gpg' created
 gpg: requesting key 1C61B9CD from hkp server keyserver.ubuntu.com
 gpg: /tmp/tmpxs_xtdw1/trustdb.gpg: trustdb created
 gpg: key 1C61B9CD: public key "Launchpad PPA for Vincent Bernat" imported
 gpg: Total number processed: 1
 gpg:               imported: 1  (RSA: 1)
 OK
 Ign http://dl.google.com stable InRelease
 Ign http://archive.ubuntu.com trusty InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://archive.canonical.com precise InRelease
 Ign http://extras.ubuntu.com precise InRelease
 Ign http://archive.ubuntu.com trusty-updates InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://dl.hhvm.com trusty InRelease
 Hit http://downloads.hipchat.com stable InRelease
 Ign http://us.archive.ubuntu.com precise InRelease
 Hit http://security.ubuntu.com trusty-security Release.gpg
 Hit http://archive.canonical.com precise Release.gpg
 Hit http://extras.ubuntu.com precise Release.gpg
 Ign http://archive.ubuntu.com trusty-proposed InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://us.archive.ubuntu.com precise-security InRelease
 Hit http://downloads.hipchat.com stable/main amd64 Packages
 Hit http://security.ubuntu.com trusty-security Release
 Ign http://packages.dotdeb.org squeeze InRelease
 Hit http://archive.canonical.com precise Release
 Hit http://extras.ubuntu.com precise Release
 Ign http://archive.ubuntu.com trusty-backports InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://us.archive.ubuntu.com precise-updates InRelease
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Hit http://downloads.hipchat.com stable/main i386 Packages
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Hit http://archive.ubuntu.com trusty Release.gpg
 Hit http://security.ubuntu.com trusty-security/universe amd64 Packages
 Ign http://us.archive.ubuntu.com precise-backports InRelease
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://archive.canonical.com precise/partner Sources
 Hit http://extras.ubuntu.com precise/main Sources
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://archive.ubuntu.com trusty-updates Release.gpg
 Hit http://mirror.stshosting.co.uk precise InRelease
 Hit http://us.archive.ubuntu.com precise Release.gpg
 Hit http://security.ubuntu.com trusty-security/restricted amd64 Packages
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://archive.canonical.com precise/partner amd64 Packages
 Hit http://extras.ubuntu.com precise/main amd64 Packages
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://archive.ubuntu.com trusty-proposed Release.gpg
 Hit http://us.archive.ubuntu.com precise-security Release.gpg
 Hit http://packages.elasticsearch.org stable Release.gpg
 Hit http://security.ubuntu.com trusty-security/multiverse amd64 Packages
 Hit http://archive.canonical.com precise/partner i386 Packages
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Hit http://extras.ubuntu.com precise/main i386 Packages
 Hit http://archive.ubuntu.com trusty-backports Release.gpg
 Hit http://us.archive.ubuntu.com precise-updates Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Hit http://security.ubuntu.com trusty-security/main amd64 Packages
 Hit http://archive.ubuntu.com trusty Release
 Ign http://downloads-distro.mongodb.org dist InRelease
 Hit http://us.archive.ubuntu.com precise-backports Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Hit http://repo.mysql.com trusty InRelease
 Hit http://security.ubuntu.com trusty-security/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-updates Release
 Hit http://us.archive.ubuntu.com precise Release
 Hit http://packages.elasticsearch.org stable Release
 Hit http://security.ubuntu.com trusty-security/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed Release
 Ign http://archive.canonical.com precise/partner Translation-en
 Hit http://us.archive.ubuntu.com precise-security Release
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Ign http://apt.newrelic.com newrelic InRelease
 Hit http://archive.ubuntu.com trusty-backports Release
 Hit http://security.ubuntu.com trusty-security/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates Release
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://archive.ubuntu.com trusty/main Sources
 Hit http://security.ubuntu.com trusty-security/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports Release
 Hit http://archive.ubuntu.com trusty/universe Sources
 Get:1 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Hit http://us.archive.ubuntu.com precise/main Sources
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://archive.ubuntu.com trusty/restricted Sources
 Hit http://us.archive.ubuntu.com precise/restricted Sources
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://archive.ubuntu.com trusty/multiverse Sources
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Hit http://us.archive.ubuntu.com precise/universe Sources
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://archive.ubuntu.com trusty/main amd64 Packages
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://us.archive.ubuntu.com precise/multiverse Sources
 Ign http://downloads.hipchat.com stable/main Translation-en_IN
 Hit http://dl.google.com stable Release.gpg
 Hit http://archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Hit http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Hit http://us.archive.ubuntu.com precise/main amd64 Packages
 Ign http://downloads.hipchat.com stable/main Translation-en
 Hit http://archive.ubuntu.com trusty/restricted amd64 Packages
 Ign http://extras.ubuntu.com precise/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise/restricted amd64 Packages
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Ign http://extras.ubuntu.com precise/main Translation-en
 Get:2 http://oss.oracle.com unstable/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Hit http://archive.ubuntu.com trusty/main i386 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://us.archive.ubuntu.com precise/multiverse amd64 Packages
 Ign http://oss.oracle.com unstable/main i386 Packages/DiffIndex
 Hit http://archive.ubuntu.com trusty/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise/main i386 Packages
 Hit http://archive.ubuntu.com trusty/restricted i386 Packages
 Ign http://oss.oracle.com unstable/non-free i386 Packages/DiffIndex
 Hit http://us.archive.ubuntu.com precise/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise/universe i386 Packages
 Hit http://archive.ubuntu.com trusty/main Translation-en
 Hit http://us.archive.ubuntu.com precise/multiverse i386 Packages
 Get:3 http://www.apache.org 21x InRelease [3,167 B]
 Hit http://archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise/main Translation-en
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://archive.ubuntu.com trusty/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise/multiverse Translation-en
 Hit http://mirror.stshosting.co.uk precise/main amd64 Packages
 Hit http://oss.oracle.com unstable/main i386 Packages
 Hit http://mirror.stshosting.co.uk precise/main i386 Packages
 Hit http://oss.oracle.com unstable/non-free i386 Packages
 Hit http://archive.ubuntu.com trusty/universe Translation-en
 Hit http://us.archive.ubuntu.com precise/restricted Translation-en
 Get:4 http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-updates/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise/universe Translation-en
 Hit http://archive.ubuntu.com trusty-updates/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security/main Sources
 Hit http://downloads-distro.mongodb.org dist Release.gpg
 Hit http://archive.ubuntu.com trusty-updates/main amd64 Packages
 Hit http://repo.mysql.com trusty/mysql-5.6 Sources
 Hit http://us.archive.ubuntu.com precise-security/restricted Sources
 Hit http://archive.ubuntu.com trusty-updates/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/universe Sources
 Hit http://archive.ubuntu.com trusty-updates/restricted i386 Packages
 Hit http://repo.mysql.com trusty/mysql-5.6 amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security/multiverse Sources
 Hit http://us.archive.ubuntu.com precise-security/main amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/multiverse i386 Packages
 Hit http://repo.mysql.com trusty/mysql-5.6 i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/restricted amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/main i386 Packages
 Hit http://archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/universe amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-security/multiverse amd64 Packages
 Hit http://archive.ubuntu.com trusty-updates/restricted Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-security/main i386 Packages
 Hit http://archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://us.archive.ubuntu.com precise-security/restricted i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security/multiverse i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-proposed/restricted amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/main Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-security/multiverse Translation-en
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-proposed/main amd64 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://us.archive.ubuntu.com precise-security/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-security/universe Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-proposed/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/main Sources
 Err http://oss.oracle.com unstable/main amd64 Packages
   HttpError404
 Hit http://archive.ubuntu.com trusty-proposed/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/restricted Sources
 Err http://oss.oracle.com unstable/non-free amd64 Packages
   HttpError404
 Hit http://archive.ubuntu.com trusty-proposed/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/universe Sources
 Hit http://apt.newrelic.com newrelic Release.gpg
 Ign http://oss.oracle.com unstable/main Translation-en_IN
 Hit http://archive.ubuntu.com trusty-proposed/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Sources
 Ign http://oss.oracle.com unstable/main Translation-en
 Hit http://archive.ubuntu.com trusty-proposed/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/main amd64 Packages
 Ign http://oss.oracle.com unstable/non-free Translation-en_IN
 Hit http://archive.ubuntu.com trusty-proposed/universe Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/restricted amd64 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Ign http://oss.oracle.com unstable/non-free Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/universe amd64 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise-updates/multiverse amd64 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://dl.google.com stable Release
 Hit http://archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-updates/main i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise-updates/restricted i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/universe i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/multiverse i386 Packages
 Hit http://archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-updates/main Translation-en
 Hit http://archive.ubuntu.com trusty-backports/main i386 Packages
 Get:5 http://www.apache.org 21x/main amd64 Packages [704 B]
 Hit http://us.archive.ubuntu.com precise-updates/multiverse Translation-en
 Hit http://archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/restricted Translation-en
 Hit http://archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://us.archive.ubuntu.com precise-updates/universe Translation-en
 Hit http://archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://us.archive.ubuntu.com precise-backports/main Sources
 Hit http://archive.ubuntu.com trusty-backports/universe Translation-en
 Get:6 http://www.apache.org 21x/main i386 Packages [704 B]
 Hit http://us.archive.ubuntu.com precise-backports/restricted Sources
 Hit http://us.archive.ubuntu.com precise-backports/universe Sources
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Sources
 Hit http://us.archive.ubuntu.com precise-backports/main amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com precise-backports/main i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/restricted i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/universe i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com precise-backports/main Translation-en
 Ign http://archive.ubuntu.com trusty/main Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-backports/multiverse Translation-en
 Ign http://archive.ubuntu.com trusty/multiverse Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-backports/restricted Translation-en
 Ign http://archive.ubuntu.com trusty/restricted Translation-en_IN
 Hit http://us.archive.ubuntu.com precise-backports/universe Translation-en
 Ign http://archive.ubuntu.com trusty/universe Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/main Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/multiverse Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/restricted Translation-en_IN
 Ign http://us.archive.ubuntu.com precise/universe Translation-en_IN
 Hit http://downloads-distro.mongodb.org dist Release
 Hit http://apt.newrelic.com newrelic Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://ppa.launchpad.net trusty Release
 Hit http://dl.google.com stable/main amd64 Packages
 Hit http://dl.google.com stable/main i386 Packages
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://downloads-distro.mongodb.org dist/10gen amd64 Packages
 Hit http://downloads-distro.mongodb.org dist/10gen i386 Packages
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Ign http://dl.hhvm.com trusty/main Translation-en
 Ign http://mirror.stshosting.co.uk precise/main Translation-en_IN
 Ign http://mirror.stshosting.co.uk precise/main Translation-en
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en_IN
 Ign http://repo.mysql.com trusty/mysql-5.6 Translation-en
 Ign http://www.apache.org 21x/main Translation-en_IN
 Ign http://www.apache.org 21x/main Translation-en
 Ign http://dl.google.com stable/main Translation-en_IN
 Ign http://dl.google.com stable/main Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en_IN
 Ign http://downloads-distro.mongodb.org dist/10gen Translation-en
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Fetched 4,764 B in 1min 38s (48 B/s)
 Temp File /tmp/ptconfigure-temp-script-25680166743.sh Removed 

 Configuration file '/etc/default/haproxy'
 ==> Modified (by you or by a script) since installation.
 ==> Package distributor has shipped an updated version.
   What would you like to do about it ?  Your options are:
    Y or I  : install the package maintainer's version
    N or O  : keep your currently-installed version
      D     : show the differences between the versions
      Z     : start a shell to examine the situation
 The default action is to keep your current version.
 *** haproxy (Y/I/N/O/D/Z) [default=N] ? Y
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
   vim-haproxy haproxy-doc
 The following NEW packages will be installed:
   haproxy
 0 upgraded, 1 newly installed, 0 to remove and 13 not upgraded.
 Need to get 550 kB of archives.
 After this operation, 1,223 kB of additional disk space will be used.
 Get:1 http://ppa.launchpad.net/vbernat/haproxy-1.5/ubuntu/ trusty/main haproxy amd64 1.5.11-1ppa1~trusty [550 kB]
 Fetched 550 kB in 10s (51.4 kB/s)
 Selecting previously unselected package haproxy.
 (Reading database ... 401696 files and directories currently installed.)
 Preparing to unpack .../haproxy_1.5.11-1ppa1~trusty_amd64.deb ...
 Unpacking haproxy (1.5.11-1ppa1~trusty) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up haproxy (1.5.11-1ppa1~trusty) ...
 Installing new version of config file /etc/haproxy/haproxy.cfg ...
 Installing new version of config file /etc/default/haproxy ...
 Installing new version of config file /etc/init.d/haproxy ...
  * Starting haproxy haproxy
   ...done.
 Processing triggers for ureadahead (0.100.0-16) ...
 [Pharaoh Logging] Adding Package haproxy from the Packager Apt executed correctly
 HA Proxy Init script config file /etc/default/haproxy added
 [Pharaoh Logging] Restarting haproxy service
  * Restarting haproxy haproxy
    ...done.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 HAProxy: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
-----------                               


.. cssclass:: table-bordered


 +-----------------------------+---------------------------------+---------------+--------------------------------------------------+
 | パラメーター                | 代替パラメーター                | オプション    | コメント                                         |
 +=============================+=================================+===============+==================================================+
 |ptconfigure HAProxy Install  | HAProxy , ha-proxy, haproxy     | Y(Yes)        | システムは、インストールプロセスを開始します     |
 +-----------------------------+---------------------------------+---------------+--------------------------------------------------+
 |ptconfigure HAProxy Install  | HAProxy , ha-proxy, haproxy     | N(No)         | システムは、インストール·プロセスを停止し、|     |
 +-----------------------------+---------------------------------+---------------+--------------------------------------------------+
      



構成
--------------------

このコマンドは HAproxy サーバーと分散負荷を構成するに役立ちます。一度、下特定のコマンドが実行されるシステムが提供する各セクションの既定値を任意に変更が行われる場合、ユーザー データを提供できます。


.. code-block:: bash

                ptconfigure HAproxy configure


上記のコマンドのスクリーン ショットは以下します。

.. code-block:: bash


 kevvell@corp:/# ptconfigure haproxy configure
 ********************************************
 *******************************
 *        Pharaoh Tools        *
 *       HA Proxy Server!      *
 *******************************
 [Pharaoh Logging] No environment name provided for Load Balancing
 What is the environment name you want to balance load to? 
 kevell
 
 Set non-default value for global_log? Default is 127.0.0.1 local0 notice (Y/N) 
 y
 What value for global_log? 
 127.0.0.0
 Set non-default value for global_maxconn? Default is 20000 (Y/N) 
 n
 Set non-default value for global_user? Default is haproxy (Y/N) 
 n
 Set non-default value for global_group? Default is haproxy (Y/N) 
 n
 Set non-default value for defaults_log? Default is global (Y/N) 
 n
 Set non-default value for defaults_mode? Default is http (Y/N) 
 n
 Set non-default value for defaults_option_string? Default is option dontlognull
 option redispatch (Y/N) 
 n
 Set non-default value for defaults_retries? Default is 3 (Y/N) 
 y
 What value for defaults_retries?
 5
 Set non-default value for defaults_timeout_connect? Default is 5000 (Y/N) 
 y
 What value for defaults_timeout_connect?
 2000
 Set non-default value for defaults_timeout_client? Default is 10000 (Y/N) 
 y
 What value for defaults_timeout_client?
 1000
 Set non-default value for defaults_timeout_server? Default is 10000 (Y/N) 
 y
 What value for defaults_timeout_server?
 1000
 Set non-default value for listen_appname? Default is appname (Y/N) 
 n
 Set non-default value for listen_ip_port? Default is 0.0.0.0:80 (Y/N) 
 y
 What value for listen_ip_port?
 127.0.0.1:80
 Set non-default value for listen_mode? Default is http (Y/N) 
 n
 Set non-default value for listen_balance? Default is roundrobin (Y/N) 
 n
 Set non-default value for listen_option_string? Default is option httpclose
 option forwardfor (Y/N) 
 n
 Set non-default value for listen_server_string? Default is server  192.168.1.7: check
 (Y/N) 
 y
 What value for listen_server_string?
 kevvell
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 HA Proxy Server: Success
 ------------------------------
 Installer Finished
 ******************************




利点
--------------

* すべてのアプリケーション 1 つの単一の ip アドレス経由でクラスターにアクセスします。HAProxy の背後に隠されたデータベース クラスターのトポロジ。
* それは、アプリケーションを変更せずにデータベース ノードを追加することが可能です。
* (MySQL にて) データベース接続の最大数に達すると、HAProxy キュー新しい接続を追加します。これは制限のきちんとした方法です。
  データベース接続を要求し、過負荷保護を実現します。
 
