==========
PHPCS
==========

あらすじ
----------

このモジュールは、レポから php cs をインストールするのに役立ちます。インストール中に、このモジュールは、最新バージョンを取得します。ユーザーは、プログラムのデータ ディレクトリと遺言執行者の場所を指定できます。最後に結果を明確に報告されます。

ヘルプ コマンド
----------------

ヘルプ コマンド同様目的に関してユーザーを導くように php cs モジュールに含まれているオプションについて。また、php の cs をインストールするための構文について説明します。Php cs のヘルプのコマンドは以下の通りです。

.. code-block:: bash

	ptconfigure PHPCS help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットに PHPCS 下 help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCS help 
 ****************************** 

  This command allows you to install PHPCS from a GC Repo. 

  PHPCS 

        - install 
        Installs the latest version of PHPCS 
        example: ptconfigure phpcs install 

        - uninstall 
        Uninstalls the latest version of PHPCS 
        example: ptconfigure phpcs uninstall 

 ------------------------------ 
 End Help 
 ****************************** 


インストール
-------------

PHP の CS をインストールするように、次のコマンドを使用して簡単です：


.. code-block:: bash
	
	ptconfigure PHPCS install

次の操作上のコマンドを入力した後で示すように、表形式に発生します。


.. cssclass:: table-bordered

 +---------------------+----------------------------------------------+-------------+---------------------------------------------------+
 | パラメータ          | 代替パラメータ                               | オプション  | 注釈                                              |
 +=====================+==============================================+=============+===================================================+
 |Install PHPCI? (Y/N) | その代わりPHPCIの、我々はまた、phpci使用す   | Y(Yes)      | ユーザーは、Yと入力することができ、               |
 |                     | ることができます。                           |             | インストールプロセスを続行したい場合              |
 +---------------------+----------------------------------------------+-------------+---------------------------------------------------+
 |Install PHPCI? (Y/N) | その代わりPHPCIの、我々はまた、phpci使用す   | N(No)       | ユーザーは、Nと入力することができ、               |
 |                     | ることができます。                           |             | 、インストールプロセスを終了したい場合は|         |
 +---------------------+----------------------------------------------+-------------+---------------------------------------------------+

ユーザー インストール プロセスの進行を表形式で示すように、次の操作が発生します。

.. cssclass:: table-bordered

 +---------------------+------------------------+-------------------+---------------------------------------------------------------------+
 | パラメーター        | パス                   | オプション        | コメント                                                            |
 +=====================+========================+===================+=====================================================================+
 |Program data         | “/opt/phpunit(対応す   | Yes               | ユーザーがデフォルトのプログラムのデータディレクトリを使用してイ    |
 |directory            | るモジュール)”         |                   | ンストールを続行する場合、それらはYESと入力をすることができます     | 
 |(デフォルト)         |                        |                   |                                                                     |
 +---------------------+------------------------+-------------------+---------------------------------------------------------------------+
 |Program data         | User Specific          | No(エンドス       | ユーザーが自分自身のプログラムデータディレクトリを続行したい場合は、|
 |directory            |                        | ラッシュ)         | 入力Nとして、そして手に、彼らは場所を所有指定することができます。   |
 +---------------------+------------------------+-------------------+---------------------------------------------------------------------+
 |Program executor     | “/usr/bin”             | Yes               | ユーザーがデフォルトのプログラム実行ディレクトリを使用してインスト  |
 |directory            |                        |                   | ールを続行する場合、それらはYESと入力をすることができます           |
 |(デフォルト)         |                        |                   |                                                                     |
 +---------------------+------------------------+-------------------+---------------------------------------------------------------------+
 |Program executor     | User Specific          | No(エンドス       | ユーザーが独自のプログラム実行ディレクトリを続行したい場合は、      |
 |directory            |                        | ラッシュ)         | 入力Nとして、そして手に、彼らは場所を所有指定することができます。|  |
 +---------------------+------------------------+-------------------+---------------------------------------------------------------------+


表形式で示すように、これらの工程の後、結果は、明らかにステータスとともに報告される。以下のスクリーンショットは、インストールとPHPCSのアンインストールに関わるプロセスについてグラフィカルにご説明します。

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS install 
 Install PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-74085209498.sh 
 chmod 755 /tmp/ptconfigure-temp-script-74085209498.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-74085209498.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-74085209498.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 php-pear is already the newest version. 
 0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded. 
 downloading PHP_CodeSniffer-2.3.0.tgz ... 
 Starting to download PHP_CodeSniffer-2.3.0.tgz (464,453 bytes) 
 .............................................................................................done: 464,453 bytes 
 install ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-74085209498.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS uninstall 
 Uninstall PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-50071430908.sh 
 chmod 755 /tmp/ptconfigure-temp-script-50071430908.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-50071430908.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-50071430908.sh 
 uninstall ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-50071430908.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Uninstaller: 
 ------------------------------ 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  





利点
-----------

* このモジュールで更新されたバージョンと PHP の CS をインストールするユーザーを容易にします。
* ユーザーは、プログラムのデータ ディレクトリと遺言執行者のための独自のパスを選択できます。
* ヘルプとインストールの宣言で使用されるパラメーターは大文字と小文字を区別しながら他の人に比べての利点を追加する必要があります。
 

