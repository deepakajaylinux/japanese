=========
PHPDox
=========

概要
------------

このモジュールは、最新バージョンのPHPののDoxをインストール中に、ユーザーが容易になる。 phpdoxは、PHPのソースコードから、例えば、HTML形式でAPIドキュメントを生成するためのドキュメントジェネレータである。このモジュールは、PHPのDoxのをインストールするのに役立つかを私たちは見てみましょう。

helpコマンド
---------------------

helpコマンドは、とだけでなく、Phpdoxモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それはPhpdoxモジュールの別のパラメータを示しています。また、Phpdoxモジュールをインストールするための構文について説明します。 Phpdoxモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash 
	 
	ptconfigure Phpdox help 

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、Phpdox下に、helpコマンドについてあなたを視覚化。


.. code-block:: bash 

 kevell@corp:/# ptconfigure PHPDox help 

 ****************************** 

 This command allows you to update PHPDox. 

 PHPDox, phpdox 

  - install 
  Installs the latest version of Docker 
 example: ptconfigure phpdox install 

 ------------------------------ 
 End Help 
 ****************************** 

インストール
----------------

ユーザーがマシンにphpdoxをインストールするために使用するコマンドを以下に示します。

.. code-block:: bash 
 
	ptconfigure phpdox install 

表形式で示すように、上記のコマンドを入力した後、次の処理が発生します。


.. cssclass:: table-bordered 

 
 +--------------------------+-------------------+-------------+--------------------------------------------------------+
 | パラメータ               | 代替パラメータ    | オプション  | コメント                                               |
 +==========================+===================+=============+========================================================+
 |Install PHPDox? (Y/N)     | phpdox, PHPDox    | Y(Yes)      | ユーザーは、Yと入力することができ、                    |
 |                          |                   |             | インストールプロセスを続行したい場合                   |
 +--------------------------+-------------------+-------------+--------------------------------------------------------+
 |Install PHPDox? (Y/N)     | phpdox, PHPDox    | N(No)       | ユーザーは、Nと入力することができ、                    |
 |                          |                   |             | インストールプロセスを終了したい場合は|                |
 +--------------------------+-------------------+-------------+--------------------------------------------------------+



ユーザーがインストールを進行する場合は、インストールのプロセスは、以下のスクリーンショットのようになります。


.. code-block:: bash 

 kevell@corp:/# ptconfigure phpdox install 

 Install PHPDox? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHPDox!        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-27804177792.sh 
 chmod 755 /tmp/ptconfigure-temp-script-27804177792.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-27804177792.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-27804177792.sh 
 --2015-01-28 15:42:36--  http://phpdox.de/releases/phpdox.phar 
 Resolving phpdox.de (phpdox.de)... 188.94.27.6 
 Connecting to phpdox.de (phpdox.de)|188.94.27.6|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 801185 (782K) [application/phar] 
 Saving to: Ã¢¬Ëphpdox.pharÃ¢¬¢ 

 100%[=======================================================================================================>] 8,01,185    11.7KB/s   in 2m 9s  

 2015-01-28 15:44:47 (6.08 KB/s) - Ã¢¬Ëphpdox.pharÃ¢¬¢ saved [801185/801185] 
 
 PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open 
 shared object file: No such file or directory in Unknown on line 0 
 Sorry, but your PHP environment is currently not able to run phpDox due to 
 the following issue(s): 
 
 ext/xsl not installed/enabled 

 Please adjust your PHP configuration and try again. 



 Oups... phpDox encountered a problem and has terminated! 

 It most likely means you've found a bug, so please file a report for this 
 and paste the following details and the stacktrace (if given) along: 

 PHP Version: 5.5.9-1ubuntu4.5 (Linux) 
 PHPDox Version: 0.7.0 
 ErrorException: E_CORE_WARNING 
 Location: Unknown (Line 0) 
 
 PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open shared object 
 file: No such file or directory 

 No stacktrace available 
 

 phpDox 0.7.0 - Copyright (C) 2010 - 2015 by Arne Blankerts 

 Temp File /tmp/ptconfigure-temp-script-27804177792.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 PHPDox: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 

メリット
-----------

* ヘルプとインストールで使用されるパラメータは、他の人に比べながら、追加的な利点である大文字と小文字を区別しません。
* これは、Ubuntuと同様にセントOSの両方に裕福なです。
* この意志モジュールが更新されたバージョンでphpdoxをインストールします。
* モジュールがすでにユーザマシン内に存在されている場合は、それがすでに存在しているようにメッセージが表示されます。

