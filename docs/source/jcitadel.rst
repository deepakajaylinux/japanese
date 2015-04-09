=========
Citadel
=========

あらすじ
-----------

シタデルは、完全な機能豊富なオープン ソースのグループウェア プラットフォーム。シタデル システムは非常に汎用性です。テキスト ベースのインタ フェース、AJAX スタイルの web インターフェイスなど多くの人気のある PIM クライアント SMTP、POP、IMAP を使用して、ユーザーに提示する多数のフロント エンドを提供しています。これらのすべては同時に使用することができます。

また、非常にスケーラブルです。設備の整ったシタデル サーバーは多数の同時ユーザーをサポートできるだけでなく、ルームとその内容を共有する城砦ノードの分散ネットワークを作成することもできます。

ヘルプ コマンド
----------------

このコマンドは、シタデル モジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。宣言で使用されている代替パラメーターはヘルプ オプションの下で明確に定義されます。このコマンドをインストールに使用するコマンドを知っているエンド ・ ユーザーのガイドします。以下に、コマンド。


.. code-block:: bash
     	
	ptconfigure  Citadel help


スクリーン ショットの絵の表現は以下します。


.. code-block:: bash
 

 kevell@corp:/# ptconfigure Citadel help
 ******************************


  This module installs Citadel Server and provides configuration

  Citadel, citadel-server, citadel

        - install
        Installs Citadel Server
        example: ptconfigure citadel install

        - configure
        Configure E-Mail with Citadel Server
        example: ptconfigure citadel configure

 ------------------------------
 End Help
 ******************************


インストール
--------------

シタデル サーバー マシンにインストールする必要があるとき城砦スイートをインストールするには、次のコマンドを入力できます。システムがインストールの手順を実行します。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
       
	ptconfigure Citadel  install



