===================
FireFox24
===================


あらすじ
----------

このモジュールは firefox24 をインストールするために使用します。Ubuntu のリリース バージョンを定期的に更新されます。現在および予想される web 標準を実装しています。長期的なサポートには、新しいハードウェア、セキュリティ パッチおよびクラウド コンピューティング インフラストラクチャに更新プログラム用の更新プログラムが含まれます。それは、Ubuntu とセント OS と快適です。


ヘルプ コマンド
----------------

このコマンドは目標と Firefox24 モジュールの下に利用可能なコマンドについて機能することができます。また、firefox24 をインストールするコマンドについて説明します。インストールの前に、ユーザーはこのヘルプ コマンドは、その機能を説明を読むことができます。

.. code-block:: bash
           
      ptconfigure firefox24 help


次のイメージはまた、このモジュールを明確に理解することができます。


.. code-block:: bash

	Kevell@corp:/# ptconfigure firefox24 help
	******************************


	 This command allows you to install Firefox24.

	 Firefox24, ff24, firefox24

        - install
        Installs the latest version of Firefox 24
        example: ptconfigure firefox24 install

	------------------------------
	End Help
	******************************


インストール
--------------

それはモジュールをインストールする firefox24 ptconfigureの下でちょうど、下記のコマンドを使用して明白なプロセス


.. code-block:: bash
       
  ptconfigure firefox24 install

コマンド キーの後に求めることができます。

Install firefox24?(Y/N)


場合に、ユーザー入力の Y として、firefox24 パッケージからインストールします。その他に、それは、画面を終了できます。次のスクリーン ショットはそれを説明することができます。
 

.. code-block:: bash
        
        kevell@corp:/# ptconfigure Firefox24 install

        Install Firefox? (Y/N) 
        y
        *******************************
        *        Pharaoh Tools        *
        *          Firefox            *
        *******************************
        Creating /tmp/ptconfigure-temp-script-51942043520.sh
        chmod 755 /tmp/ptconfigure-temp-script-51942043520.sh 2>/dev/null
        Changing /tmp/ptconfigure-temp-script-51942043520.sh Permissions
        Executing /tmp/ptconfigure-temp-script-51942043520.sh
        Cloning into 'firefox24'...
        remote: Counting objects: 78, done.
        remote: Total 78 (delta 0), reused 0 (delta 0)
        Unpacking objects: 100% (78/78), done.
        Checking connectivity... done.
        Temp File /tmp/ptconfigure-temp-script-51942043520.sh Removed
        Program Executor Deleted if existed
        ... All done!
        *******************************
        Thanks for installing , visit www.pharaohtools.com for more
        ******************************


        Single App Installer:
        --------------------------------------------
        Firefox24: Success
        ------------------------------
        Installer Finished
        ******************************

                                                       

オプション
--------------

.. cssclass:: table-bordered


 +------------------------+------------------------------------------+----------------+---------------------------------------+
 | パラメータ             | 代替パラメータ                           | 必須           | コメント                              |
 +========================+==========================================+================+=======================================+
 |ptconfigure firefox24   | 3代替パラメータがあります – Firefox24,   | Y(Yes)         | システムがptconfigure下では、         |
 |Install                 | ff24, firefox24                          |                | インストールプロセスを開始します      |
 +------------------------+------------------------------------------+----------------+---------------------------------------+
 |ptconfigure firefox24   | 3代替パラメータがあります – Firefox24,   | N(No)          | システムがptconfigure下では、         |
 |Install                 | ff24, firefox24                          |                | インストールプロセスを停止します|     |
 +------------------------+------------------------------------------+----------------+---------------------------------------+

利点
------------------

* Firefox24 は新しいハードウェアとそのシリーズに日に公開されたすべての更新プログラムの統合のサポートを使用します。
* Firefox24 は、大文字と小文字です。
* プライバシーとセキュリティ対策、スマート検索が可能です。
* それは、Ubuntu や centOS で快適です。
 

