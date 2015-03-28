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


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter local source file path
 /home/kevells/Desktop/graphs
 Enter remote target file path
 /home/murali/Desktop/graphs
 [Pharaoh Logging] Opening SFTP Connections...
 [192.168.1.4]Connection failure. Will not execute commands on this box..
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************



 SFTP Put: Success

 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash



 kevell@corp:/# ptconfigure sftp get

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
 Please Enter remote SSH Port
 22
 ***********************************
 *   Due to a software limitation, *
 *    The user that you use here   *
 *  will have their command prompt *
 *    changed to PHARAOHPROMPT     *
 *  ... I'm working on that one... *
 *  Exit program to stop (CTRL+C)  *
 ***********************************
 Enter Server Info:
 Please Enter SSH Server Target Host Name/IP
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter remote source file path
 /home/murali/Desktop/graphs
 Enter local target file path
 /hoem/kevells/Desktop/graphs1
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] [192.168.1.4] Executing SFTP Get...
 [Pharaoh Logging] No SFTP Object
 [Pharaoh Logging] 
 [Pharaoh Logging] [192.168.1.4] SFTP Get Completed...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
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




 

