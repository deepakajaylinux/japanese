==================
SystemDetection
==================


概要
----------------

このモジュールはユーザーのマシンの検出を目指してし、手にそれらがユーザーのシステムについてのそれらに必要な情報を提供します。ユーザーのアプリケーション設定を構成する機能を提供するも。アプリケーションの設定のいくつかの例を含む私 sql 管理者、建築、管理者ユーザー、ホスト、バージョン、linux ディストリビューションのタイプで。Ubuntu や centOS で快適です。


Helpコマンド
----------------------

ヘルプ コマンド同様目的に関してユーザーを導くようにシステム検出モジュールに含まれているオプションについて。ヘルプ コマンドはシステムの検出 ptvirtualize モジュールの下に代替パラメーターが一覧表示されます。また、ユーザーのコンピューターを検出するための構文について説明します。システムを検出するための help コマンドを以下に示します。


.. code-block:: bash

		ptvirtualize systemdetection help

このモジュールのための利点を追加する非大文字小文字を区別ヘルプ コマンドの構文です。次のスクリーン ショット下システムを検出する help コマンドについてユーザーを視覚化します。

.. code-block:: bash

 kevell@corp:/# ptvirtualize systemdetection help

 ******************************
 Pharaoh Tools - ptvirtualize
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
----------

検出システムの設定を検出するために使用します。1 つのコマンドを使用して、ユーザーはシステム アプリケーションに関するすべての情報を得ることができます。システムの検出に使用するコマンドは以下の通りです。

.. code-block:: bash

		ptvirtualize systemdetection detect

上記のコマンドをキーイングの後システムの検出プロセスを開始します。システムの検出中に対応するマシンに関する次の情報が報告されます。

Operating System

Linux Type

Distro

Version

Architecture

Host Name

IP Address 0.

IP Address 1.

最後に、検出後、上記について情報述べた機能を明確に報告されます。次のスクリーン ショットは、システムの検出プロセスについてユーザーを示しています。

.. code-block:: bash

 kevellscorp:/# ptvirtualize systemdetection detect

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: kevells
 IP Address 0: 127.0.0.1
 IP Address 1: 192.168.1.19

 ------------------------------
 Detection Finished
 ******************************



代替パラメータ
----------------------------------

システム検出ではなく、次のパラメーターを使用できます。

System Detection

system-detection

system detection

メリット
-------------

* ユーザーは、このシステムの検出を使用してアプリケーション設定を構成できます。
* システムを検出する、ヘルプ コマンドを宣言するために使用されるパラメーターは大文字と小文字を他と比較される間、追加の利点。
* それは裕福な両方セント OS とも Ubuntu のように。
* 保護とセキュリティが可能です。システムと内部プロセスや悪意のある外部のリソースへの防止の害。
  
認証、所有権、および制限付きアクセスは、このシステムの明白な部分です。

* システム管理者は一般的に、ユーザー インターフェイスをとき最初ログイン インチで始まる判断 
* いくつかの最適なパフォーマンスをアセンブリに記述されていますが一般的に、PHP で書かれました。
* システム検出モジュール サポートを提供します： 
* リモート プロセスや通信をホストを特定します。
* 2 つのプロセス間の接続を確立します。
* 開き、必要に応じて、接続を閉じます。




