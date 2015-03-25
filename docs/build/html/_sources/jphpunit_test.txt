========
PhpUnit
========

概要
----------

Phpunit は、tesingkamen で PHP のプログラミング言語用の単体テスト フレームワークです。Php のテスト スイートを初期化し、pttest に人気となったある発祥した単体テスト フレームワークのアーキテクチャのインスタンスです。


2 つの方法で機能します。Init であり、実行します。Ubuntu や centos を使用する価値があります。.

Helpコマンド
---------------

ヘルプ コマンド同様目的に関してユーザーをリードとして、Phpunit モジュールに含まれているオプションについて。Help コマンドは、pttest モジュールの下に Phpunit の代替パラメーターを一覧表示されます。また、ユーザーのマシンを初期化するための構文について説明します。Phpunit のヘルプ コマンドを以下に示します。

.. code-block:: bash
	
		pttest phpunit help

このモジュールのための利点を追加する非大文字小文字を区別ヘルプ コマンドの構文です。次のスクリーン ショット下システムを検出する help コマンドについてユーザーを視覚化します。

.. code-block:: bash

 kevell@corp:/# pttest PHPUnit help
 ******************************


  This command allows you to initialize a PHPUnit test suite.

  PHPUnit, phpunit

        - init, initialize
        Initialises the PHPUnit test suite of this project
        example: pttest phpunit init
        example: pttest phpunit initialize

        - execute
        Executes the PHPUnit test suite of this project
        example: pttest phpunit execute

 ------------------------------
 End Help
 ******************************


代替パラメータ
---------------------------

Phpunit のユーザーの代わりに、次の新しいパラメーターを利用できます。

PHPUnit,  phpunit


初期化する
--------------

それはこのプロジェクトの phptest スイートを初期化します。これは、一般的な使用はテストされるクラスのオートローディングを設定するスクリプトを作成するユーザーをように指示できます。Init コマンドは次のとおり、です。

.. code-block:: bash

		pttest phpunit init

入力した後、システムは PHPUnit の初期化として質問することができます？Y/N。これは、次のスクリーン ショットによって説明することができます。

.. code-block:: bash

 kevell@corp:/# pttest phpunit init
 Initialize PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79746566500.sh
 chmod 755 /tmp/ptconfigure-temp-script-79746566500.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79746566500.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79746566500.sh
 Temp File /tmp/ptconfigure-temp-script-79746566500.sh Removed
 Creating /tmp/ptconfigure-temp-script-57284647129.sh
 chmod 755 /tmp/ptconfigure-temp-script-57284647129.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-57284647129.sh Permissions
 Executing /tmp/ptconfigure-temp-script-57284647129.sh
 Temp File /tmp/ptconfigure-temp-script-57284647129.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitInit: Success

 ------------------------------
 Installer Finished
 ******************************


Execute
-------------

この execute pttest の PHPUnit のテスト スイートを実行するユーザーに役立ちます。ユーザーはインタプリタの対話型のセッションでコマンドを入力可能性があります。 またはシステム プログラムは人間の介入無しのバッチ プロセスで実行できます。次のコマンドを使用するには、phpunit を実行します。


.. code-block:: bash

		pttest phpunit execute

コマンドの入力後それ質問します。以下のイメージによって視覚化することができます。

.. code-block:: bash

 kevell@corp:/# pttest phpunit execute
 Execute PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-23757829034.sh
 chmod 755 /tmp/ptconfigure-temp-script-23757829034.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23757829034.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23757829034.sh
 /tmp/ptconfigure-temp-script-23757829034.sh: 3: /tmp/ptconfigure-temp-script-23757829034.sh: phpunit: not found
 Temp File /tmp/ptconfigure-temp-script-23757829034.sh Removed
 Creating /tmp/ptconfigure-temp-script-85280710426.sh
 chmod 755 /tmp/ptconfigure-temp-script-85280710426.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-85280710426.sh Permissions
 Executing /tmp/ptconfigure-temp-script-85280710426.sh
 Temp File /tmp/ptconfigure-temp-script-85280710426.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitExec: Success

 ------------------------------
 Installer Finished
 ******************************


オプション
--------------


.. cssclass:: table-bordered

 +------------------------------+-------------+--------------------------------------------------+
 | パラメータ                   | オプション  | 注釈                                             |
 +==============================+=============+==================================================+
 |Initialize Phpunit? (Y/N)	| Yes	      | PHPUnitはpttestの下で初期化することができます    |
 +------------------------------+-------------+--------------------------------------------------+
 |Execute Phpunit? (Y/N)	| Yes	      | PHPUnitのはpttestの下で実行することができます    |
 +------------------------------+-------------+--------------------------------------------------+
 |Initialize Phpunit/Execute 	| No	      | それは、画面を終了することができます             |
 |Phpunit? (Y/N)|		|	      |					 	         |
 +------------------------------+-------------+--------------------------------------------------+
 


メリット
----------

* PHPUnit は、コードの誤りを検出する、早ければ早いほど、早くそれらを修正することができますそのビューで作成されました。
* すべての単体テスト フレームワークのような PHPUnit はテスト対象のコードのユニットの動作が期待どおりに動作ことを確認するアサーションを使用
  します。
* PHPUnit xml など異なる形式の番号でのテスト結果を出力できます。
* Phpunit はケース非感受性をすることができます。
* Ubuntu や centos 関連 Phpunit 快適さ。

