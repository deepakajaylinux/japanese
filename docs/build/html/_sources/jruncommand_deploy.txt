=============
Run Command
=============

概要
------------

実行コマンド モジュールを使用すると、オペレーティング システム コマンドを実行することができます。これは主に自動操縦で使用されます。この実行コマンド、ユーザーを使用して、コマンド、またはフロント エンド ユーザーのともバック グラウンドでいずれかを実行する名前を指定できます。実行コマンドを使用してを見てみましょう。


Helpコマンド
---------------------

Help コマンドは、コマンドを実行、その主要な機能、その代替のパラメーター、コマンド、またはフロント エンド ユーザーのともバック グラウンドでいずれかを実行する名前を指定するため、コマンドを実行するため、また構文について使用するコマンドの使用について説明します。Help コマンドを宣言するために使用する構文を次に示します。


.. code-block:: bash

		ptdeploy RunCommand help

次のスクリーン ショットは、help コマンドの働きについて絵を示しています。

.. code-block:: bash

 kevell@corp:/# ptdeploy RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


ファイル名を指定して実行]コマンドを使用する方法
------------------------------------------------------


以下のように実行コマンドを指定するために使用する構文。

.. code-block:: bash

	ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

.. cssclass:: table-bordered

 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 | パラメーター                 | 機能                                          | 使用法                                        |
 +==============================+===============================================+===============================================+
 |command="ls -lah /tmp"	| これは、ユーザーがコマンドとその              | これを使用することにより、ユーザは、その要    |
 |				| 目的を指定することができます。                | 件に従って、独自のコマンドを指定する          |
 |                              |                                               | ことができる。                                |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 |run-as-user="ubuntu"		| ユーザーの名前を指定することができ、          | これを使用することにより、ユーザーは自        |
 |				| このユーザーを使用することにより。            | 分の要件に応じて自分の必要なユーザーロ        |
 |                              |                                               | グインを指定することができます。              |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 |" --background		| それはどこにバックグラウンドで、またはフロン  | これを使用することにより、ユーザは、          |
 |				| トエンドのいずれかで特定のコマンドを実        | その要件に従って使用する、プラットフォーム    |
 |				| 行するには、ユーザが指定することができます|   | を指定することができる。|                     |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+




構文とテーブルすることができます上記のように役立ちます、ユーザー実行コマンドを使用する方法。

.. code-block:: bash

 kevell@corp:/# ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 

 ******************************* 
 *   Golden Contact Computing  * 
 *         Run Command        * 
 ******************************* 
 Use NoHup?: (Y/N) 
 y 
 cd /home/karunakaran 
 su  ubuntu 
 nohup ls -lah /tmp & 
 exit 
 Creating /tmp/ptconfigure-temp-script-56005480696.sh 
 chmod 755 /tmp/ptconfigure-temp-script-56005480696.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-56005480696.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-56005480696.sh 
 No passwd entry for user 'ubuntu' 
 nohup: redirecting stderr to stdout 
 total 92K 
 drwxrwxrwt 10 root        root        4.0K Mar 20 17:06 . 
 drwxr-xr-x 29 root        root        4.0K Mar 20 16:18 .. 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonKEKGVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonMKENVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 10:07 .bamficonN2NXVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonSM8KVX 
 -rwxr-xr-x  1 root        root          58 Mar 20 17:06 ptconfigure-temp-script-56005480696.sh 
 -rw-------  1 karunakaran karunakaran    0 Mar 20 09:50 config-err-UrGst6 
 -rw-------  1 root        root        1000 Mar 20 09:49 .configtest.KiQIacNN 
 -rw-r--r--  1 root        root          33 Mar 20 09:50 cxtracker.start.log 
 drwxr-xr-x  2 root        root        4.0K Mar 20 09:50 hsperfdata_root 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:50 .ICE-unix 
 -rw-r--r--  1 root        root           3 Mar 20 15:40 kk.txt 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 16:58 luh3hawd.tmp 
 srwxrwxrwx  1 mongodb     nogroup        0 Mar 20 09:49 mongodb-27017.sock 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 10:07 .org.chromium.Chromium.VRBmwX 
 srwxrwxr-x  1 karunakaran karunakaran    0 Mar 20 10:06 OSL_PIPE_1000_SingleOfficeIPC_8a32f718ac801a6e525d3030e0878e45 
 -rw-r--r--  1 root        root           0 Mar 20 15:42 papyrusfile 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 14:33 plugtmp 
 drwxr-xr-x  2 root        root        4.0K Mar 20 14:42 ServerBlocktemp 
 -rw-rw-r--  1 karunakaran karunakaran    0 Mar 20 09:50 unity_support_test.0 
 drwxr-xr-x  2 root        root        4.0K Mar 20 13:02 vhosttemp 
 -r--r--r--  1 root        root          11 Mar 20 09:49 .X0-lock 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:49 .X11-unix 
 Temp File /tmp/ptconfigure-temp-script-56005480696.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.gcsoftshop.co.uk for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 
 
 RunCommand: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 


メリット
------------

* ヘルプ コマンドを宣言するために使用されるパラメーター、インストールしない大文字と小文字は他と比較される間、加えられた利点であります。
* それは裕福な両方セント OS とも Ubuntu のように。
* ユーザーは、名前、ユーザーのともバック 
  グラウンドでいずれかを実行するコマンドやフロント エンドを指定できます。
* ヘルプ コマンド実行のコマンドを実行する方法でユーザーのガイド、またその目的。

