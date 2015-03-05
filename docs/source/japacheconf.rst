============
ApacheConf
============

概要
--------

このモジュールの管理およびインストール Apache の設定を支援します。それはあなたの環境の構成を指定します。それは裕福な ubuntu と同様セント OS のように。


Helpコマンド
--------------

Help コマンドは、目的とこのモジュールで使用できるコマンドについて説明します。また、特定のモジュールをインストールするコマンドについて説明します。
宣言に使用できる代替のパラメーターを示します。ヘルプを宣言するために使用されるコマンドが表示されます以下の通り：

.. code-block:: bash

	ptconfigure apacheconf help


スクリーン ショットは、下図のように、このモジュールの下に help コマンドの使用状況を視覚的に表します。


.. code-block:: bash
	
 kevell@corp:/# ptconfigure apacheconf help
 ******************************


  This module lets you install a configuration for Apache HTTP Server. The only commands available are this help
  and install.

  ApacheConf, apache-configure, apache-configuration, apache-conf, apacheconf

        - install
        Installs a configuration for Apache
        example: ptconfigure apacheconf install

 ------------------------------
 End Help
 ******************************


インストール
---------------

単に、下記のコマンドを使用してこのptconfigureの下で特定のツールをインストールする方が簡単です。

.. code-block:: bash
 
  ptconfigure apacheconf install

上記のコマンドを与えた後、ツールは確認します。


.. code-block:: bash

  Install Apache conf? (Y/N)

Y として入力を与える場合、モジュールが正常にインストールします。

またロックファイル PidFile、タイムアウト、キープア ライブ、MaxKeepAliveRequest、キープア ライブ タイムアウトのデフォルト以外の値を指定するいくつかのコマンドがスローされます。場合は、ユーザーが与える Y(Yes) と入力自動的に既定値を修正します。ユーザーは N(No) として入力を与える場合、ユーザーから値について尋ねるでしょう。

インストールでスクリーン ショット下記手順やコマンドについて視覚的に説明する必要があります。

.. code-block:: bash


 kevell@corp:/# ptconfigure apacheconf install
 Install Apache Conf? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Conf!        *
 *******************************
 Set non-default value for LockFile? Default is ${APACHE_LOCK_DIR}/accept.lock (Y/N) 

 Set non-default value for PidFile? Default is ${APACHE_PID_FILE} (Y/N) 

 Set non-default value for Timeout? Default is 300 (Y/N) 

 Set non-default value for KeepAlive? Default is On (Y/N) 

 Set non-default value for MaxKeepAliveRequests? Default is 100 (Y/N) 

 Set non-default value for KeepAliveTimeout? Default is 5 (Y/N) 

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ApacheConf: Success
 ------------------------------
 Installer Finished
 ******************************


オプション
------------

.. cssclass:: table-bordered

 +-------------------------------+---------------------------------------------+---------+------------------------------------------------+
 | パラメーター                  | 代替パラメーター                            | 必要な  | コメント                                       |
 +===============================+=============================================+=========+================================================+
 |Install Apache conf? (Y/N)     | 代わりにApachemoduls、我々は使用すること    | Yes     | ユーザーがYESと入力を与えた場合は、            |     
 |                               | ができますApacheModules, apachemods、       |         | モジュールをインストールします。モジュール。   |
 |                               | Apache-modules こうして                     |         |                                                |
 +-------------------------------+---------------------------------------------+---------+------------------------------------------------+
 |Install Apache conf? (Y/N)     | 代わりにApachemoduls、我々は使用すること    | No      | ユーザーはNOと入力を与えた場合、               |
 |                               | ができますApacheModules, apachemods、       |         | それは、出口を取得します。                     |
 |                               | Apache-modules こうして|                    |         |                                                |
 +-------------------------------+---------------------------------------------+---------+------------------------------------------------+


利点
--------

* モジュールをインストールすると、Apache の構成を管理するエンドユーザーを支援します。
* インストール中に Apache ツール、エンド ・ ユーザーは設計およびこのモジュールを使用して彼らの要件に従って構成を管理できます。
* 場合、既に構成創設以来存在する既存のものが上書きされます。
* それは裕福なセント OS とも Ubuntu のように。
* 宣言で使用されるパラメーターは大文字と小文字を区別する加えられた利点であります。
 

