=======
SFTP
=======


概要
-------------

このモジュールは、別に 1 つのシステムからファイルを転送するのに支援します。アップロードしたり、システムにファイルをダウンロードできます。自動化が可能です。Put し、get オプションでは、このモジュールで利用できます。また、仮想ボックスを管理します。それは Ubuntu と cenOS とユーザーフレンドリーです。


Helpコマンド
-------------------------

Help コマンドは、指定されたコマンドに関する情報を見つけるために使用します。Ptvirtualize の下でセキュリティで保護されたファイル転送 Protocol(SFTP) の機能の変更について、ユーザーはこのヘルプ コマンドを使用できます。


.. code-block:: bash

		ptvirtualize  sftp help


次のスクリーンショットは、あなたをガイド。

.. code-block:: bash

 kevell@corp:/# ptvirtualize sftp help

 ******************************
 Pharaoh Tools - ptvirtualize
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


代替パラメータ
---------------------------------

2 つの代替パラメーターが利用できます。彼らには SFTP と sftp です。Sftp を使用して、代わりに、ユーザーは SFTP を使用できます。

Put
------

ファイル転送は、リモート サーバーにローカルから実行できます。このプット オプションはサーバーのユーザー詳細を要求します。次のコマンドは、プット オプションのために使用します。

.. code-block:: bash

		ptvirtualize  sftp put – yes –source=”/tmp/file” – target=”/home/user/file”

次のスクリーン ショットはこのコマンドの使用方法を示します。

.. code-block:: bash

 kevell@corp:ptconfigure sftp put
 
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


SFTP on server group? Y/N

もしその後、 Yのようなユーザ入力

SSh timeout section?

ユーザが値を入力しなければならない

Please enter remote ssh port

Default value is 22. ユーザーが任意の値を入力することができます

Enter environments configured in project? (Y/N)

ユーザーは、それがロードを開始し、その後、Yを入力する必要があります。

Enter local source file path?

ユーザは、ファイル·パスを入力しなければならない

そして、すべてが接続されます。

Nとして、ユーザ入力した場合、それを終了することができる。



Get
-------

ファイル転送は、ローカル サーバーをリモートから実行できます。サーバー グループの入力をユーザーに要求します。次のコマンドを使用するオプションを取得します。


.. code-block:: bash

		ptvirtualize  sftp get – yes –source=”/tmp/file” – target=”/home/user/file”

次のスクリーンショットは、それを説明しています。


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds

 Please Enter remote SSH Port

 Use Environments Configured in Project? (Y/N) 

 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter remote source file path

 Enter local target file path

 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************


SFTP on server group? Y/N

もしその後、 Yのようなユーザ入力

SSh timeout section?

ユーザが値を入力しなければならない

Please enter remote ssh port

Default value is 22. ユーザーが任意の値を入力することができます

Enter environments configured in project? (Y/N)

ユーザーは、それがロードを開始し、その後、Yを入力する必要があります。

Enter local target file path?

ユーザは、ローカルターゲットファイルパスを入力する必要が

そして、すべてが接続されます。

Nとして、ユーザ入力した場合、それを終了することができる。以下のスクリーンショットは、その機能を示しています。


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 N
 ******************************


 Shell Result: Failure
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************



オプション
-------------

.. cssclass:: table-bordered

 +------------------------+---------------------------+--------------------------------------------------------------+
 | パラメータ             | 代替パラメータ            | 注釈                                                         |
 +========================+===========================+==============================================================+
 |put                     | SFTP, sftp        	      | Source to target - ファイルが転送できる                      |
 +------------------------+---------------------------+--------------------------------------------------------------+
 |get			  | SFTP, sftp                | Path to source - ファイルには、リモートシステムからダウンロ  |  
 |                        |                           | ードすることができます|                                      |
 +------------------------+---------------------------+--------------------------------------------------------------+




オプション
-------------

* 遠隔地からマルチ サーバー。
* 指定したファイルは使用可能なエラー メッセージが来る。
* Accessability は許可せずに困難です。
* 自動的に上書きする場合に既にファイルの場合は存在します。
* 非大文字小文字を区別します。
* 秘密保持とセキュリティが可能です。


