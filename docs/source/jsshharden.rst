=============
Ssh Harden
=============



あらすじ
----------

このモジュールの作成と変更 sshhardens に役立ちます。Ssh を強化する SSH のアカウントのユーザーのためのセキュリティ機能を容易にします。

ヘルプ コマンド
----------------

ヘルプ コマンド目的に関してユーザーをリードし、含まれるオプションについてだけでなく、SSH で硬化モジュール。SSH の代替パラメーターをヘルプ コマンド リストを強化します。SSH を使用する構文についても説明します版を強化します。ヘルプ コマンド SSH 強化する以下のとおりです。


.. code-block:: bash

	ptconfigure SshHarden help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、SSH ハーデン下 help コマンドについて視覚化します。


.. code-block:: bash

	Kevell@corp:/# ptconfigure SshHarden help
	
	******************************


        This command allows you to modify create or modify sshhardens

	SshHarden, sshharden, ssh-harden

        - securify
        Add some security to your SSH accounts
        example: ptconfigure ssh-harden securify

	------------------------------
	End Help
	******************************

版
-----------

SSH 経由で SSH のアカウントのセキュリティを強化、ユーザーの securifying のために使用されるコマンドを次に示します。


.. code-block:: bash

	ptconfigure ssh-harden securify

与えられた上記のコマンドを入力した後を表形式で示すように Ssh 硬化のインストールを開始します。


.. cssclass:: table-bordered

 +--------------------+----------------------------------------------------+-------------+---------------------------------------------+
 | パラメータ         | 代替パラメータ                                     | オプション  | 注釈                                        |
 +====================+====================================================+=============+=============================================+
 |Install Ssh         | 代わりにSsh Hardening の、次の代替を使用する       | Y(Yes)      | ユーザーは、Yと入力することができ、         |
 |Hardening? (Y/N)    | こともできます。SshHarden, sshharden, ssh-harden.  |             | インストールプロセスを続行したい場合        |
 +--------------------+----------------------------------------------------+-------------+---------------------------------------------+
 |Install Ssh         | 代わりにSsh Hardening の、次の代替を使用する       | N(No)       | ユーザーは、Nと入力することができ、         |
 |Hardening? (Y/N)    | こともできます。SshHarden, sshharden, ssh-harden.  |             | インストールプロセスを終了したい場合は|     |
 +--------------------+----------------------------------------------------+-------------+---------------------------------------------+


Ssh のインストール強化 securifying できるようにする場合は、ユーザーの代金、ssh のユーザーのアカウントを取得を開始しました。実行のプロセスが発生する間、sshd の設定ファイルを取得することを禁止ルート ssh ログインを変更と同様、sshd の設定ファイルの変更を禁止パスワード ベースの ssh ログイン。最後に、それは再起動、ssh サービスし、完成した Ssh ハーデン変更の結果を表示します。次のスクリーン ショットは絵上記のプロセスについて説明します。


.. code-block:: bash

	Kevell@corp:/# ptconfigure ssh-harden securify
	
	Install Ssh Hardening? (Y/N) 
	y
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 175
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 149
	[Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
	[Pharaoh Logging] /etc/ssh/sshd_config modified to disallow root ssh login
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 175
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 149
	[Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
	[Pharaoh Logging] /etc/ssh/sshd_config modified to disallow password based ssh login
	[Pharaoh Logging] Restarting ssh service
	ssh stop/waiting
	ssh start/running, process 17375
	******************************


	SshHarden Modifications:
	--------------------------------------------

	Ssh Hardening: Success

	------------------------------
	SshHarden Mods Finished
	******************************

利点
------------

* この Ssh ユーザー SSH アカウントのセキュリティ機能を有効にエンハンサーとして行為を強化します。
* ヘルプと securifying で使用されるパラメーター、インストール操作しない大文字と小文字は、追加の利点と比較している間であります。その他。
* このモジュールを有効にします変更の ssh を強化を禁止しているルート ssh 設定ログイン、パスワード ベースの ssh ログイン。
 

