PTTest
==============

概要
------------

pttestは、PHPを用いてテスト構成と実行の自動化管理を目指す。

これは、テストスイートの構成および実行を処理するためのツールと技術の範囲でルールの共通セットを使用しています。

これは、言語やテストツールの広い範囲でテストを実行するための共通APIを提供します。ユーザーは、ほとんど、あるいは必要に応じて余分な構成の複雑なテストスイートを実行することができます。これは、手動またはオペレーティングシステムを使用してユーザーテストに栄養を与えると手に環境安定性を確保します。

これは、オブジェクト指向と拡張可能な、モジュラーである。ユーザーは、フレームと彼らの要求に応じて、独自のモジュールを追加することができ、必要に応じて余分なモジュールを感じているのであれば。

それは、構成管理、テストの自動化管理、自動展開、ビルドとリリース管理、より、 PHPのコードで実装されているすべての、すべてを包み込むファラオツールスイートの一部です。


helpコマンド
-------------------

あなたが特定のモジュールの目的を知りたい場合は、次のように単にコマンドを入力します。

.. code-block:: bash

		pttest ModuleName help

このコマンドは、その特定のモジュールの使用法とは、ユーザーが実行できるアクションで使用可能なオプションを提供します。下のスクリーンショットは、 pttestの下でhelpコマンドを使用してbehatモジュールの使用方法を説明しています。

helpコマンドも宣言で使用できる代替パラメータを示します。



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

インストール
----------------

pttestのインストールは、可用性と、ユーザーの要件に応じて2つの方法で行うことができます。 pttestをインストールする彼ら2つの方法があります。

* Installing pttest via ptconfigure	
* Installing the pttest without depending on ptconfigure.

ptconfigure経由pttestインストール
---------------------------------------------

ユーザーは自分のマシンでptconfigureを持っている場合、それは、次のコマンドを使用してpttestをインストールするための簡単な方法は、次のとおりです。

.. code-block:: bash

		sudo ptconfigure pttest install --yes --guess

ptconfigureに依存せずにpttestのインストール
--------------------------------------------------------------

ユーザーは応じて、彼らは、次のコマンドを使用することができptconfigureを使用せずにpttestをインストールしたい場合：

.. code-block:: bash

		sudo apt-get install php5 git

.. code-block:: bash

	git clone https://github.com/phpengine/pttest && sudo php pttest/install-silent

or

希望のユーザーは、インストール時に場所を指定するために、以下のコマンドは、予測可能である


.. code-block:: bash

		git clone https://github.com/phpengine/pttest && sudo php pttest/install

使用して、可能なモジュールにする方法
------------------------------------

pttestツールを使用する方法を私たちは最初、単に入力し、見てみましょう

.. code-block:: bash

		pttest

このコマンドはpttestの下で利用可能なモジュールのすべての名前が一覧表示されます。以下のスクリーンショットは、視覚的にあることを示している。

.. code-block:: bash

 kevell@corp:/# pttest 
 ******************************


 PTTest by Golden Contact Computing
 -------------------

 About:
 -----------------
 pttest is for Test Automation. It can be used to generate starter test suites for your applications,
 and automated test execution scripts within minutes.

 By providing an common API by which to execute tests in a wide range
 of languages and test tools, you can run complex test suites across a range of platforms with little to no
 extra configuration.

 -------------------------------------------------------------

 Available Commands:
 ---------------------------------------

 Autopilot - ptconfigure Autopilot - User Defined Installations
 Behat - Behat - Initialize or Execute a Behat Test Suite
 Cucumber - Cucumber - Initialize or Execute a Cucumber Test Suite
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 PHPUnit - PHPUnit - Initialize or Execute a PHPUnit Test Suite
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Testify - Testifyer - Creates default tests for your project

 ******************************

PTTestモジュールと遊ぶ
------------------------------------

.. toctree::
   :maxdepth: 6
   


 jbehat_test
 jcucumber_test
 jenvironmentconfig_test
 jphpunit_test
 jsystemdetection_test
 jtemplating_test


