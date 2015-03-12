======================
PHPCodeBeautifier
======================


概要
--------------

PhpCodeBeautifierはそれを提示するユーザ独自の方法に合わせて、コードを再フォーマットに時間を費やすのユーザーを避けるモジュールです。適切な形式では読みやすく、理解し、コードが簡単になります。 PHPビューティは、ユーザーのソースコードを解析し、ユーザーの選択のスタイルでそれをフォーマットします。これは、UbuntuとセントOSでよく実行されます。

Helpコマンド
------------------------

helpコマンドは、とだけでなく、PhpCodeBeautifierモジュールに含まれているオプションについての目的について、ユーザーをリードしています。 helpコマンドは、ptconfigureモジュールの下にPHPコードの代わりのパラメータをリストに表示します。また、ユーザーのコードビューティをインストールするための構文について説明します。 PhpCodeBeautifierためのhelpコマンドを以下に示します。

.. code-block:: bash 

	ptconfigure PHPCodeBeautifier help

このモジュールの利点が追加され、helpコマンド以外の、大文字と小文字を区別するための構文。次のスクリーンショットは、このモジュールの利点が追加されたヘルプコマンド以外の場合の構文の下でhelpコマンドについてユーザに視覚化する。次のスクリーンショットは、PHPコードの下でhelpコマンドについてユーザに視覚化する。


.. code-block:: bash 

 kevell@corp:/# ptconfigure PHPCodeBeautifier help 


 ****************************** 

 This command allows you to update PHPCodeBeautifier. 
 
 PHPCodeBeautifier, phpcodebeautifier 

 - install 
 Installs the latest version of PHPCodeBeautifier 
 example: ptconfigure PHPCodeBeautifier install 

 ------------------------------ 
 End Help 
 ****************************** 



インストール
-----------------

インストールは通常、オペレーティングシステムによって容易にアクセスするために、ローカルコンピュータ上の新しいファイルへのインストールファイルから生成されたコピーされたコードを/が含まれます。これは、フォーマットして、コードを美化する。そのうちのいくつかは冗長な要素を削除することができます。それらを使用して、ユーザが確認し、バックアップを有していなければならないため、ユーザーデータは常に復元することができる。次のコマンドは、PhpCodeBeautifierをインストールするために使用。

.. code-block:: bash 

	ptconfigure PhpCodeBeautifier install 

このモジュールをインストールする際に次のスクリーンショットが現れます。


.. code-block:: bash 


 kevell@corp:/# ptconfigure PHPCodeBeautifier install 

 Install PHPCodeBeautifier? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHPCodeBeautifier!        * 
 ******************************* 
 [Pharaoh Logging] Package php-pear from the Packager Apt is already installed, so not installing 
 Creating /tmp/ptconfigure-temp-script-47226840682.sh 
 chmod 755 /tmp/ptconfigure-temp-script-47226840682.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-47226840682.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-47226840682.sh 
 PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open shared object file: No such file or directory in Unknown on line 0 
 WARNING: "pear/Console_Getopt" is deprecated in favor of "pear/Console_GetoptPlus" 
 Did not download optional dependencies: pear/PHP_DocBlockGenerator, use --alldeps to download automatically 
 WARNING: "pear/DB" is deprecated in favor of "pear/MDB2" 
 Did not download optional dependencies: pear/DB, pear/MDB2, pear/Mail, use --alldeps to download automatically 
 pear/PHP_Beautifier can optionally use package "pear/PHP_DocBlockGenerator" (version >= 1, excluded versions: 1) 
 pear/Log can optionally use package "pear/DB" (version >= 1.3) 
 pear/Log can optionally use package "pear/MDB2" (version >= 2.0.0RC1) 
 pear/Log can optionally use package "pear/Mail" 
 pear/Log can optionally use PHP extension "sqlite" 
 downloading PHP_Beautifier-0.1.15.tgz ... 
 Starting to download PHP_Beautifier-0.1.15.tgz (74,408 bytes) 
 .................done: 74,408 bytes 
 downloading Log-1.12.8.tgz ... 
 Starting to download Log-1.12.8.tgz (46,725 bytes) 
 ...done: 46,725 bytes 
 install ok: channel://pear.php.net/Log-1.12.8 
 install ok: channel://pear.php.net/PHP_Beautifier-0.1.15 
 Temp File /tmp/ptconfigure-temp-script-47226840682.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 
 

 Single App Installer: 
 -------------------------------------------- 
 PHPCodeBeautifier: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  

オプション
-------------

.. cssclass:: table-bordered 

 +--------------------------+-----------------------+-------------+--------------------------------------------+
 | パラメーター             | 代替パラメータ        | オプション  | コメント                                   |
 +==========================+=======================+=============+============================================+
 |Install                   | PhpcodeBeautifier,    | Y           | それはptconfigureの下phpCodeBeautifier     |
 |PhpCodeBeautifier? (Y/N)  | phpcodebeautifier     |             | のインストールが開始さ                     |
 +--------------------------+-----------------------+-------------+--------------------------------------------+
 |Install                   | PhpcodeBeautifier,    | N           | これは、インストールを終了します           |
 |PhpCodeBeautifier? (Y/N)  | phpcodebeautifier|    |             |                                            |
 +--------------------------+-----------------------+-------------+--------------------------------------------+



メリット
-------------

* 視覚的にファイルを処理することを可能にPhpCodeBeautifier。
* PhpCodeBeautifierはその中で85の言語PHPやRuby、HTMLの上で記述されたソースコードをフォーマットすることができます。
* これは、非大文字と小文字の区別である。
* PhpCodeBeautifierはUbuntuとセントのOSで動作するようにスーツ。
* PhpCodeBeautifierは、プレゼンテーションの標準に準拠するプログラムを再フォーマットする特定のユーティリティです。

