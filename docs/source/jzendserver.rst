============
Zend Server
============

概要
-------------

プライベート、パブリック、ハイブリッド - のZend Serverは、より高速なPHPアプリケーションを実行し、オンプレミスまたはクラウドでより良い拡張するために設計されたアプリケーションプラットフォームです。

ZendのServerは、サーバー上にデプロイすることができ、より高品質なアプリケーションを作成するための開発プラットフォームとして利用可能です。と高いパフォーマンスと拡張性を必要とするミッションクリティカルなアプリケーションを実行するための生産プラットフォーム。

ZendのServerは、アプリケーションデリバリサイクル全体の一貫性、自動化とコラボレーション機能を提供して連続的送達を、可能にするプラットフォームです。それは、信頼性、パフォーマンスと高レベルのセキュリティを必要とするPHPアプリケーションを実行し、管理するための完全な、オラクルが有効になって、エンタープライズ対応のWebアプリケーションサーバです。


helpコマンド
----------------------

このコマンドは、Zendのサーバモジュールの使用状況を判断するのに役立ちます。ユーザーは、このモジュールを実行する別の方法/形式について知って来る。このコマンドは、このコマンドの目的を知ることが、エンドユーザーをガイドします。与えられた以下のコマンドと同じのスクリーンショットである。

 
.. code-block:: bash 
       
       	ptconfigure zendserver help 

上記のコマンドの絵画表現は、以下に記載されている

 
.. code-block:: bash 

 kevell@corp:/# ptconfigure ZendServer help 

 ****************************** 
  This command allows you to update ZendServer. 

  ZendServer, zendserver, Zendserver 
	 
	- install 
	Installs the latest version of ZendServer 
	example: ptconfigure zendserver install 

 ------------------------------ 
 End Help 
 ****************************** 

インストール
----------------

このコマンドは、システムにzendserverインストールするのに役立ちます。場合には、システム内で既に利用可能zendserverこのコマンドは、バージョンを更新した場合。以下のコマンドは、インストールのプロセスを実行します。

 
.. code-block:: bash 
        
        ptconfigure zendserver install 