.. code-block:: bash



 kevell@corp:/# ptconfigure citadel install 


 Install Citadel Server? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Citadel Server!        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-77287537627.sh 
 chmod 755 /tmp/ptconfigure-temp-script-77287537627.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-77287537627.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-77287537627.sh 
 Temp File /tmp/ptconfigure-temp-script-77287537627.sh Removed 
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Stopping apache2 service 
  * Stopping web server apache2 
  * 
 Creating /tmp/ptconfigure-temp-script-39510208428.sh 
 chmod 755 /tmp/ptconfigure-temp-script-39510208428.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-39510208428.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-39510208428.sh 
 Temp File /tmp/ptconfigure-temp-script-39510208428.sh Removed 
 invoke-rc.d: initscript lighttpd, action "reload" failed. 
 apache2_invoke: Enable configuration javascript-common 
 invoke-rc.d: initscript apache2, action "reload" failed. 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following extra packages will be installed: 
  citadel-client citadel-mta citadel-server citadel-webcit javascript-common 
  libcitadel4 libev4 libjs-prototype libjs-scriptaculous libsieve2-1 tinymce 
 Suggested packages: 
  localepurge 
 Recommended packages: 
  db4.6-util 
 The following NEW packages will be installed: 
  citadel-client citadel-mta citadel-server citadel-suite citadel-webcit 
  javascript-common libcitadel4 libev4 libjs-prototype libjs-scriptaculous 
  libsieve2-1 tinymce 
 0 upgraded, 12 newly installed, 0 to remove and 86 not upgraded. 
 Need to get 1,955 kB of archives. 
 After this operation, 8,788 kB of additional disk space will be used. 
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main javascript-common all 11 [6,066 B] 
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjs-prototype all 1.7.1-3 [44.2 kB] 
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjs-scriptaculous all 1.9.0-2 [107 kB] 
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libsieve2-1 amd64 2.2.6-1.2 [73.1 kB] 
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/universe tinymce all 3.4.8+dfsg0-1 [488 kB] 
 Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libcitadel4 amd64 8.24-1 [60.5 kB] 
 Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-client amd64 8.24-1 [78.5 kB] 
 Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libev4 amd64 1:4.15-3 [29.6 kB] 
 Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-server amd64 8.24-1 [348 kB] 
 Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-mta amd64 8.24-1 [4,520 B] 
 Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-webcit amd64 8.24-dfsg-1 [712 kB] 
 Get:12 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-suite all 8.24-dfsg-1 [3,542 B] 
 Preconfiguring packages ... 
 Fetched 1,955 kB in 21s (92.5 kB/s) 
 Selecting previously unselected package javascript-common. 
 (Reading database ... 194611 files and directories currently installed.) 
 Preparing to unpack .../javascript-common_11_all.deb ... 
 Unpacking javascript-common (11) ... 
 Selecting previously unselected package libjs-prototype. 
 Preparing to unpack .../libjs-prototype_1.7.1-3_all.deb ... 
 Unpacking libjs-prototype (1.7.1-3) ... 
 Selecting previously unselected package libjs-scriptaculous. 
 Preparing to unpack .../libjs-scriptaculous_1.9.0-2_all.deb ... 
 Unpacking libjs-scriptaculous (1.9.0-2) ... 
 Selecting previously unselected package libsieve2-1. 
 Preparing to unpack .../libsieve2-1_2.2.6-1.2_amd64.deb ... 
 Unpacking libsieve2-1 (2.2.6-1.2) ... 
 Selecting previously unselected package tinymce. 
 Preparing to unpack .../tinymce_3.4.8+dfsg0-1_all.deb ... 
 Unpacking tinymce (3.4.8+dfsg0-1) ... 
 Selecting previously unselected package libcitadel4. 
 Preparing to unpack .../libcitadel4_8.24-1_amd64.deb ... 
 Unpacking libcitadel4 (8.24-1) ... 
 Selecting previously unselected package citadel-client. 
 Preparing to unpack .../citadel-client_8.24-1_amd64.deb ... 
 Unpacking citadel-client (8.24-1) ... 
 Selecting previously unselected package libev4. 
 Preparing to unpack .../libev4_1%3a4.15-3_amd64.deb ... 
 Unpacking libev4 (1:4.15-3) ... 
 Selecting previously unselected package citadel-server. 
 Preparing to unpack .../citadel-server_8.24-1_amd64.deb ... 
 Unpacking citadel-server (8.24-1) ... 
 Selecting previously unselected package citadel-mta. 
 Preparing to unpack .../citadel-mta_8.24-1_amd64.deb ... 
 Unpacking citadel-mta (8.24-1) ... 
 Selecting previously unselected package citadel-webcit. 
 Preparing to unpack .../citadel-webcit_8.24-dfsg-1_amd64.deb ... 
 Unpacking citadel-webcit (8.24-dfsg-1) ... 
 Selecting previously unselected package citadel-suite. 
 Preparing to unpack .../citadel-suite_8.24-dfsg-1_all.deb ... 
 Unpacking citadel-suite (8.24-dfsg-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 Setting up javascript-common (11) ... 
 * Reloading web server configuration lighttpd 
   ...fail! 
 * Reloading web server apache2 
 * 
 * Apache2 is not running 
 Setting up libjs-prototype (1.7.1-3) ... 
 Setting up libjs-scriptaculous (1.9.0-2) ... 
 Setting up libsieve2-1 (2.2.6-1.2) ... 
 Setting up tinymce (3.4.8+dfsg0-1) ... 
 Setting up libcitadel4 (8.24-1) ... 
 Setting up citadel-client (8.24-1) ... 
 Adding group `citadel' (GID 132) ... 
 Done. 
 Adding system user `citadel' (UID 123) ... 
 Adding new user `citadel' (UID 123) with group `citadel' ... 
 Not creating home directory `/var/lib/citadel'. 
 Setting up libev4 (1:4.15-3) ... 
 Setting up citadel-server (8.24-1) ... 
 Setting up citadel-webcit (8.24-dfsg-1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 Setting up citadel-mta (8.24-1) ... 
 Setting up citadel-suite (8.24-dfsg-1) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 [Pharaoh Logging] Adding Package citadel-suite from the Packager Apt executed correctly 
 [Pharaoh Logging] Restarting citadel service 
 sendcommand: started (pid=24114) connecting to Citadel server at /var/run/citadel/citadel-admin.socket 
 200 karthik Citadel server ADMIN CONNECTION ready. 
 DOWN 
 231 Shutting down server.  Goodbye. 
 sendcommand: processing ended. 
 ....................... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Citadel: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 



                             

.. cssclass:: table-bordered

 +--------------------------+------------------------------------------------------+------------+--------------------------------------------+
 | パラメータ               | 代替パラメータ                                       | オプション | 注釈                                       |
 +==========================+======================================================+============+============================================+
 |ptconfigure Citadel       | 3つの代替のパラメータのいずれかは、                  | Y          | ユーザーがこのオプションを提供すると、     |
 |Install? (Y/N)            | コマンドで使用することができる- Citadel,             |            | システムはインストールプロセスを開始します |
 |                          | citadel-server, citadel                              |            |                                            |
 |                          | 例: ptconfigure citadel-server Install               |            |                                            |
 +--------------------------+------------------------------------------------------+------------+--------------------------------------------+
 |ptconfigure Citadel       | 3つの代替のパラメータのいずれかは、                  | N          | ユーザーがこのオプションを提供すると、     |
 |Install? (Y/N)            | コマンドで使用することができる- Citadel,             |            | システムはインストールプロセスを停止します |
 |                          | citadel-server, citadel                              |            |                                            |
 |                          | 例: ptconfigure citadel-server Install|              |            |                                            |
 +--------------------------+------------------------------------------------------+------------+--------------------------------------------+


構成
-------------

このコマンドは、シタデル サーバーを構成するのに役立ちます。一度、下特定のコマンドが実行されるシステムが提供する各セクションの既定値を任意に変更が行われる場合、ユーザー データを提供できます。構成を使用するコマンドを次に示します。


.. code-block:: bash
         
        ptconfigure Citadel configure

.. code-block:: bash

 kevell@corp# ptconfigure citadel configure

 *******************************
 *        Pharaoh Tools        *
 *         Citadel Server!        *
 *******************************
 [Pharaoh Logging] No environment name provided for Load Balancing
 What is the environment name you want to balance load to? 
 kevell
 Set non-default value for global_log? Default is 127.0.0.1 local0 notice (Y/N) 
 n
 Set non-default value for global_maxconn? Default is 2000 (Y/N) 
 n
 Set non-default value for global_user? Default is citadel (Y/N) 
 n
 Set non-default value for global_group? Default is citadel (Y/N) 
 n
 Set non-default value for defaults_log? Default is global (Y/N) 
 n
 Set non-default value for defaults_mode? Default is http (Y/N) 
 n
 Set non-default value for defaults_option_string? Default is option httplog
    option dontlognull
    option redispatch (Y/N) 
 n
 Set non-default value for defaults_retries? Default is 3 (Y/N) 
 n
 Set non-default value for defaults_timeout_connect? Default is 5000 (Y/N) 
 n
 Set non-default value for defaults_timeout_client? Default is 10000 (Y/N) 
 n
 Set non-default value for defaults_timeout_server? Default is 10000 (Y/N) 
 n
 Set non-default value for listen_appname? Default is appname (Y/N) 
 n
 Set non-default value for listen_ip_port? Default is 0.0.0.0:80 (Y/N) 
 n
 Set non-default value for listen_mode? Default is http (Y/N) 
 n
 Set non-default value for listen_stats_enable? Default is enable (Y/N) 
 n
 Set non-default value for listen_stats_uri_string? Default is stats uri /citadel?stats (Y/N) 
 n
 Set non-default value for listen_stats_realm_string? Default is stats realm Strictly\ Private (Y/N) 
 n
 Set non-default value for listen_stats_auth_string? Default is stats auth ptconfigure:ptconfigure (Y/N) 
 n
 Set non-default value for listen_balance? Default is roundrobin (Y/N) 
 n
 Set non-default value for listen_option_string? Default is option httpclose
    option forwardfor (Y/N) 
 n
 Set non-default value for listen_server_string? Default is server  192.168.1.10:80 check
 (Y/N) 
 n
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Citadel Server: Success
 ------------------------------
 Installer Finished
 ******************************





利点
--------

* E メール、カレンダー/スケジューリング、アドレス帳
* 掲示板、メーリング リスト サーバーをインスタント メッセージング
* 複数ドメインのサポート
* 直感的な魅力的な AJAX スタイル web インターフェイス
 

