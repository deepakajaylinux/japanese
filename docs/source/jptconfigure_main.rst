PTConfigure
=============


概要
**********

ptconfigureは、PHPを用いて構成管理、システムの自動化とインフラを実行する際にDevOpsエンジニア、システム管理者は、インフラストラクチャマネージャを可能にする自動化ドライブです。この条項に自動的に利用者の全体のプロジェクト。

また、これは、プロジェクトへのパッケージと設定ファイルを提供するために使用することができる。それはあなたのプロジェクトの環境安定性を保証します。

ツールの他のタイプに比べながらptconfigure封筒を満たす下のモジュールシンプルでだけでなく、複雑な開発環境の要件。 ptconfigureツールをインストールすることで、全体のファラオツールの機能はカバーされます。

短いルートとして使用しているマシンの行為にptconfigureをインストールすると、他のファラオのツールのインストールを完了します。 ptconfigureのインストールプロセスの実行中最も最近更新されたバージョンの意志が追加された利点である、インストールする準備ができて取得します。

ptconfigureは、パッケージのインストールのメソッドを単純化することを目指しています。とだけでなく、それは、ユーザーが容易に知覚使用するために確保されている。

ptconfigureは、あらゆる規模の全体管理を包むのに役立つ。これは、豊か等の開発者のような管理のユーザ、システム管理者は、リリースエンジニアの必要性を満たす

ptconfigureの符号化システムは、PHPに基づいています。 ptconfigureは、オブジェクト指向のデータ型だけでなく、データに適用することができる操作の種類だけでなく、豊かである。

したがって、手続き型プログラミング技術よりオブジェクト指向プログラミング技術を比較しながら、オブジェクト指向プログラミングは、新しいタイプのオブジェクトが追加されたときに変更する必要のないモジュールを作成することができ。

追加モジュールのいずれかが必要な場合、ユーザーは、フレームとその要件に応じてモジュールを設計し、彼らは含めることができようにそれは、拡張可能です。

そしてまた、それはユーザーのニーズに従ってコードを書き換える方が簡単です。そのドキュメントは1.1.1としてptconfigureの現在リリースされたバージョンが含まれています。

インストール
**************

お使いのマシンにptconfigureをインストールする前に、gitのとPHP5があなたのマシンに存在するかどうかを確認してください。
そうでない場合、下記のように従ってください

UbuntuのではgitとPHP5をインストールするコマンド
--------------------------------------------------

.. rubric:: git 
 
.. code-block:: bash 

                apt-get install git 

.. rubric:: php 

.. code-block:: bash 

                apt-get install php 

セントのOSでのgitとPHP5をインストールするコマンド
---------------------------------------------------

.. rubric:: git 

.. code-block:: bash 

                yum install git 

.. rubric:: php 

.. code-block:: bash 

                yum install php. 

GitのとPHP5のインストールが完了した後に、のあなたのマシンでptconfigureをインストールする方法を見てみましょう。

マック、LinuxやUnixの場合
-------------------------------------

これは、符号化を使用して簡単である

.. code-block:: bash 

        git clone https://github.com/PharaohTools/ptconfigure.git && sudo php ptconfigure/install-silent 

Windowsの場合
----------------

それは簡単である、オプション「管理者として実行」を介して端末のオープンを取得して、次のコーディングを適用します

.. code-block:: bash 

	git clone https://github.com/PharaohTools/ptconfigure.git && php ptconfigure\install-silent 


