==============
PTDeploy
==============


概要
------------

ptdeployは、PHPのコードによる自動展開、ビルドおよびリリースの機能、Webアプリケーションのバージョン管理やインフラを持つユーザーのアプリケーションを包み込む。

これは、ユーザーが容易になり、自動化された配置テンプレートを提供し、あなたのプロジェクトのために完全に連続ビルドをインストールします。

helpコマンド
---------------------

あなたが特定のモジュールの目的を知りたい場合は、次のように単にコマンドを入力します。

.. code-block:: bash
        
                ptdeploy ModuleName help

このコマンドは、その特定のモジュールの使用法とは、ユーザーが実行できるアクションで使用可能なオプションを提供します。下のスクリーンショットは、helpコマンドを使用してptdeploy下のモジュールApacheのコントロールの使用方法を説明しています。


.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheControl help
 ******************************


  This command is part of Default Modules and handles Apache Server Control Functions.

  ApacheControl, apachecontrol, apachectl

          - start
          Start the Apache server
          example: ptdeploy apachecontrol start
          example: ptdeploy apachecontrol start --yes --guess
          example: ptdeploy apachecontrol start --yes --apache-command="apache2"

          - stop
          Stop the Apache server
          example: ptdeploy apachecontrol stop
          example: ptdeploy apachecontrol stop --yes --guess
          example: ptdeploy apachecontrol stop --yes --apache-command="apache2"

          - restart
          Restart the Apache server
          example: ptdeploy apachecontrol restart
          example: ptdeploy apachecontrol restart --yes --guess
          example: ptdeploy apachecontrol restart --yes --apache-command="apache2"

          - reload
          Reloads the Apache server configuration without restarting
          example: ptdeploy apachecontrol reload
          example: ptdeploy apachecontrol reload --yes --guess
          example: ptdeploy apachecontrol reload --yes --apache-command="apache2"

 ------------------------------
 End Help
 ******************************


helpコマンドも宣言で使用できる代替パラメータを示します。



なぜ、このptdeployを構築する
------------------------------------------

十分に展開するために構築するために、多くのファイルをFTPまたは他の広告アドホック溶液からコピーするために必要とされる。また、エンタープライズ自動化ツールの多くが欠落していた。ファラオのツールの下でこれらの不足のptdeployを克服するために構築した。
PHPは、ルビーはカピストラーノのギャップをfiils同じようptdeployを持っています。

このツールは、プロビジョニングアプリケーションのためであり、あなたの箱に構築します。ユーザーは、1つまたは2つのPHPファイルや、迅速にセットアップクラウドフレンドリー配備パターンで自分のシステムにさえ、単純または複雑なアプリケーションの配備パターンを設定することができます。

ptdeployはモジュールです。オブジェクト指向と拡張可能。したがって、ユーザーは彼らの要件に基づいて、新しいモジュールを作成して追加することができます余分なモジュールを必要とする場合。

このptdeployは、ユーザーの展開のすべてのステップが単一のファイルにカバーされますラッパーとして機能します。これは、アプリケーションのインスタンスを起動するために1つのコマンドを使用できます。

インストール
---------------

ptdeployのインストールは、可用性と、ユーザーの要件に応じて2つの方法で行うことができます。彼らptdeployをインストールする2つの方法があります。

* ptconfigure経由でptdeployのインストール
* ptconfigureに依存せずにptdeployをインストールする。



ptconfigure経由でptdeployのインストール
-------------------------------------------------

ユーザーは自分のマシンでptconfigureを持っている場合、それは、次のコマンドを使用してptdeployをインストールするための簡単​​な方法は、次のとおりです。

.. code-block:: bash

        sudo ptconfigure ptdeploy install --yes --guess


ptconfigureに依存せずにptdeployのインストール
------------------------------------------------------------------------------

ユーザーは応じて、彼らは、次のコマンドを使用することができptconfigureを使用せずにptdeployをインストールしたい場合：

.. code-block:: bash
                
        sudo apt-get install php5 git

.. code-block:: bash

        git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install-silent

or 

以下のコマンドは、インストール時に場所を指定したいユーザーのための予測可能である。

.. code-block:: bash

        git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install

高度な機能
-------------------------

ホストファイルの編集、仮想ホスト·ファイル、設定ファイル、データベースの更新とそれ以上はこのすべてを使用して自動化することができます。

リモート·サーバー管理の機能を使用することにより、ユーザーは任意のサイズのインフラストラクチャ全体の展開を自動化することができます。


ptdeployがdapperfy使用してプロジェクトを推進してどのような方法
-----------------------------------------------------------------------------------------

ワードdapperfyは、プロジェクトのためのいくつかのオートパイロットを作成ptdeployコマンドです。

dapperfyを使用することは非常に迅速であり、そしておそらく最高の出発点です。