上記のコマンドの絵画表現は、以下に記載されている


 
.. code-block:: bash 

 kevell@corp:/# ptconfigure ZendServer install 
 Install ZendServer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         ZendServer!        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-65684868988.sh 
 chmod 755 /tmp/ptconfigure-temp-script-65684868988.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-65684868988.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-65684868988.sh 
 --2015-01-28 12:32:03--  http://repos.zend.com/zend.key 
 Resolving repos.zend.com (repos.zend.com)... 175.41.7.3, 175.41.7.4 
 Connecting to repos.zend.com (repos.zend.com)|175.41.7.3|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 1673 (1.6K) [application/pgp-keys] 
 Saving to: â€˜STDOUTâ€™ 

 100%[=======================================================================================================>] 1,673       --.-K/s   in 0.002s  

 2015-01-28 12:32:03 (736 KB/s) - written to stdout [1673/1673] 
 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main amd64 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://debian.datastax.com/community/ stable/main i386 Packages (/var/lib/apt/lists/debian.datastax.com_community_dists_stable_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main amd64 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main amd64 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main amd64 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main amd64 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main amd64 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main i386 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main i386 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main i386 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main i386 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://www.apache.org/dist/cassandra/debian/ 21x/main i386 Packages (/var/lib/apt/lists/www.apache.org_dist_cassandra_debian_dists_21x_main_binary-i386_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all amd64 Packages (/var/lib/apt/lists/packages.dotdeb.org_dists_squeeze_all_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages) 
 W: Duplicate sources.list entry http://packages.dotdeb.org/ squeeze/all i386 Packages (/var/lib/apt/lists/packages.dotdeb.org_dists_squeeze_all_binary-i386_Packages) 
 W: Duplicate sources.list entry http://apt.newrelic.com/debian/ newrelic/non-free amd64 Packages (/var/lib/apt/lists/apt.newrelic.com_debian_dists_newrelic_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://apt.newrelic.com/debian/ newrelic/non-free amd64 Packages (/var/lib/apt/lists/apt.newrelic.com_debian_dists_newrelic_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://apt.newrelic.com/debian/ newrelic/non-free amd64 Packages (/var/lib/apt/lists/apt.newrelic.com_debian_dists_newrelic_non-free_binary-amd64_Packages) 
 W: Duplicate sources.list entry http://apt.newrelic.com/debian/ newrelic/non-free i386 Packages (/var/lib/apt/lists/apt.newrelic.com_debian_dists_newrelic_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://apt.newrelic.com/debian/ newrelic/non-free i386 Packages (/var/lib/apt/lists/apt.newrelic.com_debian_dists_newrelic_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry http://apt.newrelic.com/debian/ newrelic/non-free i386 Packages (/var/lib/apt/lists/apt.newrelic.com_debian_dists_newrelic_non-free_binary-i386_Packages) 
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages) 
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages) 
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages) 
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages) 
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages) 
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages) 
 W: You may want to run apt-get update to correct these problems 
 OK 
 Ign http://security.ubuntu.com trusty-security InRelease 
 Get:1 http://security.ubuntu.com trusty-security Release.gpg [933 B] 
 Get:2 http://security.ubuntu.com trusty-security Release [62.0 kB] 
 Get:3 http://security.ubuntu.com trusty-security/main Sources [64.8 kB] 
 Get:4 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B] 
 Hit http://www.apache.org 21x InRelease 
 Ign http://in.archive.ubuntu.com trusty InRelease 
 Ign http://extras.ubuntu.com trusty InRelease 
 Hit http://www.apache.org 21x/main amd64 Packages 
 Get:5 http://security.ubuntu.com trusty-security/universe Sources [17.4 kB] 
 Hit http://extras.ubuntu.com trusty Release.gpg 
 Ign http://in.archive.ubuntu.com trusty-updates InRelease 
 Hit http://www.apache.org 21x/main i386 Packages 
 Hit http://extras.ubuntu.com trusty Release 
 Ign http://in.archive.ubuntu.com trusty-backports InRelease 
 Hit http://in.archive.ubuntu.com trusty Release.gpg 
 Hit http://extras.ubuntu.com trusty/main Sources 
 Get:6 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B] 
 Hit http://extras.ubuntu.com trusty/main amd64 Packages 
 Get:7 http://security.ubuntu.com trusty-security/multiverse Sources [723 B] 
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg 
 Hit http://extras.ubuntu.com trusty/main i386 Packages 
 Get:8 http://security.ubuntu.com trusty-security/main amd64 Packages [200 kB] 
 Hit http://in.archive.ubuntu.com trusty Release 
 Ign http://www.apache.org 21x/main Translation-en_IN 
 Get:9 http://in.archive.ubuntu.com trusty-updates Release [62.0 kB] 
 Ign http://www.apache.org 21x/main Translation-en 
 Ign http://repos.zend.com server InRelease 
 Hit http://repos.zend.com server Release.gpg 
 Hit http://downloads.hipchat.com stable InRelease 
 Hit http://repos.zend.com server Release 
 Hit http://repos.zend.com server/non-free amd64 Packages 
 Hit http://downloads.hipchat.com stable/main amd64 Packages 
 Hit http://repos.zend.com server/non-free i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports Release 
 Hit http://in.archive.ubuntu.com trusty/main Sources 
 Hit http://downloads.hipchat.com stable/main i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/restricted Sources 
 Hit http://in.archive.ubuntu.com trusty/universe Sources 
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources 
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages 
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages 
 Ign http://extras.ubuntu.com trusty/main Translation-en 
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages 
 Ign http://repos.zend.com server/non-free Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages 
 Ign http://repos.zend.com server/non-free Translation-en 
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages 
 Hit http://dl.hhvm.com trusty InRelease 
 Ign http://packages.dotdeb.org squeeze InRelease 
 Ign http://debian.datastax.com stable InRelease 
 Hit http://dl.hhvm.com trusty/main amd64 Packages 
 Get:10 http://debian.datastax.com stable Release.gpg [280 B] 
 Hit http://packages.dotdeb.org squeeze Release.gpg 
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages 
 Ign http://downloads.hipchat.com stable/main Translation-en_IN 
 Hit http://dl.hhvm.com trusty/main i386 Packages 
 Ign http://downloads.hipchat.com stable/main Translation-en 
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/main Translation-en 
 Hit http://packages.dotdeb.org squeeze Release 
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en 
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages 
 Get:11 http://debian.datastax.com stable Release [2,870 B] 
 Hit http://packages.dotdeb.org squeeze/all i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en 
 Get:12 http://debian.datastax.com stable/main amd64 Packages [16.2 kB] 
 Ign http://dl.hhvm.com trusty/main Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en 
 Ign http://dl.hhvm.com trusty/main Translation-en 
 Get:13 http://in.archive.ubuntu.com trusty-updates/main Sources [158 kB] 
 Ign http://apt.newrelic.com newrelic InRelease 
 Hit http://apt.newrelic.com newrelic Release.gpg 
 Hit http://apt.newrelic.com newrelic Release 
 Get:14 http://debian.datastax.com stable/main i386 Packages [16.2 kB] 
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages 
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages 
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN 
 Ign http://packages.dotdeb.org squeeze/all Translation-en 
 Get:15 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B] 
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN 
 Ign http://apt.newrelic.com newrelic/non-free Translation-en 
 Ign http://debian.datastax.com stable/main Translation-en_IN 
 Ign http://debian.datastax.com stable/main Translation-en 
 Get:16 https://repo.varnish-cache.org precise InRelease 
 Get:17 http://security.ubuntu.com trusty-security/universe amd64 Packages [85.3 kB] 
 Get:18 https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages 
 Get:19 https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages 
 Get:20 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN 
 Get:21 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,061 B] 
 Get:22 http://in.archive.ubuntu.com trusty-updates/universe Sources [97.6 kB] 
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN 
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en 
 Get:23 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [3,553 B] 
 Get:24 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [406 kB] 
 Get:25 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [1,161 B] 
 Get:26 http://security.ubuntu.com trusty-security/main i386 Packages [190 kB] 
 Get:27 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B] 
 Get:28 http://security.ubuntu.com trusty-security/universe i386 Packages [85.3 kB] 
 Get:29 http://security.ubuntu.com trusty-security/multiverse i386 Packages [1,412 B] 
 Hit http://security.ubuntu.com trusty-security/main Translation-en 
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en 
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en 
 Hit http://security.ubuntu.com trusty-security/universe Translation-en 
 Get:30 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8,875 B] 
 Get:31 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [241 kB] 
 Get:32 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [9,382 B] 
 Get:33 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [397 kB] 
 Get:34 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [8,846 B] 
 Get:35 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [241 kB] 
 Get:36 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [9,558 B] 
 Hit http://in.archive.ubuntu.com trusty-updates/main Translation-en 
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse Translation-en 
 Hit http://in.archive.ubuntu.com trusty-updates/restricted Translation-en 
 Hit http://in.archive.ubuntu.com trusty-updates/universe Translation-en 
 Hit http://in.archive.ubuntu.com trusty-backports/main Sources 
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Sources 
 Hit http://in.archive.ubuntu.com trusty-backports/universe Sources 
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Sources 
 Hit http://in.archive.ubuntu.com trusty-backports/main amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/restricted amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/universe amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/main i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/restricted i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/universe i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports/main Translation-en 
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Translation-en 
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Translation-en 
 Hit http://in.archive.ubuntu.com trusty-backports/universe Translation-en 
 Ign http://in.archive.ubuntu.com trusty/main Translation-en_IN 
 Ign http://in.archive.ubuntu.com trusty/multiverse Translation-en_IN 
 Ign http://in.archive.ubuntu.com trusty/restricted Translation-en_IN 
 Ign http://in.archive.ubuntu.com trusty/universe Translation-en_IN 
 Fetched 2,431 kB in 3min 8s (12.9 kB/s) 
 Reading package lists... 
 Temp File /tmp/ptconfigure-temp-script-65684868988.sh Removed 
 [Pharaoh Logging] Package libmemcached6 from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Package php-5.3-memcached-zend-server from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Package php-5.3-extra-extensions-zend-server from the Packager Apt is already installed, so not installing 
 php5_invoke prerm: Disable module xsl for cli SAPI 
 php5_invoke prerm: Disable module xsl for cgi SAPI 
 Zend Server Daemon: running service's main ... 
 
 [28.01.2015 12:35:51 p11778/t140290098251648 WARNING] ZSemaphoreImpl::constructor: failed to get semaphore id: File exists 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  ca-certificates-java default-jre-headless imagemagick-common java-common 
  java-wrappers libboost-filesystem1.54.0 libboost-program-options1.54.0 
  libboost-regex1.54.0 libc-client2007e libfftw3-double3 libgflags2 
  libgoogle-glog0 libjargs-java liblqr-1-0 libmagickcore5 libmagickwand5 
  libonig2 libtbb2 libunwind8 mlock openjdk-7-jre-headless php5-cli 
  php5-readline python-thrift tzdata-java 
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
  php-5.3-common-extensions-zend-server php-5.3-xsl-zend-server 
 Suggested packages: 
  php-5.3-java-bridge-zend-server 
 The following packages will be REMOVED: 
  php5-xsl 
 The following NEW packages will be installed: 
  php-5.3-common-extensions-zend-server php-5.3-xsl-zend-server 
  zend-server-php-5.3-common 
 0 upgraded, 3 newly installed, 1 to remove and 301 not upgraded. 
 Need to get 0 B/69.6 MB of archives. 
 After this operation, 134 MB of additional disk space will be used. 
 (Reading database ... 178719 files and directories currently installed.) 
 Removing php5-xsl (5.5.9+dfsg-1ubuntu4.5) ... 
 Selecting previously unselected package php-5.3-xsl-zend-server. 
 (Reading database ... 178713 files and directories currently installed.) 
 Preparing to unpack .../php-5.3-xsl-zend-server_5.3.26+b2_amd64.deb ... 
 Unpacking php-5.3-xsl-zend-server (5.3.26+b2) ... 
 Selecting previously unselected package php-5.3-common-extensions-zend-server. 
 Preparing to unpack .../php-5.3-common-extensions-zend-server_6.0.0+b90_all.deb ... 
 Unpacking php-5.3-common-extensions-zend-server (6.0.0+b90) ... 
 Selecting previously unselected package zend-server-php-5.3-common. 
 Preparing to unpack .../zend-server-php-5.3-common_6.1.0+b1177_amd64.deb ... 
 Unpacking zend-server-php-5.3-common (6.1.0+b1177) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 Setting up php-5.3-xsl-zend-server (5.3.26+b2) ... 
 Setting up php-5.3-common-extensions-zend-server (6.0.0+b90) ... 
 Setting up zend-server-php-5.3-common (6.1.0+b1177) ... 
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0 
 Content-type: text/html 
 
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0 
 Content-type: text/html 
 
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0 
 Content-type: text/html 
 
 Stopping Zend Server 6.1.0 .. 
 
 zsd is not running 
 jqd is not running 
 zdd is not running 
 scd is not running 
 lighttpd is not running 
 monitor is not running 
 
 Zend Server stopped. 
 Creating/Upgrading Zend databases. This may take several minutes... 
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0 
 Content-type: text/html 

 [Pharaoh Logging] Adding Package zend-server-php-5.3-common from the Packager Apt executed correctly 
 [Pharaoh Logging] Package libapache2-mod-php-5.3-zend-server from the Packager Apt is already installed, so not installing 
 dpkg: error processing package zend-server-php-5.3 (--configure): 
  subprocess installed post-installation script returned error exit status 2 
 Errors were encountered while processing: 
 zend-server-php-5.3 
 E: Sub-process /usr/bin/dpkg returned an error code (1) 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
   ca-certificates-java default-jre-headless imagemagick-common java-common 
  java-wrappers libboost-filesystem1.54.0 libboost-program-options1.54.0 
  libboost-regex1.54.0 libc-client2007e libfftw3-double3 libgflags2 
  libgoogle-glog0 libjargs-java liblqr-1-0 libmagickcore5 libmagickwand5 
  libonig2 libtbb2 libunwind8 mlock openjdk-7-jre-headless php5-cli 
  php5-readline python-thrift tzdata-java 
 Use 'apt-get autoremove' to remove them. 
 The following NEW packages will be installed: 
  zend-server-php-5.3 
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded. 
 Need to get 0 B/2,546 B of archives. 
 After this operation, 53.2 kB of additional disk space will be used. 
 Selecting previously unselected package zend-server-php-5.3. 
 (Reading database ... 180936 files and directories currently installed.) 
 Preparing to unpack .../zend-server-php-5.3_6.1.0+b1177_amd64.deb ... 
 Unpacking zend-server-php-5.3 (6.1.0+b1177) ... 
 Setting up zend-server-php-5.3 (6.1.0+b1177) ... 
 Enabling module php5. 
 To activate the new configuration, you need to run: 
   service apache2 restart 
 Module rewrite already enabled 
 Enabling site zendserver_gui. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0 
 Content-type: text/html 
 
 ERROR: "/usr/sbin/apache2ctl" -S 2>&1 returned with error 
 [Pharaoh Logging] Adding Package zend-server-php-5.3 from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 
 

 Single App Installer: 
 -------------------------------------------- 
 ZendServer: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 