可能なモジュール
******************

 DummyLinuxModule - ダミーのLinuxモジュール

 ApacheConf - Apache Conf - Apacheの設定をインストール

 ApacheModules - Apache Modules - Apache用の一般的に使用されるモジュール

 ApacheReverseProxyModules - Apache Reverse Proxy Modules - Apache用のプロキシ/ロードバランサモジュールリバース

 ApacheServer - Apache Server - Apacheサーバをインストールするか、削除する

 Apt - 追加、削除または変更メンツ

 Autopilot - PTConfigure Autopilot - ユーザー定義のインストール

 Behat - Behat - PHP BDDテストルーム

 Boxify - Boxify Wrapper - クラウドインスタンスを作成します。

 Chgrp - chgrpコマンドの機能

 chmod - chmodの機能

 CHOWN - chownコマンドの機能

 Chrome - Chrome - Chromeをインストールまたは削除する

 ChromeDriver - リモートサーバーを制御するChromeブラウザ

 Citadel - Citadel Server  - シタデルServerをインストールまたは削除する

 Cleofy - PTConfigure Cleofyer - あなたのプロジェクトのデフォルトのオートパイロットを作成します。

 Composer - Composer - アップグレードまたは再インストールして作曲

 Copy - コピー機能

 DNSify - DNSify Wrapper - DNSレコードの存在または除去を確実に

 DeveloperTools - Developer Tools - 開発者のためのIDEの他のツール

 DigitalOcean - デジタルオーシャンサ​​ーバーの管理機能

 DigitalOceanV2 - デジタルオーシャンサ​​ーバー管理機能 - APIバージョン2

 Encryption - 暗号化やファイルの復号化

 EnvironmentConfig - Environment Configuration - プロジェクトのための設定環境

 File - ファイルを変更する機能

 FileWatcher - ファイルウォッチャー - 変更に関するオプションのアクションで、ファイルの変更を待ち

 Firefoxの - Firefoxの - Firefoxをインストールまたは削除する

 Firefox14 - Firefoxの14 - のFirefoxのバージョンは非常にSeleniumサーバーでテスト

 Firefox17 - Firefoxの17 - のFirefoxのバージョンは非常にSeleniumサーバーでテスト

 Firefox24 - Firefoxの24 - のFirefoxのバージョンは非常にSeleniumサーバーでテスト

 Firefox33 - Firefoxの33 - のFirefoxのバージョンは非常にSeleniumサーバーでテスト

 Firewall  - 追加、削除、またはファイアウォールの変更

 GIMP - GIMP - イメージエディタ

 Gem  - ルビー宝石パッケージマネージャ

 Generator - PTDeployオートパイロットジェネレータ - インタラクティブにオートパイロットファイルを生成

 GitBucket - Git Bucket - - GitのSCM管理Webアプリケーション

 GitCommand - Gitのコマンド

 GitKeySafe - Git Key-Safe  - コマンド中にSSHキーを指定できるようにgitのためのスクリプトをインストールします。

 GitLab - Gitのラボ - GitのSCM管理Webアプリケーション

 GitTools - Gitのツール - GitのSCMを操作するためのツール

 HAProxy - HAプロキシサーバ - HAプロキシサーバーをインストールするか、削除する

 HHVM - HHVM - FacebookのからPHP仮想マシンの実行時

 Hostname - ホスト名を表示または変更

 INSTALLPACKAGE - PTConfigure事前定義されたインストーラ

 IntelliJの - IntelliJの - JetBrainsのからの偉大なIDE

 Invoke - SSH呼び出し関数

 JRush - JRush - ゴールデン·コンタクトのJoomlaのコマンドラインユーティリティ

 Javaの - JavaのJDK 1.7

 Jenkins - Jenkins - Javaのビルドサーバー

 JenkinsPlugins - ジェンキンスPHPプラグイン - ジェンキンスPHPのビルドのための一般的なプラグイン

 JenkinsSudoNoPass - あなたのジェンキンスユーザー用パスワードなし須藤を設定

 LigHTTPDServer - lighttpdのサーバー - lighttpdのサーバーをインストールまたは削除

 Logging - ログ記録への出力のエラー

 MediaToolsの - メディアツール - ツールは、ビューを支援し、メディアファイルを管理する

 MKDIR - MKDIR機能

 ModuleManagerによって - PTConfigureで使用されるモジュールを管理

 MongoDBは - MongoDBのサーバー - MongoDBのデータストアサーバー

 MysqlAdmins - MySQLの管理者は、 - MySQLの管理ユーザーをインストールする

 mysqlserverは - MySQLサーバ - MySQLのRDBMSサーバー

 MysqlTools - MySQLのツール - 投与すること、およびMySQLで開発するための

 NagiosServer - Nagiosのサーバー - Nagiosのサーバーをインストールまたは削除

 NetworkTools - ネットワークツール - ネットワークを操作するためのツール

 NginxServer - nginxのサーバー - nginxのサーバーをインストールまたは削除

 NodeJS - ノードJS - サーバーサイドJavaScriptエンジン

 PECL - PECLsを追加、削除または変更します

 PHPAPC - PHP APC - 一般的に使用されるPHP APC

 PHPCI - PHPCI - PHPビルドサーバー

 PHPCS - PHPコードスニファ - 静的コード解析ツール

 PHPConf - PHPカンファレンス - PHP設定をインストール

 PHPMD - PHPのメス検出器 - 静的解析ツール

 PHPModules - PHPモジュール - 一般的に使用されるPHPモジュール

 PHPSSH - PHP SSH - PHP SSH拡張

 PHPStorm - PHPStorm - JetBrainsのからの偉大なIDE

 PHPUnitは - PHPユニット - xUnitのユニットテストの標準のPHP実装

 PTConfigure - PTConfigure - アップグレードまたは再インストールしPTConfigure

 PTDeploy - PTDeploy - PHP自動ウェブサイトの展開ツール

 PTTest - アップグレードまたは再インストールしPTTest

 PTVirtualize - PTVirtualize - PHP用の仮想マシン管理ソリューション

 PackageManager - ネイティブパッケージマネージャラッパー - OS中立のパッケージをインストールする

 PapyrusEditor - パピルスエディタWebインターフェイス

 Parallax - 視差 - 並行してコマンドを実行

 Pear  - PEARパッケージマネージャ

 Phake - Phake - PHPのタスク作成ツール（メイク/レーキ）

 PharaohTools - ファラオツール - 奨めはそれらをすべてインストールします

 Pingの - そのが応答かどうかを確認するためのPingをテスト

 Port  - その上でリッスンしているプロセスを確認するポートをテスト

 PostInput - HTTP POST /ゲット入力インタフェース

 PostgresServer - Postgresのサーバ - PostgresのRDBMSサーバー

 Process - プロセスの機能

 Python  - Pythonの - プログラミング言語

 RubyBDD - ルビーBDDスイート - キュウリ、カラバッシュ、カピバラとSaucelabsの共通の宝石をインストールする

 RubyRVM - ルビーRVM - Rubyのバージョン管理

 RubySystem - ワイドルビーRVMシステム - Rubyのバージョン管理システムワイド版

 runCommandプロバイダー - コマンドを実行します

 SFTP - SFTP機能

 SVN - SVN - ソースコントロールマネージャー

 SeleniumServer - セレンWebブラウザ制御サーバー

 Service - サービスを開始、停止または再起動します

 SshEncrypt - プライベートSSHキーを暗号化/インストールする

 SshHarden - マシンのSSHアカウント/セットアップにセキュリティ機能を適用します

 SshKeyInstall - ユーザーアカウントにSSH公開鍵をインストールします。

 SshKeyStore - 保存とSSHキーにアクセスするための

 SshKeygen - SSHのkeygen - SSHケイペアを生成

 StandardTools- すべてのインストールのための標準ツール - StandardTools

 SudoNoPass - すべてのユーザーのための設定パスワードなし須藤

 SystemDetection - システム検出 - 実行中のオペレーティングシステムを検出

 Task - Task Wrapper - 簡単に再現可能なタスク

 Teamcity - Teamcity  - JetBrainsのビルドサーバー

 Templating - 実行時に置き換えるプレースホルダや線を持つファイルをインストールします。

 ThoughtWorksGo - ThoughtWorksのからの連続配信サーバ

 UbuntuCompiler - コンパイルLinuxのプログラムのために

 VNC - VNC - ディスプレイマネージャソリューション

 vncpasswdを - vncpasswdを - ディスプレイマネージャソリューション

 Varnish  - HTTPキャッシュ

 Virtualboxの - Virtualboxの - 地元の仮想マシンソリューション

 WinExe - WinExesを追加、削除または変更します

 WireframeSketcher - ワイヤーフレームスケッチャー - Wireframingアプリケーション

 Xvfbの - Xvfbの - ディスプレイマネージャソリューション

 Yum  - ヤムパッケージを追加、削除または変更します



