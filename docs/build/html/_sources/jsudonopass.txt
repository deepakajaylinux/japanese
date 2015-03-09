============
Sudonopass
============

あらすじ
---------------

Sudonopass は、特定のコマンドを root 権限で実行に使用されます。興味深い点は、ユーザー、特定のコマンド sudo を使用して、システムの現在のユーザーのパスワードをユーザーが求められます。ユーザー パスワードを入力して、一度 root 特権を持つコマンドを実行します。これは Ubuntu とセント OS との作業に最適です。

ヘルプ コマンド
-----------------------

このコマンドのヘルプガイド sudonopass モジュールに関するユーザー。これはビジネス ユーザーのすべてのタイプに適しています。ヘルプ コマンド sudonopass モジュールに組み込まれたコマンドの短いリストが表示されます。次のスクリーン ショットは、それを列挙します。

.. code-block:: bash

	kevell@corp:/# ptconfigure SudoNoPass help
	******************************


	 This command allows you to add an entry to the system sudo file that will
	 allow your user to have passwordless sudo. This is required for
	 quite a few of the  builds provided by Golden Contact, as
	 will perform test execution, software installs and more, silently.

	 SudoNoPass, sudonopass, sudo-nopass, sudo-passwordless

        - install
        Installs the sudo without password entry
        example: ptconfigure sudo-nopass install

	------------------------------
	End Help
	******************************

インストール
------------------

Ubuntu Linux システム パッケージに sudonopass をインストールするには、このモジュールを使用してください。


.. code-block:: bash

          ptconfigure sudonopass install

Install sudonopass ?(Y/N)

ユーザーの入力を与え、うんと自動的にインストールされます構成ルート パス アクセスみんなのため。次のスクリーン ショットはそれを説明します。


.. code-block:: bash

	kevell@corp:/# ptconfigure sudo-nopass install
	Install Sudo w/o Pass for User? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         Sudo NoPass!        *
	*******************************
	Enter User To Install As:
	Kevells
	The following will be written to /etc/sudoers
	Please check if it looks wrong
	You may not be able to use Sudo if it is incorrect!!!
	Kevells ALL=NOPASSWD: ALL
	Is this okay? (Y/N) 
	y
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	SudoNoPass: Success
	------------------------------
	Installer Finished
	******************************

オプション
------------


.. cssclass:: table-bordered

 +---------------------------+---------------+----------------------------------------------------------+
 | パラメーター              | オプション    | 出力                                                     |
 +===========================+===============+==========================================================+
 |Install sudonopass         | yes           | それはptconfigureの下sudonopassをインストールします      |
 +---------------------------+---------------+----------------------------------------------------------+
 |Install sudonopass         | No            | それは終了します|                                        |
 +---------------------------+---------------+----------------------------------------------------------+


利点
------------

* Sudonopass は root 権限が特定のコマンド (または特定の時刻) であることを確認しますではなく、完全なセッション
  root 特権の偶発的な誤用が発生します。
* ユーザーは、ユーザーに sudonopass も付与限られた特権を使用できます。ユーザーのコントロールを持っているユーザーしたくない場合に便利です。
  sudonopass をしながらすべてのルートの権限。最もよい利点は、その sudonopass は、root パスワードではなく、ユーザーのログイン パスワードが必要で   す。これは root のパスワードを維持するのに役立ちます プライベートがありますユーザー (sudoer) 時でさえそれを変更する必要を残さない。
* このファイルは sudo と実行の自分の時間を使用して実行されたコマンドに関する情報を提供します。これにより、管理者を維持するには
  信頼されるユーザーのトラック

 

