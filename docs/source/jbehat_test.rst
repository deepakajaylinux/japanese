=========
Behat
=========

概要
------------

このモジュールでは、behat のテスト スイートを初期化するユーザーことができます。Behat は、php スクリプトのテストに役立ちます。それは有効および無効のテンプレートを強調表示できます。私たちを見てみましょうどのように init に teskingkamen behat を実行し、。


Helpコマンド
---------------------

ヘルプ コマンドの目的と、モジュールの下に使用可能なオプションに関するユーザーをガイドします。宣言で使用されている代替のパラメーターを示します。それは、pttest の下で behat を実行する初期化の構文について説明します。ヘルプを宣言するために使用するコマンドを次に示します。


.. code-block:: bash

 		pttest behat help

次のスクリーン ショットは、help コマンドの働きについて絵を示しています。


.. code-block:: bash

 kevell@corp:/# pttest Behat help
 ******************************


  This command allows you to initialize a Behat test suite.

  Behat, behat

        - init, initialize
        Initialises the Behat test suite of this project
        example: pttest behat init
        example: pttest behat initialize

        - execute
        Executes the Behat test suite of this project
        example: pttest behat execute

 ------------------------------
 End Help
 ******************************


Behatを初期化する方法
-----------------------------

初期化に使用されるコマンド pttest 下 behat が表示されます。


.. code-block:: bash

		pttest behat init

or 

.. code-block:: bash

		pttest behat initialize


上記のコマンドを入力した後で示されている初期化のプロセスが発生する、テーブルの下。


.. cssclass:: table-bordered

 +------------------------+----------------------------------------+------------+---------------------------------------+
 | パラメータ             | 代替パラメータ                         | オプション | 注釈                                  |
 +========================+========================================+============+=======================================+
 |Initialize Behat? (Y/N) | の代わりに Behat, 我々は使用すること   | Y(Yes)     | ユーザーは、 Yとして入力でき          |
 |                        | ができます behat また                  |            | るのinitを続行したい場合              |
 +------------------------+----------------------------------------+------------+---------------------------------------+
 |Initialize Behat? (Y/N) | の代わりに Behat, 我々は使用すること   | N(No)      | ユーザーは、Nとして入力することができ |
 |                        | ができます behat また                  |            | るのinitプロセスを終了したい場合は|   |
 +------------------------+----------------------------------------+------------+---------------------------------------+



最後に pttest behat を取得、次のスクリーン ショットに示すように初期化されます。

.. code-block:: bash

 kevell@corp:/# pttest behat init
 Initialize Behat? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Behat         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-72748278108.sh
 chmod 755 /tmp/ptconfigure-temp-script-72748278108.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-72748278108.sh Permissions
 Executing /tmp/ptconfigure-temp-script-72748278108.sh
 /tmp/ptconfigure-temp-script-72748278108.sh: 3: /tmp/ptconfigure-temp-script-72748278108.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-72748278108.sh Removed
 Creating /tmp/ptconfigure-temp-script-35600300430.sh
 chmod 755 /tmp/ptconfigure-temp-script-35600300430.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-35600300430.sh Permissions
 Executing /tmp/ptconfigure-temp-script-35600300430.sh
 Temp File /tmp/ptconfigure-temp-script-35600300430.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************


どのようにBehatを実行するには
-------------------------------

Pttest の下で behat を実行するために使用されるコマンドが表示されます。


.. code-block:: bash

		pttest behat execute


上記のコマンドを入力した後で示されている実行のプロセスが発生する、テーブルの下。

.. cssclass:: table-bordered 
 
 +-----------------------+----------------------------------------+------------+-----------------------------------------+
 | パラメータ            | 代替パラメータ                         | オプション | 注釈                                    |
 +=======================+========================================+============+=========================================+
 |Execute Behat (Y/N)    | の代わりに Behat, 我々は使用すること   | Y(Yes)     | ユーザーは、 Yと彼らができる            |
 |                       | ができます behat また                  |            | 実行入力を続行したい場合                |
 +-----------------------+----------------------------------------+------------+-----------------------------------------+
 |Execute Behat? (Y/N)   | の代わりに Behat, 我々は使用すること   | N(No)      | ユーザーは、Nとして入力することが       |
 |                       | ができます behat また                  |            | できます実行プロセスを終了したい場合は| |
 +-----------------------+----------------------------------------+------------+-----------------------------------------+


実行を続行すると、次のスクリーン ショットに示すように実行のプロセスが発生します。


.. code-block:: bash

 kevell@corp:/# pttest behat execute
 Execute Behat? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *            Behat!           *
 *******************************
 Creating /tmp/ptconfigure-temp-script-93439425208.sh
 chmod 755 /tmp/ptconfigure-temp-script-93439425208.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-93439425208.sh Permissions
 Executing /tmp/ptconfigure-temp-script-93439425208.sh
 /tmp/ptconfigure-temp-script-93439425208.sh: 2: /tmp/ptconfigure-temp-script-93439425208.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-93439425208.sh Removed
 Creating /tmp/ptconfigure-temp-script-97268122064.sh
 chmod 755 /tmp/ptconfigure-temp-script-97268122064.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-97268122064.sh Permissions
 Executing /tmp/ptconfigure-temp-script-97268122064.sh
 Temp File /tmp/ptconfigure-temp-script-97268122064.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************


メリット
-----------

* Php スクリプトのエラーを識別するユーザーをガイドします。
* ユーザーことができますフレームし、駆動開発の動作を指定する behat の機能を使用します 。
* 初期化と実行のプロセスは、この behat pttestt の下で実行できます。
* それは裕福な両方セント OS とも ubuntu のように。
* パラメーターの宣言で使用しない大文字と小文字は他と比較される間、加えられた利点であり
  ます。


