=================
Selenium Server
=================


あらすじ
-----------

セレンは、ポータブル ソフトウェア フレームワーク web アプリケーションのテストです。セレンはテスト スクリプト言語 (セレン IDE） を習得することがなくテストを作成するための録音/再生ツールを提供します。また人気のあるプログラミング言語、Java、c#、Groovy、Perl、PHP、Python、Ruby などの数のテスト ドメイン固有言語 (Selenese) [1] テストを記述するを提供します。テストは、最新の web ブラウザーに対して実行できます。セレンの Windows、Linux、および Macintosh プラットフォームで展開します。

私たちを見てみましょうどのようにこのモジュール促進セレン サーバーをインストールするユーザーについて。

ヘルプ コマンド
--------------------

Help コマンドと同様、目的に関するユーザー ガイドとしてセレン サーバー モジュールに含まれているオプションについて。セレン サーバー モジュールの代替パラメーターを示します。また、それをインストールするための構文について説明します。セレン サーバー モジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash

	ptconfigure seleniumserver help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、セレン サーバー モジュールの下に、help コマンドについて視覚化します。



.. code-block:: bash

 kevell@corp:/# ptconfigure SeleniumServer help
 ******************************


  This command allows you to install Selenium Server.

  SeleniumServer, selenium-server, selenium, selenium-srv, seleniumserver

        - install
        Installs Selenium Server. Note, you'll also need Java installed
        as it is a prerequisite for Selenium
        example: ptconfigure selenium install
        example: ptconfigure selenium install --with-chrome-driver # will set the executor command to use default chrome driver


 ------------------------------
 End Help
 ******************************

インストール
----------------

セレン サーバーをインストールするために使用されるコマンドは下記に示されているコマンドを入力するだけです。


.. code-block:: bash

		ptconfigure seleniumserver install


上記のコマンドのスクリーン ショットは以下します。


.. code-block:: bash

 kevell@corp:/# ptconfigure selenium install

 Install Selenium Server? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         Selenium Srv        *
 *******************************
 Enter Selenium Version
 (0) 2.39
 (1) 2.40
 (2) 2.41
 (3) 2.42
 (4) 2.43
 (5) 2.44
 5
 PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/SeleniumServer/Model/SeleniumServerAllLinux.php on line 50
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Command 'git' found
 [Pharaoh Logging] Command 'gitk' found
 [Pharaoh Logging] Command 'git-cola' found
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-96670533394.sh
 chmod 755 /tmp/ptconfigure-temp-script-96670533394.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-96670533394.sh Permissions
 Executing /tmp/ptconfigure-temp-script-96670533394.sh
 --2015-02-12 15:31:34--  http://selenium-release.storage.googleapis.com//selenium-server-standalone-.0.jar
 Resolving selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)... 74.125.236.43, 74.125.236.42, 74.125.236.44, ...
 Connecting to selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)|74.125.236.43|:80... connected.
 HTTP request sent, awaiting response... 404 Not Found
 2015-02-12 15:31:35 ERROR 404: Not Found.
 
 mv: cannot stat ‘/tmp/selenium/*’: No such file or directory
 mv: cannot stat ‘selenium-server-standalone-.0.jar’: No such file or directory
 Temp File /tmp/ptconfigure-temp-script-96670533394.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 SeleniumServer: Success
 ------------------------------
 Installer Finished
 ******************************



オプション
------------


上記のコマンドを入力した後、次の操作が発生します表形式で表示されます。


.. cssclass:: table-bordered

 +------------------+----------------------------------------------------+---------------+-------------------------------------------------+
 | パラメーター     | 代替パラメーター                                   | オプション    | コメント                                        |
 +==================+====================================================+===============+=================================================+
 |Install Selenium  | の代わりに seleniumserver, 我々は使用することがで  | Y(Yes)        | ユーザーは、Yと入力することができ、             |
 |Server? (Y/N)     | きますSeleniumServer, Selenium, selenium-srv ,     |               | インストールプロセスを続行したい場合            |
 |                  | selenium-server.                                   |               |                                                 |
 +------------------+----------------------------------------------------+---------------+-------------------------------------------------+
 |Install Selenium  | の代わりに seleniumserver, 我々は使用することがで  | N(No)         | ユーザーは、Nと入力することができ、             |
 |Server? (Y/N)     | きますSeleniumServer, Selenium, selenium-srv ,     |               | インストールプロセスを終了したい場合は          |
 |                  | selenium-server.|                                  |               |                                                 |
 +------------------+----------------------------------------------------+---------------+-------------------------------------------------+




利点
-----------

* ヘルプとインストールで使用されるパラメーター大文字小文字が区別されません中に他の人に比べて、追加の利点は。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* C#、java、python、php、perl、ruby と同様実行などお好みのプログラミング言語で自動テストを開発することができます。
  クロム、Firefox や IE などブラウザーの別の組合せにそれらのテスト
 

