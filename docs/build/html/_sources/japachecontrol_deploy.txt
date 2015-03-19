================
Apache Control
================

概要
-------------

このモジュールはApacheのサーバの制御機能を処理することを目的とデフォルトのモジュールの一つである。これは、Apacheサーバで実行されるべき必要な制御機能を可能にし、容易にする。私たちは、制御機能とApacheサーバーのこれらの制御機能を処理に関与してどのようにこのモジュールの働きと目的を見てみましょう。

helpコマンド
---------------------

helpコマンドは、この特定のモジュールを処理し、使用する方法をユーザーにつながる簡単なユーザーガイドとして機能します。
Apacheの制御下helpコマンドの構文を以下に示します。

.. code-block:: bash

	ptdeploy ApacheControl help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。 helpコマンドも宣言で使用することができる別のパラメータを示しています。次のスクリーンショットは、Apacheのコントロール下に、helpコマンドについてあなたを視覚化。

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

Apacheサーバに含まれる4つの基本的な制御機能は、次のとおりです。

* Start
* Stop
* Restart
* Reload

制御機能を定義する3つの方法がある。我々は、機能を開始する取る場合、それは、以下に示すように、ユーザーの必要に応じて3つの異なる方法で定義することができる。

.. code-block:: bash
		
	ptdeploy ApacheControl start

または

.. code-block:: bash

	ptdeploy ApacheControl start --yes --guess

または

.. code-block:: bash

	ptdeploy ApacheControl start --yes --apache-command="apache2"


私たちは今後のトピックで宣言する3つの異なる構文の使用方法を見てみましょう。

代替パラメータ
-------------------------------

次の宣言で定義することができる代替パラメータは次のとおりです。

ApacheControl, apachecontrol, apachectl

機能を開始
--------------------

ユーザーがApacheの制御機能を起動したい場合のように、次の構文を使用することができます。

.. code-block:: bash

	ptdeploy ApacheControl start

（これはapcheサーバの制御機能を定義する構文の一タイプである）
上記のようにコマンドを入力した後、以下のステップが実行されます。

ステップ1：Do you want to start Apache? (Y/N).

ユーザーは、YまたはNを指定する必要が

ステップ2：What is the apache service name?

(0) apache2

(1) httpd

ユーザーは、要件ごとに0または1かどうかを指定する必要があります。

Apacheのサービス名の入力を取得した後、それはプロセスを開始します。

次のスクリーンショットは、絵画的に開始処理を示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol start
 Do you want to Start Apache? (Y/N)
 y
 What is the apache service name?
 (0) apache2
 (1) httpd
 0
 Starting Apache...
 * Starting web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************

ストップ機能
------------------

ユーザーがApacheの制御機能を停止したい場合のように、次の構文を使用することができます。

.. code-block:: bash

	ptdeploy apachecontrol stop --yes --guess

（これは、構文の第二のタイプは、Apacheサーバの制御機能を定義している）

推測オプションは、特定の定義された機能のデフォルト値を実行するために使用することができる。

Ubuntuのためにapche2はデフォルト値です。

セントのOSのhttpdの場合はデフォルト値です。

次のスクリーンショットは、絵画的に推測オプションの停止機能と目的についてあなたを示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol stop --yes --guess
 Stopping Apache...
 * Stopping web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************

ファンクションを再起動する
---------------------------------------------

ユーザーがApacheの制御機能を再起動したい場合のように、次の構文を使用することができます。

.. code-block:: bash
	
	ptdeploy apachecontrol restart --yes --apache-command="apache2"

（これはapcheサーバの制御機能を定義する構文の三種類である）

ユーザーは、必要なApacheのコマンドの値を指定するには、構文のこの第三のタイプを使用することができます。以下に示すように、スクリーンショットは、構文および絵画的機能を再起動する方法のこの第三のタイプを示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol restart --yes --apache-command="apache2"
 Restarting Apache...
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globa lly to suppress this message
 * Restarting web server apache2
  
  ....done.
 ******************************


 1Apache Controller Finished
 ******************************

機能のリロード
----------------------------

ユーザーがApacheの制御機能をリロードしたい場合のように、次の構文を使用することができます。

.. code-block:: bash

	ptdeploy apachecontrol reload

または

.. code-block:: bash

	ptdeploy apachecontrol --yes --guess

または

.. code-block:: bash

	ptdeploy apachecontrol --yes --apache-command="apache2"

リロード機能は、再起動せずにApacheサーバをリロード実行します。

メリット
-----------

* これは、セント-OSとUbuntuの両方で行うことがよくある。
* 宣言に使用されるパラメータは、他の人に比べながら、付加的な利点である、大文字と小文字を区別しません。
* 宣言に使用された3つの異なる構文があり、利用者は、要件ごとに、それらの間でいずれかを選択できます。
* 3異なる構文リロード、再起動、停止、開始の4つのすべての制御機能に適用されます。
