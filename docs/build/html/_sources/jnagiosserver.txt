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

 kevell@corp:/# ptconfigure nagios help
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
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:

 The following packages have unmet dependencies:
 nagios3 : Depends: nagios3-core (= 3.2.3-3ubuntu1) but it is not going to be installed
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt did not execute correctly
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
 

