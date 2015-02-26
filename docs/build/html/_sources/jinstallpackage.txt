===============
InstallPackage
===============


あらすじ
------------------

インストール パッケージは、差動ロジック出力高速クロック分配回路でよく使用されます。このコマンドは、ビルド サーバー、dev クライアント、テスト サーバー、開発サーバー、生産パッケージをインストールするユーザーを提供します。このコマンドの主な機能は、ソフトウェアの事前に構成された一覧には。Ubuntu や CentOS を適しています。

ヘルプ コマンド
-----------------------

ヘルプ コマンド同様目的に関してユーザーを導くように installpackage モジュールに含まれているオプションについて。Help コマンドは、ptconfigure モジュールの下に installpackage の代替パラメーターを一覧表示されます。また、インストールするための構文について説明します。Installpackage モジュールのヘルプ コマンドを以下に示します。

.. code-block:: bash

		ptconfigure installpackage help


次のスクリーン ショットは、installpackage モジュールの完全な努力を示しています。


.. code-block:: bash

 kevell@corp:/# ptconfigure InstallPackage help

 ******************************


  This command is part of Core and provides you  with a method by which you can perform some default CLI Installs of
  different types of box.

  InstallPackage, installpackage, installpack, install-pack, install, inpack, install-package

    - dev-client
      install a dev client machine for you to work on, a bunch of IDE's, DB's and a complete set of the
      tools you need to start work immediately.
      example: ptconfigure install autopilot dev-client

    - dev-server
      Install the preconfigured list of software for a developers server.
      example: ptconfigure install autopilot dev-server

    - test-server
      Install the preconfigured list of software for a testing server.
      example: ptconfigure install autopilot test-server

    - build-server
      Install the preconfigured list of software for a build server.
      example: ptconfigure install autopilot test-server

    - production
      Install the preconfigured list of software for a production server.
      example: ptconfigure install autopilot test-server

 ------------------------------
 End Help
 ******************************
 


インストール
---------------

インストールには、更新されたバージョンで、インストールを行うために必要な installpackage のインストールが含まれます。それは ptconfigure の下で Installpackage モジュールをインストールするマニフェスト プロセスです。ちょうど、下記のコマンドを使用して Installpackage


.. code-block:: bash

	ptconfigure installpackage Install

それは質問攻めにコマンド入力活性化後。

ユーザーが [はい] を入力するときに自動的にシステムからのチェックと Installpackage がインストールされます。ない場合、インストールを終了します。次のスクリーン ショットは、Installpackage とその機能を示しています。


.. code-block:: bash




代替パラメーター
-------------------------------

宣言で定義することができます、代替パラメーターを次に示します。

InstallPackage, installpackage, installpack, install, inpack, installpackage.

Dev-client
---------------

このコマンドは、ユーザーはすぐに作業を開始する必要があるツールの完全なセットとデータベースの統合の開発環境の束上で動作する使用されます。次のコマンドをクライアントの dev の機械に使用されます。


.. code-block:: bash

		ptconfigure install autopilot dev-client


上記の当該コマンドとして入力後プロセスのインストールを開始します。

次のスナップショットはその機能を示しています。


.. code-block:: bash



開発サーバ
----------------

このコマンドを使用して、インストールする開発者向けのサーバー ソフトウェアのリストをあらかじめ。自動操縦装置はこのプロセスで重要な役割を果たします。これらの機能を正常に動作するには、ptconfigure はこのコマンドを使用して dev サーバーを推奨します。

.. code-block:: bash

		ptconfigure install autopilot dev-server


スクリーン ショットは、その機能についてユーザーをガイドします。


.. code-block:: bash

テスト サーバー
-----------------

ここでは自動操縦機能テスト サーバーで主要な役割。サーバーをテストするためのソフトウェアの構成済みのリストをインストールする使用します。テスト ソフトウェアもご利用いただけます。次のコマンドは、テスト サーバーをインストールするために使用します。



.. code-block:: bash

		ptconfigure install autopilot test-server



スクリーン ショットは、その機能についてユーザーをガイドします。



.. code-block:: bash



サーバーを構築します。
------------------------

このコマンドのインストールに使用するビルド サーバーのソフトウェアのリストをあらかじめ。自動操縦装置はこのプロセスで重要な役割を果たします。これらの機能を正常に動作するには、ptconfigure はこのコマンドを使用してビルド サーバーを推奨します。


.. code-block:: bash

	ptconfigure install autopilot build-server



スクリーン ショットは、その機能についてユーザーをガイドします。



.. code-block:: bash

生産
-----------------

このインストールに使用するコマンドは本番サーバのソフトウェアのリストをあらかじめ。自動操縦装置はこのプロセスで重要な役割を果たします。これらの機能を正常に動作するには、ptconfigure はこのコマンドを使用して運用サーバーを推奨します。


.. code-block:: bash

		ptconfigure install autopilot build-server

スクリーン ショットは、その機能についてユーザーをガイドします。


.. code-block:: bash



利点
-------------

* 非大文字小文字を区別します。
* Ubuntu や CentOS で裕福な。
* Dev サーバー、クライアント開発、生産、ビルド サーバー、テスト サーバーのインストールはこのモジュールの追加の利点です。
* 自動操縦は重要な役割を果たします。