使用方法
***********

ptconfigureツールを使用する方法を、私たちは見てみましょう、

まず、単に入力

 
.. code-block:: bash 

    ptconfigure 

このコマンドはptconfigureの下で利用可能なモジュールのすべての名前が一覧表示されます。
ここでは、スクリーンショットはptconfigure下で利用可能すべてのモジュールの表示を示している。

 
.. code-block:: bash 

    
 Kevell@corp:/# ptconfigure 
 ****************************** 


 PTConfigure - Pharaoh Tools 
 ------------------- 

 Configuration, Infrastructure and Systems Automation Management in PHP. 

 Can be used to set up a Development Client, Development Server, Testing Servers, SCM Servers or Production 
 Application Servers in minutes, out of the box, with Zero configuration across multiple Operating Systems. 

 You can quickly create simple or complex systems completely configured by code across platforms. 

 Using Convention over Configuration, a lot of common Configuration Management tasks can be completed with little or 
 no extra implementation work. 

 ------------------------------------------------------------- 

 Available Commands: 
 --------------------------------------- 

 DummyLinuxModule - Dummy Linux Module 
 ApacheConf - Apache Conf - Install a Apache Configuration 
 ApacheModules - Apache Modules - Commonly used modules for Apache 
 ApacheReverseProxyModules - Apache Reverse Proxy Modules - Reverse Proxy/Load Balancer Modules for Apache 
 ApacheServer - Apache Server - Install or remove the Apache Server 
 Apt - Add, Remove or Modify Apts 
 Autopilot - PTConfigure Autopilot - User Defined Installations 
 Behat - Behat - The PHP BDD Testing Suite 
 Boxify - Boxify Wrapper - Create Cloud Instances 
 Chgrp - Chgrp Functionality 
 Chmod - Chmod Functionality 
 Chown - Chown Functionality 
 Chrome - Chrome - Install or remove Chrome 
 ChromeDriver - The Chrome Browser remote controlling server 
 Citadel - Citadel Server - Install or remove the Citadel Server 
 Cleofy - PTConfigure Cleofyer - Creates default autopilots for your project 
 Composer - Composer - Upgrade or Re-install Composer 
 Copy - Copy Functionality 
 DNSify - DNSify Wrapper - Ensure the existence or removal of DNS records 
 DeveloperTools - Developer Tools - IDE's and other tools for Developers 
 DigitalOcean - Digital Ocean Server Management Functions 
 DigitalOceanV2 - Digital Ocean Server Management Functions - API Version 2 
 Encryption - Encryption or Decryption of files 
 EnvironmentConfig - Environment Configuration - Configure Environments for a project 
 File - Functions to Modify Files 
 FileWatcher - File Watcher - Wait for changes in files, with optional actions on changes 
 Firefox - Firefox - Install or remove Firefox 
 Firefox14 - Firefox 14 - A version of Firefox highly tested with Selenium Server 
 Firefox17 - Firefox 17 - A version of Firefox highly tested with Selenium Server 
 Firefox24 - Firefox 24 - A version of Firefox highly tested with Selenium Server 
 Firefox33 - Firefox 33 - A version of Firefox highly tested with Selenium Server 
 Firewall - Add, Remove or Modify Firewalls 
 GIMP - GIMP - The Image Editor 
 Gem - Ruby Gems Package Manager 
 Generator - PTDeploy Autopilot Generator - Generate Autopilot files interactively 
 GitBucket - Git Bucket - The Git SCM Management Web Application 
 GitCommand - Git Commands 
 GitKeySafe - Git Key-Safe - Install a script for git to allow specifying ssh keys during commands 
 GitLab - Git Lab - The Git SCM Management Web Application 
 GitTools - Git Tools - Tools for working with Git SCM 
 HAProxy - HA Proxy Server - Install or remove the HA Proxy Server 
 HHVM - HHVM - The PHP Virtual Machine runtime from Facebook 
 Hostname - View or Modify Hostname 
 InstallPackage - PTConfigure Predefined Installers 
 IntelliJ - IntelliJ - A great IDE from JetBrains 
 Invoke - SSH Invocation Functions 
 JRush - JRush - The Joomla command line utility from Golden Contact 
 Java - Java JDK 1.7 
 Jenkins - Jenkins - The Java Build Server 
 JenkinsPlugins - Jenkins PHP Plugins - Common Plugins for Jenkins PHP Builds 
 JenkinsSudoNoPass - Configure Passwordless Sudo for your Jenkins user 
 LigHTTPDServer - LigHTTPD Server - Install or remove the LigHTTPD Server 
 Logging - Logging - Output errors to the logging 
 MediaTools - Media Tools - Tools to help view and manage Media files 
 Mkdir - Mkdir Functionality 
 ModuleManager - Manage the modules used in PTConfigure 
 MongoDB - MongoDB Server - The MongoDB Datastore Server 
 MysqlAdmins - Mysql Admins - Install administrative users for Mysql 
 MysqlServer - Mysql Server - The Mysql RDBMS Server 
 MysqlTools - Mysql Tools - For administering and developing with Mysql 
 NagiosServer - Nagios Server - Install or remove the Nagios Server 
 NetworkTools - Network Tools - Tools for working with Networks 
 NginxServer - Nginx Server - Install or remove the Nginx Server 
 NodeJS - Node JS - The Server Side Javascript Engine 
 PECL - Add, Remove or Modify PECLs 
 PHPAPC - PHP APC - Commonly used PHP APC 
 PHPCI - PHPCI - The PHP Build Server 
 PHPCS - PHP Code Sniffer - The static code analysis tool 
 PHPConf - PHP Conf - Install a PHP Configuration 
 PHPMD - PHP Mess Detector - The static analysis tool 
 PHPModules - PHP Modules - Commonly used PHP Modules 
 PHPSSH - PHP SSH - PHP SSH Extension 
 PHPStorm - PHPStorm - A great IDE from JetBrains 
 PHPUnit - PHP Unit - The PHP Implementation of the XUnit Unit Testing standard 
 PTConfigure - PTConfigure - Upgrade or Re-install PTConfigure 
 PTDeploy - PTDeploy - The PHP Automated Website Deployment tool 
 PTTest - Upgrade or Re-install PTTest 
 PTVirtualize - PTVirtualize - The Virtual Machine management solution for PHP 
 PackageManager - Native Package Manager Wrapper - Install OS neutral packages 
 PapyrusEditor - Papyrus Editor Web Interface 
 Parallax - Parallax - Execute commands in parallel 
 Pear - Pear Package Manager 
 Phake - Phake - The PHP task creation tool (Make/Rake) 
 PharaohTools - Pharaoh Tools - Gotta Install them all 
 Ping - Test a Ping to see if its responding 
 Port - Test a Port to see which process is listening on it 
 PostInput - HTTP Post/Get Input Interface 
 PostgresServer - Postgres Server - The Postgres RDBMS Server 
 Process - Process Functionality 
 Python - Python - The programming language 
 RubyBDD - Ruby BDD Suite - Install Common Gems for Cucumber, Calabash, Capybara and Saucelabs 
 RubyRVM - Ruby RVM - The Ruby version manager 
 RubySystem - Ruby RVM System wide - The Ruby version manager system wide version 
 RunCommand - Execute a Command 
 SFTP - SFTP Functionality 
 SVN - SVN - The Source Control Manager 
 SeleniumServer - The Selenium Web Browser controlling server 
 Service - Start, Stop or Restart a Service 
 SshEncrypt - Install/encrypt private SSH keys 
 SshHarden - Apply security functions to the SSH accounts/setup of the machine 
 SshKeyInstall - Install SSH Public Keys to a user account 
 SshKeyStore - For Storing and Accessing SSH Keys 
 SshKeygen - SSH Keygen - Generate SSH Kay Pairs 
 StandardTools - Standard Tools for any Installation 
 SudoNoPass - Configure Passwordless Sudo for any User 
 SystemDetection - System Detection - Detect the Running Operating System 
 Task - Task Wrapper - easily repeatable tasks 
 Teamcity - Teamcity - The Jetbrains Build Server 
 Templating - Install files with placeholders or lines replaced at runtime 
 ThoughtWorksGo - The Continuous Delivery server from ThoughtWorks 
 UbuntuCompiler - For Compiling Linux Programs 
 VNC - VNC - The Display Manager Solution 
 VNCPasswd - VNCPasswd - The Display Manager Solution 
 Varnish - The HTTP Cache 
 Virtualbox - Virtualbox - The local Virtual Machine Solution 
 WinExe - Add, Remove or Modify WinExes 
 WireframeSketcher - Wireframe Sketcher - the Wireframing application 
 Xvfb - Xvfb - The Display Manager Solution 
 Yum - Add, Remove or Modify Yum Packages 
 
 --------------------------------------- 
 Visit www.pharaohtools.com for more 
 ****************************** 
 