Capify対Dapperfy
-------------------------

dapperfyとcapifyを比較すると、それは、PHPで書かれているようdapperfyが最良であると言うことは明らかである。

強力なポイントは、dapperfy ptdeployコマンドはユーザーがプロジェクトのためのオートパイロットの標準セットを提供することである。どこcapifyはRubyプロジェクトと同様の機能を提供します。

どのように使用し、可能なモジュール
-----------------------------------------------

単に入力し、第一、ptdeployツールを使用する方法を、私たちは見てみましょう

.. code-block:: bash

        ptdeploy

このコマンドはptdeployの下で利用可能なモジュールのすべての名前が一覧表示されます。

Available Commands:
---------------------------------------

* ApacheControl - Apacheサーバコントロール
* ApacheVHostEditor - Apacheバーチャルホスト機能
* AppSettings - PTDeployアプリケーションの設定
* Autopilot - PTConfigureオートパイロット - ユーザー定義のインストール
* Builderfy - PTDeploy Builderfyer - あなたのプロジェクトのためにいくつかの標準オートパイロットを作成します。
* CukeConf - キュウリの設定
* DBConfigure - データベース接続の設定機能
* DBInstall - データベースのインストール管理機能
* Dapperfy - PTDeploy Dapperfyer - あなたのプロジェクトのために自動化されたアプリケーションの展開オートパイロット
* Drupal - Drupalの - Drupalのための統合とテンプレート
* EnvironmentConfig - 環境設定 - プロジェクトのために環境を構成
* GitClone - GitCloneソース対照クローン機能
* HostEditor - ファイル管理機能をホストする
* Invoke - SSH呼び出し機能
* Joomla - Joomlaの - Joomlaのための統合とテンプレート
* LighttpdControl - Lighttpdのサーバーコントロール
* Logging -ログ - ログ記録への出力のエラー
* NginxControl - nginxのサーバーコントロール
* NginxSBEditor - nginxのサーバーのブロック機能
* ParallelSshChild - コマンドの実行関数
* Project - PTDeployプロジェクト管理機能
* RunCommand - コマンドを実行する
* SFTP - SFTP機能
* SVN - SVNソースコントロールプロジェクトチェックアウト/ダウンロード機能
* SystemDetection - システムの検出は - 実行中のオペレーティングシステムを検出
* Templating - テンプレート化
* Version - バージョン管理機能
* Wordpress - Wordpressの - Wordpressのための統合とテンプレート

 ******************************


ここでは、スクリーンショットはptconfigure下で利用可能すべてのモジュールの表示を示している。


.. code-block:: bash

 Available Commands:
 ---------------------------------------

 ApacheControl - Apache Server Control
 ApacheVHostEditor - Apache Virtual Host Functions
 AppSettings - PTDeploy Application Settings
 Autopilot - PTConfigure Autopilot - User Defined Installations
 Builderfy - PTDeploy Builderfyer - Create some standard autopilots for your project
 CukeConf - Cucumber Configuration
 DBConfigure - Database Connection Configuration Functions
 DBInstall - Database Installation Management Functions
 Dapperfy - PTDeploy Dapperfyer - Automated Application Deployment autopilots for your project
 Drupal - Drupal - Integration and Templates for Drupal
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 GitClone - GitClone Source Control Clone Functions
 HostEditor - Host File Management Functions
 Invoke - SSH Invocation Functions
 Joomla - Joomla - Integration and Templates for Joomla
 LighttpdControl - Lighttpd Server Control
 Logging - Logging - Output errors to the logging
 NginxControl - Nginx Server Control
 NginxSBEditor - Nginx Server Block Functions
 ParallelSshChild - Command Execution Functions
 Project - PTDeploy Project Management Functions
 RunCommand - Execute a Command
 SFTP - SFTP Functionality
 SVN - SVN Source Control Project Checkout/Download Functions
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Version - Versioning Functions
 Wordpress - Wordpress - Integration and Templates for Wordpress

 ******************************



.. toctree::
   :maxdepth: 6
   
   
 japachecontrol_deploy
 japachevhosteditor_deploy
 jappsettings_deploy
 jautopilot_deploy
 jdapperfy_deploy
 jdbconfigure_deploy
 jdbinstall_deploy
 jdrupal_deploy
 jenvironmentconfig_deploy
 jgitclone_deploy
 jgrafana_deploy
 jhosteditor_deploy
 jinvoke_deploy
 jjoomla_deploy
 jlighttpdcontrol_deploy
 jlogging_deploy
 jnginxcontrol_deploy 
 jnginxsbeditor_deploy
 jproject_deploy
 jruncommand_deploy
 jsftp_deploy
 jsvn_deploy
 jsystemdetection_deploy
 jtemplating_deploy
 jversion_deploy
 jwordpress_deploy

