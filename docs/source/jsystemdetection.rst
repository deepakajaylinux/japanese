==================
System Detection
==================

概要
-------------

このモジュールは、ユーザーのマシンを検出することを目的と手にユーザーがシステムに関して、それらに彼らに必要な情報を提供します。また、自分のアプリケーションの設定を構成するには、ユーザーに機能を提供します。アプリケーションの設定のためのいくつかの例は、MySQLの管理者ユーザ、ホスト、パスが含まれています。

helpコマンド
----------------------

helpコマンドは、とだけでなく、システムの検出モジュールに含まれているオプションについての目的について、ユーザーをリードしています。システム検出の別のパラメータからhelpコマンドの一覧。また、ユーザーのマシンを検出するための構文について説明します。システム検出のためのhelpコマンドを以下に示します。

.. code-block:: bash

	ptconfigure systemdetection help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、システム検出の下でhelpコマンドについてあなたを視覚化。

.. code-block:: bash

	kevell@corp:/# ptconfigure SystemDetection help
	******************************


	This is a default Module and provides you with a method by which you can configure Application Settings.
	 You can configure default application settings, ie: mysql admin user, host, pass

	 SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptconfigure system-detection detect

	------------------------------
	End Help
	******************************

検出
------------

システム検出のために使用するコマンドを以下に示す。

.. code-block:: bash

	ptconfigure systemdetection detect

上記のコマンドを入力した後、システム検出の処理が開始されます。システム検出時に対応する機械に関する以下の情報のが報告されています。

* オペレーティング·システム
* Linuxのタイプ
* ディストリビューション
* バージョン
* アーキテクチャ
* ホスト名
* IPアドレス0。
* IPアドレス1。

最後に、検出後、上記の特徴に関する情報が明確に報告されている。以下のスクリーンショットは、システム検出の過程についてあなたを示している。

.. code-block:: bash

        Kevell@corp:/# ptconfigure system-detection detect
	******************************


	Systems Detection:
	--------------------------------------------

	Operating System: Linux
	Linux Type: Debian
	Distro: Ubuntu
	Version: 14.04
	Architecture: 64
	Host Name: Kevells
	IP Address 0: 127.0.0.1
	IP Address 1: 192.168.1.3

	------------------------------
	Detection Finished
	******************************

別のパラメータ
------------------------

その代わりsystemdetectionの、以下のパラメータを使用することができる。

* SystemDetection
* system-detection

メリット
------------

* ユーザーは、このシステムの検出を使用してアプリケーションの設定を構成することができます。
* helpコマンドを宣言するために使用されるパラメータは、システムの検出は、と比較しながら、付加的な利点である大文字と小文字を区別しません
  他人。
* これは、裕福な両方セントOSで、同様のUbuntuのようです。