Video Cast Instruction 
*********************** 

.. raw:: html 

        <iframe width="560" height="315" src="http://pharaohtools.com/components/com_jomwebplayer/player.swf?r=1731863942" frameborder="0" allowfullscreen></iframe> 
        <br> 
        <br> 

.. rubric:: What You can Learn Here 


Helpコマンド
*****************

あなたが特定のモジュールの目的を知りたい場合は、次のように単にコマンドを入力します。

 
    ptconfigure ModuleName help 

このコマンドは、その特定のモジュールの使用法とは、ユーザーが実行できるアクションで使用可能なオプションを提供します。
下のスクリーンショットは、helpコマンドを使用してptconfigure下Behatモジュールの使用方法を説明しています。

 
.. code-block:: bash 

        Kevell@corp:/# ptconfigure behat help 
        ****************************** 


        This command allows you to install Behat. 

        Behat, behat 

        - install 
        Installs the latest version of behat 
        example: ptconfigure behat install 

        ------------------------------ 
        End Help 
        ****************************** 




PTConfigureモジュールと遊ぶ         
*******************************


.. toctree::
   :maxdepth: 6
    
   


   jamazoncloudfront
   jamazoncloudwatch  
   jamazondynamodb
   jamazonelasticache
   jamazonroute53
   jamazons3
   japacheconf
   japachemodules
   japachereverseproxy
   japacheserver
   japachevhosteditor
   japtana
   japt
   jautopilot
   jawscloudformation
   jawsrds
   jawstats
   jbehat
   jboxify
   jcassandra
   jchgrp
   jchmode
   jchown
   jchrome
   jchromedriver
   jcitadel
   jcleofy
   jcomposer
   jcopy
   jdevelopertools
   jdigitalocean
   jdnsify
   jencryption
   jenvironmentconfig
   jfile
   jfirefox
   jfirefox14
   jfirefox17
   jfirefox24
   jfirefox33
   jfirewall
   jgem
   jgenerator
   jgimp
   jgitbucket
   jgitkeysafe
   jgitlab
   jgittools
   jhaproxy
   jhhvm
   jhostname
   jinstallpackage
   jintellij
   jinvoke
   jjava
   jjenkins
   jjenkinsplugins
   jjenkinssudonopass
   jjetty
   jjmeter
   jjrush
   jlighttpdserver
   jlogging
   jmediatools
   jmemcached
   jminify
   jmkdir
   jmodulemanager
   jmongodb
   jmysqladmins
   jmysqlserver
   jmysqltools
   jnagiosserver
   jnetbeans
   jnetworktools
   jnewrelic
   jnginxserver
   jnodejs
   jopenoffice
   joracle
   jpackagemanager
   jparallax
   jpear
   jpecl
   jphake
   jpharaohtools
   jphpapc
   jphpci
   jphpcodebeautifier
   jphpconf
   jphpcs
   jphpdox
   jphpeclipse
   jphpedit
   jphpmd
   jphpmodules
   jphpssh
   jphpstorm
   jphpunit
   jphpvm
   jping
   jport
   jpostgressserver
   jprocess
   jptconfigure
   jptbuild
   jptdeploy
   jpttest
   jptvirtualize
   jpython
   jra
   jrackspace
   jredis
   jrubybdd
   jrubyrvm
   jrubysystem
   jruncommand
   jseleniumserver
   jservice
   jsftp
   jskipfish
   jsshencrypt
   jsshharden
   jsshkeygen
   jsshkeyinstall
   jsshkeystore
   jstandardtools
   jstoryplayer
   jsudonopass
   jsvn
   jsystemdetection
   jteamcity   
   jtemplating
   jtomcat
   jubuntucompiler
   juser
   jvarnish
   jvirtualbox
   jvmplayer
   jvmwareworkstation
   jvnc
   jvncpassword
   jwireframesketcher
   jxvfb
   jzendserver
  


