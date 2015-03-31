===========
Chrome
===========

あらすじ
-------------

Google のクロムは web ページやアプリケーションその優れた JavaScript レンダリングのための電光石火の速さで実行される別の web ブラウザーです。
エンジン。

クロムは、WebKit のレイアウト エンジンを使用して Google によって作成された無料の web ブラウザーです。Chrome はその非常にシンプルでミニマルなデザインに知られており、そこに最速のブラウザーとしてもてはやさ。Chrome は現在、世界で最も広く使用される web ブラウザーです。

ヘルプ コマンド
----------------------

このコマンドは、クロムの使用量を決定するのに役立ちます。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        ptconfigure Chrome help

上記のコマンドの絵の表現は以下します。


.. code-block:: bash

 kevell@corp:/# ptconfigure Chrome help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Chrome from your package
  manager

  Chrome, chrome

        - install
        Installs Chrome
        example: ptconfigure chrome install

 ------------------------------
 End Help
 ******************************



インストール
----------------

オープン ターミナルと Linux では、同じマシンに Chrome をインストールする必要があるときにインストールするには、次のコマンドを入力します。

.. code-block:: bash
        
	        ptconfigure Chrome install


上記のコマンドの絵の表現は以下します。


.. code-block:: bash



 kevell@corp:/# ptconfigure chrome install 

 Install Chrome? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         GoogleChrome        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-83399482507.sh 
 chmod 755 /tmp/ptconfigure-temp-script-83399482507.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-83399482507.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-83399482507.sh 
 OK 
 Temp File /tmp/ptconfigure-temp-script-83399482507.sh Removed 
 Creating /tmp/ptconfigure-temp-script-57040635213.sh 
 chmod 755 /tmp/ptconfigure-temp-script-57040635213.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-57040635213.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-57040635213.sh 
 Ign http://dl.google.com stable InRelease 
 Hit http://dl.google.com stable Release.gpg 
 Hit http://dl.google.com stable Release 
 Ign http://in.archive.ubuntu.com trusty InRelease 
 Ign http://ppa.launchpad.net trusty InRelease 
 Ign http://pkg.jenkins-ci.org binary/ InRelease 
 Hit http://dl.google.com stable/main amd64 Packages 
 Hit http://downloads.hipchat.com stable InRelease 
 Ign http://packages.elasticsearch.org stable InRelease 
 Ign http://archive.canonical.com trusty InRelease 
 Hit http://dl.google.com stable/main i386 Packages 
 Ign http://security.ubuntu.com trusty-security InRelease 
 Ign http://in.archive.ubuntu.com trusty-updates InRelease 
 Ign http://extras.ubuntu.com trusty InRelease 
 Ign http://ppa.launchpad.net trusty InRelease 
 Ign http://packages.elasticsearch.org stable InRelease 
 Hit http://downloads.hipchat.com stable/main amd64 Packages 
 Ign http://repos.zend.com server InRelease 
 Ign http://in.archive.ubuntu.com trusty-backports InRelease 
 Hit http://ppa.launchpad.net trusty Release.gpg 
 Hit http://archive.canonical.com trusty Release.gpg 
 Hit http://security.ubuntu.com trusty-security Release.gpg 
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg 
 Hit http://extras.ubuntu.com trusty Release.gpg 
 Hit http://packages.elasticsearch.org stable Release.gpg 
 Hit http://repos.zend.com server Release.gpg 
 Hit http://downloads.hipchat.com stable/main i386 Packages 
 Hit http://ppa.launchpad.net trusty Release.gpg 
 Ign http://dl.google.com stable/main Translation-en_IN 
 Hit http://security.ubuntu.com trusty-security Release 
 Hit http://archive.canonical.com trusty Release 
 Ign http://dl.google.com stable/main Translation-en 
 Hit http://repos.zend.com server Release 
 Hit http://extras.ubuntu.com trusty Release 
 Hit http://in.archive.ubuntu.com trusty Release.gpg 
 Hit http://packages.elasticsearch.org stable Release.gpg 
 Hit http://ppa.launchpad.net trusty Release 
 Hit http://pkg.jenkins-ci.org binary/ Release 
 Hit http://in.archive.ubuntu.com trusty-updates Release.gpg 
 Hit http://ppa.launchpad.net trusty Release 
 Hit http://security.ubuntu.com trusty-security/main Sources 
 Hit http://repos.zend.com server/non-free amd64 Packages 
 Hit http://packages.elasticsearch.org stable Release 
 Hit http://archive.canonical.com trusty/partner amd64 Packages 
 Hit http://extras.ubuntu.com trusty/main Sources 
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg 
 Hit http://ppa.launchpad.net trusty/main amd64 Packages 
 Hit http://repos.zend.com server/non-free i386 Packages 
 Hit http://packages.elasticsearch.org stable Release 
 Hit http://security.ubuntu.com trusty-security/restricted Sources 
 Hit http://archive.canonical.com trusty/partner i386 Packages 
 Hit http://in.archive.ubuntu.com trusty Release 
 Hit http://pkg.jenkins-ci.org binary/ Packages 
 Hit http://ppa.launchpad.net trusty/main i386 Packages 
 Hit http://extras.ubuntu.com trusty/main amd64 Packages 
 Hit https://repo.varnish-cache.org precise InRelease 
 Hit http://packages.elasticsearch.org stable/main amd64 Packages 
 Hit http://security.ubuntu.com trusty-security/universe Sources 
 Hit http://in.archive.ubuntu.com trusty-updates Release 
 Hit http://ppa.launchpad.net trusty/main Translation-en 
 Hit http://extras.ubuntu.com trusty/main i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-backports Release 
 Hit http://packages.elasticsearch.org stable/main i386 Packages 
 Hit http://ppa.launchpad.net trusty/main amd64 Packages 
 Hit https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages 
 Hit http://security.ubuntu.com trusty-security/multiverse Sources 
 Hit http://in.archive.ubuntu.com trusty/main Sources 
 Hit http://ppa.launchpad.net trusty/main i386 Packages 
 Hit http://security.ubuntu.com trusty-security/main amd64 Packages 
 Hit https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/restricted Sources 
 Ign http://archive.canonical.com trusty/partner Translation-en 
 Hit http://ppa.launchpad.net trusty/main Translation-en 
 Hit http://security.ubuntu.com trusty-security/restricted amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty/universe Sources 
 Get:1 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources 
 Hit http://packages.elasticsearch.org stable/main amd64 Packages 
 Hit http://security.ubuntu.com trusty-security/universe amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages 
 Ign http://downloads.hipchat.com stable/main Translation-en_IN 
 Hit http://security.ubuntu.com trusty-security/multiverse amd64 Packages 
 Hit http://packages.elasticsearch.org stable/main i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages 
 Ign http://downloads.hipchat.com stable/main Translation-en 
 Hit http://security.ubuntu.com trusty-security/main i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages 
 Hit http://security.ubuntu.com trusty-security/restricted i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages 
 Hit http://security.ubuntu.com trusty-security/universe i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages 
 Hit http://security.ubuntu.com trusty-security/multiverse i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages 
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages 
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN 
 Hit http://security.ubuntu.com trusty-security/main Translation-en 
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en 
 Ign http://extras.ubuntu.com trusty/main Translation-en 
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en 
 Hit http://in.archive.ubuntu.com trusty/main Translation-en 
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN 
 Ign http://repos.zend.com server/non-free Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en 
 Hit http://security.ubuntu.com trusty-security/universe Translation-en 
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN 
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en 
 Ign http://repos.zend.com server/non-free Translation-en 
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en 
 Ign http://pkg.jenkins-ci.org binary/ Translation-en 
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en 
 Hit http://in.archive.ubuntu.com trusty-updates/main Sources 
 Hit http://in.archive.ubuntu.com trusty-updates/restricted Sources 
 Hit http://in.archive.ubuntu.com trusty-updates/universe Sources 
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse Sources 
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty-updates/main amd64 Packages 
 Ign http://packages.elasticsearch.org stable/main Translation-en 
 Hit http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages 
 Hit http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages 
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN 
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages 
 Ign http://packages.elasticsearch.org stable/main Translation-en 
 Hit http://in.archive.ubuntu.com trusty-updates/main i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-updates/universe i386 Packages 
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages 
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
 Reading package lists... 
 Temp File /tmp/ptconfigure-temp-script-57040635213.sh Removed 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
   jsvc libcommons-daemon-java libjetty-java libslf4j-java php5-cli 
   php5-readline 
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
   libappindicator1 libindicator7 
 The following NEW packages will be installed: 
   google-chrome-stable libappindicator1 libindicator7 
 0 upgraded, 3 newly installed, 0 to remove and 87 not upgraded. 
 1 not fully installed or removed. 
 Need to get 48.5 MB of archives. 
 After this operation, 191 MB of additional disk space will be used. 
 Get:1 http://dl.google.com/linux/chrome/deb/ stable/main google-chrome-stable amd64 41.0.2272.101-1 [48.5 MB] 
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libindicator7 amd64 12.10.2+14.04.20141007.1-0ubuntu1 [21.7 kB] 
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libappindicator1 amd64 12.10.1+13.10.20130920-0ubuntu4.1 [18.2 kB] 
 Fetched 48.5 MB in 4min 30s (179 kB/s) 
 Selecting previously unselected package libindicator7. 
 (Reading database ... 207657 files and directories currently installed.) 
 Preparing to unpack .../libindicator7_12.10.2+14.04.20141007.1-0ubuntu1_amd64.deb ... 
 Unpacking libindicator7 (12.10.2+14.04.20141007.1-0ubuntu1) ... 
 Selecting previously unselected package libappindicator1. 
 Preparing to unpack .../libappindicator1_12.10.1+13.10.20130920-0ubuntu4.1_amd64.deb ... 
 Unpacking libappindicator1 (12.10.1+13.10.20130920-0ubuntu4.1) ... 
 Selecting previously unselected package google-chrome-stable. 
 Preparing to unpack .../google-chrome-stable_41.0.2272.101-1_amd64.deb ... 
 Unpacking google-chrome-stable (41.0.2272.101-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for mime-support (3.54ubuntu1.1) ... 
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ... 
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ... 
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ... 
 Rebuilding /usr/share/applications/bamf-2.index... 
 Setting up zend-server-php-5.3 (6.1.0+b1177) ... 
 Module php5 already enabled 
 Module rewrite already enabled 
 Site zendserver_gui already enabled 
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0 
 Content-type: text/html 

 Setting up libindicator7 (12.10.2+14.04.20141007.1-0ubuntu1) ... 
 Setting up libappindicator1 (12.10.1+13.10.20130920-0ubuntu4.1) ... 
 Setting up google-chrome-stable (41.0.2272.101-1) ... 
 update-alternatives: using /usr/bin/google-chrome-stable to provide /usr/bin/x-www-browser (x-www-browser) in auto mode 
 update-alternatives: using /usr/bin/google-chrome-stable to provide /usr/bin/gnome-www-browser (gnome-www-browser) in auto mode 
 update-alternatives: using /usr/bin/google-chrome-stable to provide /usr/bin/google-chrome (google-chrome) in auto mode 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 [Pharaoh Logging] Adding Package google-chrome-stable from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Chrome: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


オプション
-----------                               


.. cssclass:: table-bordered


 +-------------------------+-----------------------------------------------+--------------+--------------------------------------------+
 | パラメーター            | 代替パラメーター                              | オプション   | コメント                                   |
 +=========================+===============================================+==============+============================================+
 |ptconfigure Chrome       | 二つの代替パラメーターのいずれかをコマンド    | Y            | ユーザがオプションを提供すると、           |
 |Install? (Y/N)           | に使用することができる- Chrome ,              |              | システムはインストールプロセスを開始します |
 |                         | 例: ptconfigure chrome Install                |              |                                            |
 +-------------------------+-----------------------------------------------+--------------+--------------------------------------------+
 |ptconfigure Chrome       | 二つの代替パラメーターのいずれかをコマンド    | N            | ユーザがオプションを提供すると、           |
 |Install? (Y/N)           | に使用することができる- Chrome ,              |              | システムはインストールプロセスを停止します |
 |                         | 例: ptconfigure chrome Install|               |              |                                            |
 +-------------------------+-----------------------------------------------+--------------+--------------------------------------------+



利点
--------------

* クロムは非常に高速のウェブブラウザーです。;ロードし、非常に迅速にページが表示されます。
* 難易度は、せず、個別のウィンドウにタブをドラッグし、できますあなたのマウスで再び。
* Google のクロムは、非常に基本的なシンプルなデザインを使用すること。
* スタートアップ ページ訪問した最も頻繁にページの一覧し、クリックし、簡単にアクセスすることができます。
* Chrome は自動的にあなたの便宜のため理解する言語にページを変換します。
* あなたはいつでもあなたのアドレスバーをインターネットを検索できます。
* あなたのタブのいずれかのサイトがクラッシュした場合他の開いたタブは受けません。
* 新しいのクロムを使用してログに記録されることがなく、インターネットを参照可能性がありますプライベート機能: インコグニート。
* Firefox と Safari とは異なり、ブラウザーのテーマと色を変更できます。
* Chrome はエクスプ ローラーと FireFox よりも高速です。
* クロム秒のみにインストールします。
 