オプション
-----------

 
.. cssclass:: table-bordered 

 +-------------------------+-------------------------------------------------------+------------+-----------------------------------+
 | パラメータ              | 代替パラメータ                                        | オプション | 注釈                              |
 +=========================+=======================================================+============+===================================+
 |ptconfigure zendserver   | コマンドラインで使用することができる3つの代           | Y          | システムは、                      |
 |Install                  | 替のパラメータがある。zendserver, Zendserver,         |            | インストールプロセスを開始します  | 
 |                         | ZendServer Eg: ptconfigure zendserver install/        |            |                                   |
 |                         | ptconfigure Zendserver install                        |            |                                   |
 +-------------------------+-------------------------------------------------------+------------+-----------------------------------+
 |ptconfigure zendserver   | コマンドラインで使用することができる3つの代           | N          | システムは、                      |
 |Install                  | 替のパラメータがある。zendserver, Zendserver,         |            | インストール·プロセスを停止し、   |
 |                         | ZendServer Eg: ptconfigure zendserver install/        |            |                                   |
 |                         | ptconfigure Zendserver install|                       |            |                                   |
 +-------------------------+-------------------------------------------------------+------------+-----------------------------------+



メリット
--------------

コード、クエリ、およびフレームワーク仕様の*究極のデバッグ

* 完全な監視と根本原因分析
* 改良コードとアプリケーションのパフォーマンス
* 簡単なインストール、保守、およびクラウドでプリインストールした
* 手動または自動展開プロセス
* 真の動的な拡張性と可用性
* 認定のみと完全にサポートPHPのスタック

