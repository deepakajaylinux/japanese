======
SFTP
======



概要
--------------

          このモジュールは、別に 1 つのシステムからファイルを転送するのに支援します。アップロードしたり、システムにファイルをダウンロードできます。自動化が可能です。Put し、get オプションでは、このモジュールで利用できます。それはあなたの環境の構成を指定します。それはユーザーフレンドリー Ubuntu とセント OS。

Helpコマンド
-----------------------

Help コマンドは、指定されたコマンドに関する情報を見つけるために使用します。SFTP の機能への変更についてこのヘルプ コマンドを使用できます。


.. code-block:: bash
   
	        ptdeploy SFTP help


次のスクリーンショットは、あなたをガイド。


.. code-block:: bash

 kevell@corp:/# ptdeploy sftp help
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
-----------------

会社として、そして個人として、SFTP は各パートナーの技術課題、そのエンジニア リングの要件を満たすこと、彼らのビジネス目標を満たすに専用されています。それはモジュールをインストールする SFTP ptdeploy の下でちょうど、下記のコマンドを使用して明白なプロセス

.. code-block:: bash
  
		ptdeploy SFTP  install 


コマンドし、システムは、問題を提起する与えた後

Install SFTP server group? Y/N

もしその後、 Yのようなユーザ入力

SSh timeout section?

ユーザが値を入力しなければならない

Please enter remote ssh port

Default value is 22. ユーザーが任意の値を入力することができます

Enter server host IP? 

ユーザーがユーザー名、パスワード、およびキーのパスを入力します。

Add another server?

ユーザー入力 Y として彼がある新しいサーバー名を入力する場合

それからすべては接続されます。N 以前として入力した場合はサーバー名がアクセスできます。

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



 SFTP Put: Success

 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp put --yes --environment-name=karthik --source="/tmp/kk.txt" --target="/tmp/kk.txt" 

 Please Enter SSH Timeout in seconds 
 20 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp put --yes --source="/home/karunakaran/Desktop/readme.txt" --target="/home/karthik/Desktop/readme.txt" 

 Please Enter SSH Timeout in seconds 
 20 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 
 
 SFTP Put: Success 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp get 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 200 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter remote source file path 
 /tmp/testing 
 Enter local target file path 
 /opt/testr 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 
 

.. code-block:: bash

 
 kevell@corp:/# ptdeploy sftp get --yes --environment-name=karthik --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 
 
 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 
 
 kevell@corp:/# ptdeploy sftp get --yes --source="/tmp/testing" --target="/opt/testr" 
 
 Please Enter SSH Timeout in seconds 
 200 
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
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 

 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 



Options
------------


.. cssclass:: table-bordered

 +-------------+------------------------+----------------------+----------------------------------------------+
 | パラメータ  | 代替パラメータ         | オプション           | 注釈                                         |
 +=============+========================+======================+==============================================+
 |put	       | SFTP, sftp             | Source to target     | ファイルが転送できる                         |
 +-------------+------------------------+----------------------+----------------------------------------------+
 |get	       | SFTP, sftp             | Path to source       | ファイルには、リモートシステムからダウンロ   |
 |             |                        |                      | ードすることができます|                      |
 +-------------+------------------------+----------------------+----------------------------------------------+




メリット
----------


* 遠隔地からマルチ サーバー。
* 指定したファイルは使用可能なエラー メッセージが来る。
* Accessability は許可せずに困難です。
* 自動的に上書きする場合に既にファイルの場合は存在します。
* 非大文字小文字を区別します。
* 秘密保持とセキュリティが可能です。


ほとんどの技術技術の課題と彼らの成功を有効にする顧客の解決は SFTP の使命と情熱です。

