============
Cucumber
============


概要
------------

このモジュールは、初期化およびキュウリのテスト スイートを実行するユーザーを支援します。私たちを見てみましょうどのように初期化し、今後のトピックでキュウリのテスト スイートを実行します。


Helpコマンド
--------------------

ヘルプ コマンドの目的と、モジュールの下に使用可能なオプションに関するユーザーをガイドします。宣言で使用されている代替のパラメーターを示します。それは、pttest の下でキュウリを実行する初期化の構文について説明します。ヘルプを宣言するために使用するコマンドを次に示します。


.. code-block:: bash

		pttest cucumber help

次のスクリーン ショットは、help コマンドの働きについて絵を示しています。


.. code-block:: bash

 kevell@corp:/# pttest cucumber help
 ******************************


  This command allows you to initialize a Cucumber test suite.

  Cucumber, cucumber

        - init, initialize
        Initialises the Cucumber test suite of this project
        example: pttest cucumber init
        example: pttest cucumber initialize

        - execute
        Executes the Cucumber test suite of this project
        example: pttest cucumber execute

 ------------------------------
 End Help
 ******************************


キュウリを初期化する方法
-----------------------------------

初期化に使用されるコマンド pttest 下のキュウリが表示されます。


.. code-block:: bash

		pttest cucumber init

or 

.. code-block:: bash

		pttest cucumber initialize

上記のコマンドを入力した後で示されている初期化のプロセスが発生する、テーブルの下。


.. cssclass:: table-bordered

 +-----------------------------+-----------------------------------------+------------+---------------------------------------+
 | パラメータ                  | 代替パラメータ                          | オプション | 注釈                                  |
 +=============================+=========================================+============+=======================================+
 |Initialize Cucumber? (Y/N)   | の代わりに Cucumber, 我々は使用すること | Y(Yes)     | ユーザーは、 Yとして入力でき          |
 |                             | ができます cucumber また                |            | るのinitを続行したい場合              |
 +-----------------------------+-----------------------------------------+------------+---------------------------------------+
 |Initialize Cucumber? (Y/N)   | の代わりに Cucumber, 我々は使用すること | N(No)      | ユーザーは、Nとして入力することができ |
 |                             | ができます cucumber また                |            | initプロセスを終了したい場合は|       |
 +-----------------------------+-----------------------------------------+------------+---------------------------------------+




最後に pttest キュウリを取得次のスクリーン ショットに示すように初期化されます。

.. code-block:: bash


 kevell@corp:/# pttest cucumber init
 Initialize Cucumber? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Cucumber         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-81470621814.sh
 chmod 755 /tmp/ptconfigure-temp-script-81470621814.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-81470621814.sh Permissions
 Executing /tmp/ptconfigure-temp-script-81470621814.sh
 Temp File /tmp/ptconfigure-temp-script-81470621814.sh Removed
 Creating /tmp/ptconfigure-temp-script-65310697385.sh
 chmod 755 /tmp/ptconfigure-temp-script-65310697385.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-65310697385.sh Permissions
 Executing /tmp/ptconfigure-temp-script-65310697385.sh
 Temp File /tmp/ptconfigure-temp-script-65310697385.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Cucumber: Success

 ------------------------------
 Installer Finished
 ******************************


どのようにキュウリを実行するには
----------------------------------------

Pttest の下でキュウリを実行するために使用されるコマンドが表示されます。


.. code-block:: bash

		pttest cucumber execute

上記のコマンドを入力した後で示されている実行のプロセスが発生する、テーブルの下。

.. cssclass:: table-bordered

 +-----------------------------+-----------------------------------------+------------+-----------------------------------------+
 | パラメータ                  | 代替パラメータ                          | オプション | 注釈                                    |
 +=============================+=========================================+============+=========================================+
 |Execute Cucumber? (Y/N)      | の代わりに Cucumber, 我々は使用すること | Y(Yes)     | ユーザーは、Yとして彼らができ           |
 |                             | ができます cucumber また                |            | る実行入力を続行したい場合              |
 +-----------------------------+-----------------------------------------+------------+-----------------------------------------+
 |Execute Cucumber? (Y/N)      | の代わりに Cucumber, 我々は使用すること | N(No)      | ユーザーは、Nとして入力することができま |
 |                             | ができます cucumber また                |            | す実行プロセスを終了したい場合は|       |
 +-----------------------------+-----------------------------------------+------------+-----------------------------------------+




実行を続行すると、次のスクリーン ショットに示すように実行のプロセスが発生します。


メリット
------------


* それは裕福な両方セント OS とも ubuntu のように。
* 宣言で使用されるパラメーター大文字小文字をしない中に他の人に比べて利点であります。
* このキュウリを初期化し、キュウリのテスト スイートを実行するユーザーことができます。


