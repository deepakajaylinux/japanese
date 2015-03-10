==========
FireFox
==========

あらすじ
-----------

このモジュールは、firefox をインストールするために使用します。Ubuntu のリリース バージョンを定期的に更新されます。現在および予想される web 標準を実装しています。長期的なサポートには、新しいハードウェア、セキュリティ パッチおよびクラウド コンピューティング インフラストラクチャに更新プログラム用の更新プログラムが含まれます。それは、Ubuntu とセント OS と快適です。


ヘルプ コマンド
----------------

このコマンドは目標と Firefox モジュールの下に利用可能なコマンドについて機能することができます。また、firefox をインストールするコマンドについて説明します。インストールの前に、ユーザーはこのヘルプ コマンドは、その機能を説明を読むことができます。

.. code-block:: bash

              ptconfigure firefox help

次のイメージはまた、このモジュールを明確に理解することができます。


.. code-block:: bash

	 kevell@corp:/# ptconfigure firefox help

	 ******************************


	 This command is part of Core and provides you  with a method by which you can install Firefox from your package
         manager

	 Firefox, firefox

        - install
        Installs Firefox
        example: ptconfigure firefox install

	------------------------------
	End Help
	******************************


インストール
-------------------

それはモジュールをインストールする firefox ptconfigureの下でちょうど、下記のコマンドを使用して明白なプロセス


.. code-block:: bash

              ptconfigure firefox install


コマンド キーの後に求めることができます。

Install firefox?(Y/N)


場合に、ユーザー入力の Y として、それは、パッケージから firefox をインストールできます。その他に、それは、画面を終了できます。次のスクリーン ショットはそれを説明することができます。



.. code-block:: bash
	
	kevell@corp:/# ptconfigure firefox install

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
	Cloning into 'firefox'...
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
	Firefox: Success
	------------------------------
	Installer Finished
	******************************



オプション
--------------


.. cssclass:: table-bordered

 +--------------------------+------------------------------------+-------------+--------------------------------------------------+
 | パラメータ               | 代替パラメータ                     | オプション  | 注釈                                             |
 +==========================+====================================+=============+==================================================+
 |ptconfigure firefox       | 我々は使用することができます       | Y(Yes)      | システムは、それらがYとして入力することができ、  |
 |Install                   | Firefox, firefox                   |             | インストール処理を開始する                       |
 +--------------------------+------------------------------------+-------------+--------------------------------------------------+
 |ptconfigure Firefox       | 我々は使用することができます       | N(No)       | システムは、インストール·プロセスを停止し、      |
 |Install                   | Firefox, firefox|                  |             |                                                  |
 +--------------------------+------------------------------------+-------------+--------------------------------------------------+


利点
-------------

* Firefox は新しいハードウェアとそのシリーズに日に公開されたすべての更新プログラムの統合のためのサポートを使用します。
* それは、Ubuntu や centOS で快適です。
* Firefox はケース非感受性です。
* プライバシーとセキュリティ対策スマートな捜索
 

