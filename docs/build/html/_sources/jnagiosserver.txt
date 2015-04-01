==============
NagiosServer
==============

あらすじ
-------------

Nagios は、オープン ソースのコンピューター システムの監視、ネットワーク監視インフラストラクチャ監視ソフトウェア アプリケーションです。Nagios は監視と警告、サーバー、スイッチ、アプリケーション、およびサービスのサービスを提供しています。物事がうまくいかないとき、ユーザーに警告し、問題が解決されている 2 番目の時間を警告します。

Nagios は、もともと NetSaint の名の下に作成書かれていた、公式と非公式の両方のプラグインを維持することは積極的に開発者のグループと共にイーサン Galstad によって現在維持されます。Nagios はもともと Linux で実行ように設計がまた他の Unix 系システムでよく実行されます。それはフリー ソフトウェアの GNU 一般公衆利用許諾契約書バージョン 2 フリー ソフトウェア財団によって発行された条件の下でライセンスされています。

ヘルプ コマンド
----------------------

このコマンドは、Nagios のモジュールの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        ptconfigure nagios help


上記のコマンドの絵のスクリーン ショットは以下します。


.. code-block:: bash

 kevell@corp:/# ptconfigure nagiosserver help

 ******************************


  This command is part of Core and provides you with a method by which you can install Nagios.

  NagiosServer, nagios-server, nagiosserver, nagios

        - install
        Installs Nagios Network Monitoring Server
        example: ptconfigure nagios-server install

 ------------------------------
 End Help
 ******************************



インストール
----------------

このコマンドは、システムに、Nagios のインストールに役立ちます。特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash
        
	        ptconfigure nagios install

上記のコマンドの絵の表現は以下します。

.. code-block:: bash


 kevell@corp:/# ptconfigure nagios-server install

 Install Nagios Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Nagios Server!        *
 *******************************

 * Starting nagios3 monitoring daemon nagios3                                                                                  [ OK ] 
 enabling Apache2 config...
 apache2_invoke: Enable module cgi
 * Restarting web server apache2                                                                                                  AH00558:  
 apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to 
 suppress this message
                                                                                                                               [ OK ]
 apache2_invoke: Enable configuration nagios3
 * Reloading web server apache2                                                                                                        * 
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery nagios-images nagios3-cgi nagios3-common nagios3-core
 Suggested packages:
  javascript-common
 The following NEW packages will be installed:
  libjs-jquery nagios-images nagios3 nagios3-cgi nagios3-common nagios3-core
 0 upgraded, 6 newly installed, 0 to remove and 250 not upgraded.
 Need to get 3,748 kB of archives.
 After this operation, 12.3 MB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main nagios-images all 0.8 [2,589 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-common all 3.5.1-1ubuntu1 [53.7 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-cgi amd64 3.5.1-1ubuntu1 [794 kB]
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-core amd64 3.5.1-1ubuntu1 [231 kB]
 Get:6 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3 amd64 3.5.1-1ubuntu1 [1,528 B]
 Preconfiguring packages ...
 Fetched 3,748 kB in 1min 11s (52.1 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 231932 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package nagios-images.
 Preparing to unpack .../nagios-images_0.8_all.deb ...
 Unpacking nagios-images (0.8) ...
 Selecting previously unselected package nagios3-common.
 Preparing to unpack .../nagios3-common_3.5.1-1ubuntu1_all.deb ...
 Unpacking nagios3-common (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-cgi.
 Preparing to unpack .../nagios3-cgi_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-cgi (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-core.
 Preparing to unpack .../nagios3-core_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-core (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3.
 Preparing to unpack .../nagios3_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3 (3.5.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up nagios-images (0.8) ...
 Setting up nagios3-common (3.5.1-1ubuntu1) ...
 Setting up nagios3-cgi (3.5.1-1ubuntu1) ...
 Setting up nagios3-core (3.5.1-1ubuntu1) ...
 Setting up nagios3 (3.5.1-1ubuntu1) ...
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NagiosServer: Success
 ------------------------------
 Installer Finished
 ******************************



オプション
------------
                               

.. cssclass:: table-bordered

 +-------------------+--------------------------------------------------------+------------+-----------------------------------------+
 | パラメーター      | 代替パラメーター                                       | オプション | コメント                                |
 +===================+========================================================+============+=========================================+
 |Install Nagios     | コマンドラインで使用することができる4つの別のパラメ    | Y          | システムは、インストールプロセスを      |
 |Server Install?    | ータがある。NagiosServer, nagios-server, nagiosserver, |            | 開始します                              |
 |(Y/N)              | nagios 例: ptconfigure nagios install/                 |            |                                         |
 |                   | ptconfigure nagiosserver install                       |            |                                         |
 +-------------------+--------------------------------------------------------+------------+-----------------------------------------+
 |Install Nagios     | コマンドラインで使用することができる4つの別のパラメ    | N          | システムは、インストール·プロセスを     |
 |Server Install?    | ータがある。NagiosServer, nagios-server, nagiosserver, |            | 停止し、                                |
 |(Y/N)              | nagios 例: ptconfigure nagios install/                 |            |                                         |
 |                   | ptconfigure nagiosserver install|                      |            |                                         |
 +-------------------+--------------------------------------------------------+------------+-----------------------------------------+



利点
--------------

* ネットワーク サービス (SMTP、POP3、HTTP、NNTP、ICMP、SNMP、FTP、SSH) の監視
* マイクロソフトを含む、ネットワーク オペレーティング システムの大半上のホスト リソース (プロセッサの負荷、ディスクの使用状況、システムのログ)    の監視 Windows NSClient + + プラグインまたは MK を確認してください。
* プローブ （温度、アラーム、等) をネットワーク経由で収集したデータを送信する能力を持っているのような何かを監視 具体的には書かれたプラグイン
* Nagios リモート プラグイン エグゼキュータを介してリモートで実行されるスクリプトによる監視
* リモート監視サポートされている SSH や SSL を通して暗号化されたトンネル。
* 簡単に独自のサービスを開発することができます、単純なプラグインの設計選択の彼らのツールを使用してのニーズに応じて、チェックします。
  (シェル スクリプト, C++, Perl、Ruby、Python、PHP, c#、等.)
* グラフのプラグイン利用可能なデータ
* 並列サービス チェック
* の検出とダウンしているホスト間の区別をできるように、「親」ホストを使用してネットワークのホスト階層を定義する機能 または到達不能
* 連絡通知サービスまたはホストの問題が発生するし、（電子メール、ポケットベル、SMS、またはを介して任意のユーザー定義のメソッドを介して解決を得る
  プラグイン システム)
* 積極的な問題解決のためのサービスまたはホストのイベント中に実行するイベント ハンドラーを定義する能力
* 自動ログ ファイルのローテーション
* 冗長系監視ホストを実装するためのサポート
* 省略可能なウェブ ・ インターフェイスは、現在のネットワーク状態、通知、問題の履歴、ログファイルなどを表示するため。
* テキスト ファイルではなく、データベースを介してデータ ストレージ
 

