===========
PTTest
===========

あらすじ
---------

pttest モジュールは、テスト スイートの構成やさまざまなツールやテクノロジの共通のルール セットを使用して実行を処理するためです。スターター アプリケーション、テスト スイートの生成に使用することができ、数分以内の自動テスト実行スクリプト。
このモジュールの pttest ツールの最新バージョンをインストールするを目指しています。

ヘルプ コマンド
----------------

ヘルプ コマンドはタスクを達成するために必要を提供するためにユーザーをガイドします。確認するコマンド、ターミナルの下でのヘルプの使用を次のように与えられる

.. code-block:: bash

	ptconfigure pttest help


次のスナップショットは、help コマンドの絵の表現を与えます。



.. code-block:: bash

 kevell@corp:/# ptconfigure pttest help
 ******************************


  This command allows you to update pttest.

  pttest, cleo, pttest

        - install
        Installs the latest version of pttest
        example: pttest pttest install

 ------------------------------
 End Help
 ******************************


 
インストール
----------------

ファラオのアプリのいずれかをインストールすることをお勧め ptconfigure を通じてです。Ptconfigure を既にインストールした場合なし次のコマンドを使用して pttest インストールすることができます。


.. code-block:: bash

	ptconfigure pttest install

次のスナップショットは、help コマンドの絵の表現を与えます。


.. code-block:: bash

 kevell@corp:/# ptconfigure pttest install
 Install pttest - Update to latest version ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          pttest!         *
 *******************************
 What is the program data directory? Found "/opt/pttest" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/pttest.git'  /tmp/pttest/pttestCloning into '/tmp/pttest/pttest'...
 remote: Counting objects: 909, done.
 remote: Total 909 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (909/909), 361.15 KiB | 87.00 KiB/s, done.
 Resolving deltas: 100% (412/412), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 pttest: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
------------


.. cssclass:: table-bordered

 +------------------------+------------------------+------------+--------------------------------------------------------------------------+
 | のパラメタは           | 代替パラメータ         | オプション | 注釈                                                                     |
 +========================+========================+============+==========================================================================+
 |Install pttest ( Y/N)   | pttest, cleo, pttest   | Yes        | 以前にインストールしたバージョンのシステムチェックは、終了した場合、     |
 |                        |                        |            | それは、最新バージョンを更新あるいはそれが新鮮なパッケージをインスト     |
 |                        |                        |            | ールします。キー '/'ボタンを入力する必要があり、特定のパスのユ           |
 |                        |                        |            | ーザーにプログラムファイルを保存するか、そうでなければ、図に示すように、 |
 |                        |                        |            | デフォルトのパスを使用しています。                                       |
 +------------------------+------------------------+------------+--------------------------------------------------------------------------+
 |Install pttest ( Y/N)   | pttest, cleo, pttest   | No         | インストールプロセスを停止します|                                        |
 +------------------------+------------------------+------------+--------------------------------------------------------------------------+



ユーザーのメリット
----------------------

* 簡単に使用するアクセスおよびインストール
* コーディングは大文字小文字の区別
* 完全なソースコードが利用できるとライセンス コストはありません。

 

