=======
SFTP
=======

あらすじ
-----------

このモジュールは、別に 1 つのシステムからファイルを転送するのに支援します。アップロードしたり、システムにファイルをダウンロードできます。自動化が可能です。Put し、get オプションでは、このモジュールで利用できます。それはあなたの環境の構成を指定します。それはユーザーフレンドリー Ubuntu とセント OS。

ヘルプ コマンド
-----------------

Help コマンドは、指定されたコマンドに関する情報を見つけるために使用します。SFTP の機能への変更についてこのヘルプ コマンドを使用できます。

.. code-block:: bash

 		ptconfigure sftp help



次のスクリーン ショットは、あなたをご案内いたします。


.. code-block:: bash


 kevell@corp:/# ptconfigure sftp help
 ******************************


  This command handles SFTP Transfer Functions.

  SFTP, sftp

        - put
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure sftp put
        example: ptconfigure sftp put --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp put --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

        - get
        Will ask you for details for servers, then copy a file or directory from remote to local
        example: ptconfigure sftp get
        example: ptconfigure sftp get --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp get --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

 ------------------------------
 End Help
 ******************************



インストール
---------------

会社として、そして個人として、SFTP は各パートナーの技術課題、そのエンジニア リングの要件を満たすこと、彼らのビジネス目標を満たすに専用されています。それはモジュールをインストールする SFTP ptconfigure の下でちょうど、下記のコマンドを使用して明白なプロセス



.. code-block:: bash

		ptconfigure SFTP put



コマンドし、システムは、問題を提起する与えた後


Install SFTP server group? Y/N


その後 Y として入力した場合


SSh timeout section?


ユーザーが値を入力するには


Please enter remote ssh port

既定値は 22 です。ユーザーが任意の値を入力できます。


Enter server host IP? 

ユーザーがユーザー名、パスワード、およびキーのパスを入力します。


Add another server?

ユーザー入力 Y として彼がある新しいサーバー名を入力する場合

それからすべては接続されます。

N 以前として入力した場合はサーバー名がアクセスできます。


次のスクリーン ショットは、あなたをご案内いたします。


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds
 90
 Please Enter remote SSH Port
 22
 Use Environments Configured in Project? (Y/N) 
 N
 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter local source file path
 /root/vv
 Enter remote target file path
 /root/gg/vv
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************



オプション
------------

.. cssclass:: table-bordered

 +---------------+-------------------------------------+-------------------------------------------------------------------+
 | パラメータ    | 代替パラメータ                      | 注釈                                                              |
 +===============+=====================================+===================================================================+
 |put            | 2代替パラメータがあります。-        | 対象とするソース - ファイルを転送することができます               |
 |               | SFTP, sftp                          |                                                                   |
 +---------------+-------------------------------------+-------------------------------------------------------------------+
 |get            | 2代替パラメータがあります。-        | ソースへのパス - ファイルがリモートシステムからダウンロード       |
 |               | SFTP, sftp                          | することができます|                                               |
 +---------------+-------------------------------------+-------------------------------------------------------------------+


利点
-------------

* 遠隔地からマルチ サーバー。
* 指定したファイルは使用可能なエラー メッセージが来る。
* Accessability は許可せずに困難です。
* 自動的に上書きする場合に既にファイルの場合は存在します。
* 非大文字小文字を区別します。
* 秘密保持とセキュリティが可能です。

ほとんどの技術技術の課題と彼らの成功を有効にする顧客の解決は SFTP の使命と情熱です。




 

