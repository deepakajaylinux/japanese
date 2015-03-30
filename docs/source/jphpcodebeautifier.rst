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
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following NEW packages will be installed: 
  php-pear 
 0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 0 B/267 kB of archives. 
 After this operation, 2,287 kB of additional disk space will be used. 
 Selecting previously unselected package php-pear. 
 (Reading database ... 391909 files and directories currently installed.) 
 Preparing to unpack .../php-pear_5.5.9+dfsg-1ubuntu4.7_all.deb ... 
 Unpacking php-pear (5.5.9+dfsg-1ubuntu4.7) ... 
 Processing triggers for doc-base (0.10.5) ... 
 Processing 1 added doc-base file... 
 Setting up php-pear (5.5.9+dfsg-1ubuntu4.7) ... 
 [Pharaoh Logging] Adding Package php-pear from the Packager Apt executed correctly 
 Creating /tmp/ptconfigure-temp-script-40069326632.sh 
 chmod 755 /tmp/ptconfigure-temp-script-40069326632.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-40069326632.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-40069326632.sh 
 pear/PHP_Beautifier is already installed and is the same as the released version 0.1.15 
 install failed 
 Temp File /tmp/ptconfigure-temp-script-40069326632.sh Removed 
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

