===================
SystemDetection
===================


概要
-----------

このモジュールはユーザーのマシンの検出を目指してし、手にそれらがユーザーのシステムについてのそれらに必要な情報を提供します。ユーザーのアプリケーション設定を構成する機能を提供するも。いくつかの例では、アプリケーションの設定を含む mysql 管理者、建築、管理者ユーザー、ホスト、バージョン、linux ディストリビューションのタイプで。Ubuntu で、セント快適です OS。


Helpコマンド
---------------

ヘルプ コマンド同様目的に関してユーザーを導くようにシステム検出モジュールに含まれているオプションについて。ヘルプ コマンドはシステムの検出 pttest モジュールの下に代替パラメーターが一覧表示されます。また、ユーザのマシンを検出するための構文について説明します。システムを検出するための help コマンドを以下に示します。

.. code-block:: bash

		pttest systemdetection help

ヘルプ コマンドの構文は、大文字と小文字がこのモジュールのための利点を追加します。次のスクリーン ショットを下システムを検出する help コマンドについて視覚化します。

.. code-block:: bash

 kevell@corp:/# pttest systemdetection help
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


Detect
----------- 

ユーザーがシステム設定を検出するために、特定のコマンドの下システム アプリケーションに関するすべての情報を取得は。

.. code-block:: bash
	
		pttest systemdetection detect

Systemは、下記の詳細を提供して終わる。

* Operating System
* Linux Type
* Distro
* Version
* Architecture
* Host Name
* IP Address 0.

次のスクリーン ショットは、システムの検出プロセスについて示しています。


.. code-block:: bash

 kevell@corp:/# pttest system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: kevells
 IP Address 0: 172.16.201.1
 IP Address 1: 172.16.39.1
 IP Address 2: 192.168.1.16

 ------------------------------
 Detection Finished
 ******************************


代替パラメータ
----------------------------------

システム検出ではなく、次のパラメーターを使用できます。

* SystemDetection
* system-detection
* systemdetection


メリット
-------------

* ユーザーは、このシステムの検出を使用してアプリケーション設定を構成できます。
* システムを検出する、ヘルプ コマンドを宣言するために使用されるパラメーター大文字小文字が区別されません中に他の人に比べて、
  追加の利点があります。
* それは裕福な両方セント OS とも Ubuntu のように。
* 保護とセキュリティが可能です。システムと内部プロセスや悪意のある外部のリソースへの防止の害。認証、所有権、および制限付きアクセスは、
  このシステムの明白な部分です。
* システム管理者が一般的に、ユーザー インターフェイスをとき最初ログイン インチで始まる判断 
* いくつかの最適なパフォーマンスをアセンブリに記述されていますが一般的に、PHP で書かれました。
 



  


