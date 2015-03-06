=========
Logging
=========

あらすじ
------------------

このモジュールはコントロール パネルと必要に応じて php ログに情報を記録します。

このモジュールを使用してセンサーを通してデータを収集、データ分析し保存、収集と分析の結果を出力するプロセス。ログは、システムのコントロール パネルをインストールし、データを分析にまた意味します。非大文字小文字の区別は、このモジュールの王冠です。これは、スーツ Ubuntu とセントで動作する OS。

ヘルプ コマンド
-----------------------

このコマンドは目標と ptconfigure モジュールの下に、ログで使用できるコマンドについて機能することができます。また、ログ モジュールをインストールするコマンドについて説明します。インストールの前に、ユーザーはこのヘルプ コマンドは、その機能を説明を読むことができます。

.. code-block:: bash
        
	        ptconfigure logging help


次のスクリーン ショットは、help コマンドを可視化できます。


.. code-block:: bash


 kevell@corp:/# ptconfigure Logging help

 ******************************


  Use this to log a message to the Console, and optionally also the php error log.

  Logging, logging

        - log
        Logs a message to the console and optionally the php log
        example: ptconfigure logging log --log-message="Here is something logging to the console and error log"
        example: ptconfigure logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************

インストール
-----------------

これらのインストール手順はコントロール php ログです。インストールしより詳細な情報を ptconfigure を構成する方法についての互換性と要件、基本的な手順についての情報を説明します。このコマンドは目標と ptconfigure ログ モジュールの下に利用可能なコマンドについて機能することができます。また、ログ モジュールをインストールするコマンドについて説明します。インストールの前に、ユーザーはこのヘルプ コマンドは、その機能を説明を読むことができます。


.. code-block:: bash
        
                ptconfigure logging  log



次のスクリーン ショットは、help コマンドを可視化できます。


.. code-block:: bash

 kevell@corp:/# ptconfigure logging log 

 Install Logging? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Logging: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
------------

.. cssclass:: table-bordered

 +------------------------------+-----------------------------------------+---------------+--------------------------------------------+
 | パラメーター                 | 代替パラメーター                        | オプション    | コメント                                   |
 +==============================+=========================================+===============+============================================+
 |ptconfigure logging Install   | 我々は使用することができますLogging,    | Y             | システムがptconfigure下にログ処理を開始し  |
 |                              | logging                                 |               |                                            |
 +------------------------------+-----------------------------------------+---------------+--------------------------------------------+
 |ptconfigure logging Install   | 我々は使用することができますLogging,    | N             | システムがptconfigure下にログ処理を停止し  |
 |                              | logging|                                |               |                                            |
 +------------------------------+-----------------------------------------+---------------+--------------------------------------------+


利点
-------------

* リアルタイム データの可視化
* 非大文字小文字の区別
* ユーザ機能
* テラバイト級のデータ ストレージ
* ネットワーク接続
* よくで行うには Ubuntu とセント OS
 

