================
ChromeDriver
================

あらすじ
------------

このモジュールはカール、vim、drush、および zip を含む標準的なツールをお勧めしますいくつかの GC をインストールすることができます。クロムを取得するには、java をインストール、ユーザー ニーズをインストール取得します。私たちの今後のテーマをインストールする方法とこれを使用する方法について参照してください。

ヘルプ コマンド
--------------------

ヘルプ コマンド同様目的に関してユーザーを導くようにクロム ドライバー モジュールに含まれているオプションについて。ヘルプ コマンド クローム ドライバー モジュールの代替パラメーターが一覧表示されます。また、Chrome ドライバ モジュールをインストールするための構文について説明します。クロム ドライバー モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		cleopatra ChromeDriver help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、クロム ドライバーの下で help コマンドについて視覚化します。



.. code-block:: bash

 kevell@corp:/# cleopatra ChromeDriver help

 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  ChromeDriver, chromedriver-server, chromedriver, chromedriver-srv, chromedriverserver

        - install
        Installs ChromeDriver. Note, you'll also need Java installed
        as it is a prerequisite for ChromeDriver
        example: cleopatra chromedriver install

 ------------------------------
 End Help
 ******************************

インストール
---------------

あなたのマシンに chrome のドライバーをインストールように、次のコマンドを使用するだけで実行できます。

.. code-block:: bash

		cleopatra chromedriver install



上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered


 +---------------------+------------------------------------------------------+-------------+-------------------------------------------+
 | パラメーター        | 代替パラメーター                                     | オプション  | コメント                                  |
 +=====================+======================================================+=============+===========================================+
 |Install ChromeDriver | その代わりchromedriver、我々は使用することができます | Y(Yes)      | ユーザーは、Yと入力することができ、       |
 |Server? (Y/N)        | ChromeDriver, chromedriver-server, chromedriver-srv, |             | インストールプロセスを続行したい場合      |
 |                     | chromedriverserver また                              |             |                                           |
 +---------------------+------------------------------------------------------+-------------+-------------------------------------------+
 |Install ChromeDriver | その代わりchromedriver、我々は使用することができます | N(No)       | ユーザーは、Nと入力することができ、       |
 |Server? (Y/N)        | ChromeDriver, chromedriver-server, chromedriver-srv, |             | インストールプロセスを終了したい場合は    |
 |                     | chromedriverserver また|                             |             |                                           |
 +---------------------+------------------------------------------------------+-------------+-------------------------------------------+

	
場合は、ユーザー インストールの実行中に、インストール プロセスの進行プロセスを促す


.. code-block:: bash

	Enter Chrome Driver Version


利用可能な chrome のドライバー バージョンのリストは以下のとおりです。

.. code-block:: bash

 0. 2.0
 1. 2.10
 2. 2.1
 3. 2.11
 4. 2.2
 5. 2.3
 6. 2.4
 7. 2.5
 8. 2.6
 9. 2.7
 10. 2.8
 11. 2.9

ユーザーがそのバージョンの要件に応じて 11 0 から番号を指定します。

後のバージョンを指定するユーザー インストールのプロセスが開始して、次のスクリーン ショットから絵として描かれている完了を取得します。


.. code-block:: bash

 kevell@corp:/# cleopatra chromedriver install

 Install ChromeDriver Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         ChromeDriver        *
 *******************************
 Enter Chrome Driver Version
 (0) 2.0 
 (1) 2.10 
 (2) 2.1 
 (3) 2.11 
 (4) 2.2 
 (5) 2.3 
 (6) 2.4 
 (7) 2.5 
 (8) 2.6 
 (9) 2.7 
 (10) 2.8 
 (11) 2.9 
 11
 PHP Notice:  Undefined index: version in /opt/cleopatra/cleopatra/src/Modules/ChromeDriver/Model/ChromeDriverAllLinux.php on line 42
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/cleopatra-temp-script-26804823734.sh
 chmod 755 /tmp/cleopatra-temp-script-26804823734.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-26804823734.sh Permissions
 Executing /tmp/cleopatra-temp-script-26804823734.sh
 --2015-02-02 21:35:49--  http://chromedriver.storage.googleapis.com//chromedriver_linux64.zip
 Resolving chromedriver.storage.googleapis.com (chromedriver.storage.googleapis.com)... 74.125.236.44, 74.125.236.43, 74.125.236.42, ...
 Connecting to chromedriver.storage.googleapis.com (chromedriver.storage.googleapis.com)|74.125.236.44|:80... connected.
 HTTP request sent, awaiting response... 404 Not Found
 2015-02-02 21:35:52 ERROR 404: Not Found.
 
 mv: cannot stat '/tmp/chromedriver/*': No such file or directory
 unzip:  cannot find or open chromedriver_linux64.zip, chromedriver_linux64.zip.zip or chromedriver_linux64.zip.ZIP.
 Temp File /tmp/cleopatra-temp-script-26804823734.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 ChromeDriver: Success
 ------------------------------
 Installer Finished
 ******************************


利点
------------

* ヘルプ コマンドを宣言するために使用されるパラメーター、インストールしない大文字と小文字は他と比較される間、加えられた利点であります。
* それは裕福な両方セント OS とも Ubuntu のように。
* ユーザーは、インストール中にインストールしたいバージョンを指定できます。

 

