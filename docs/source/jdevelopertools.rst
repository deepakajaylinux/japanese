=================
DeveloperTools
=================

あらすじ
----------------

Devtools モジュール インストールより簡単、Devtools で定義された構造に従ってパッケージを作成します。またエディターを通して、あなたのパッケージをテストしやすくなります。このパッケージ内のモジュール、優れたアイデアを持っている： だけでなく、それがユーザ パッケージより信頼性の高い長期的に、意外な方法で開発プロセスも簡素化されます。これは、Ubuntu や centOS に適しています。

ヘルプ コマンド
------------------------

Devtools パッケージの開発は非常に簡単になります: それは構造のためのコード、パッケージ開発のサイクルをサポートするために効率的なツールを追加する既存の規則で動作します。Devtools、パッケージが開発されるユーザーの既定のレイアウトするたびに、ユーザーが大量のコードを書いたはそう簡単になります。

.. code-block:: bash

                ptconfigure devtools help

次のスクリーン ショットは、それについて説明します。


.. code-block:: bash

 kevell@corp:/# ptconfigure devtools help
 ******************************


  This command allows you to install a set of Developer Tools. These include
  Geany IDE, Bluefish IDE, Kompozer IDE and Emma DB Manager.

  DeveloperTools, devtools, dev-tools

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure devtools install

 ------------------------------
 End Help
 ******************************



インストール
------------------

インストールには規定または操作の準備がインストールされている機器を作るに必要なサービスへの接続が含まれます。それはモジュールをインストールする devtools ptconfigureの下でちょうど、下記のコマンドを使用してマニフェスト プロセスです。

.. code-block:: bash


 ptconfigure devtools install

それは質問攻めにコマンド入力活性化後。

ユーザーが [はい] を入力するときに自動的にシステムからのチェックと devtools がインストールされます。ない場合、インストールを終了します。次
スクリーン ショットは、それを示しています。


.. code-block:: bash


 kevell@corp:/# ptconfigure devtools install
 Install Developer Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         Devel Tools!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  geany-common
 Suggested packages:
  libvte9
 The following NEW packages will be installed:
  geany geany-common
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 3,808 kB of archives.
 After this operation, 9,872 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe geany-common all 1.23.1+dfsg-1 [2,709 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe geany amd64 1.23.1+dfsg-1 [1,100 kB]
 Fetched 3,808 kB in 4min 54s (12.9 kB/s)
 Selecting previously unselected package geany-common.
 (Reading database ... 182047 files and directories currently installed.)
 Preparing to unpack .../geany-common_1.23.1+dfsg-1_all.deb ...
 Unpacking geany-common (1.23.1+dfsg-1) ...
 Selecting previously unselected package geany.
 Preparing to unpack .../geany_1.23.1+dfsg-1_amd64.deb ...
 Unpacking geany (1.23.1+dfsg-1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up geany-common (1.23.1+dfsg-1) ...
 Setting up geany (1.23.1+dfsg-1) ...
 Preparing to unpack .../bluefish-data_2.2.5-1_all.deb ...
 Unpacking bluefish-data (2.2.5-1) ...
 Selecting previously unselected package bluefish-plugins.
 Preparing to unpack .../bluefish-plugins_2.2.5-1_amd64.deb ...
 Unpacking bluefish-plugins (2.2.5-1) ...
 Selecting previously unselected package bluefish.
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for shared-mime-info (1.2-0ubuntu3) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up bluefish-data (2.2.5-1) ...
 Setting up bluefish-plugins (2.2.5-1) ...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/AppConfig.php on line 115
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 DeveloperTools: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
-------------

.. cssclass:: table-bordered

 +------------------------+------------------------------------------------+----------------+-------------------------------------------+
 | パラメーター           | 代替パラメータ                                 | オプション     | 注釈                                      |
 +========================+================================================+================+===========================================+
 |Install devtools?(Y/N)  | 我々は使用することができます                   | Y(Yes)         | それはptconfigure下のエディタとデータベ   |
 |                        | DeveloperTools, devtools, dev-tools            |                | ースdevtoolsをインストールします          |
 +------------------------+------------------------------------------------+----------------+-------------------------------------------+
 |Install devtools?(Y/N)  | 我々は使用することができます                   | N(No)          | システム出口インストール                  |
 |                        | DeveloperTools, devtools, dev-tools|           |                |                                           |
 +------------------------+------------------------------------------------+----------------+-------------------------------------------+


利点
-------------

* パッケージの開発プロセスを促進します。
* 野生にあなたのパッケージを解放に役立ちます
* 簡単にエディターとデータベースをインストールするように。
* 迅速なデバッグ
* -オンザフライでのスタイルの変更 - クイック スタイルの変更、ユーザーもする必要はありません、テキスト エディターを使用しています。ユーザーは、特  定を調べることができます。ページ上の要素、どのスタイルが適用されているを確認します。
 

