=============
RunCommand
=============

あらすじ
-----------

実行コマンド モジュールを使用すると、オペレーティング システム コマンドを実行することができます。これは主に自動操縦で使用されます。この実行コマンド、ユーザーを使用して、コマンド、またはフロント エンド ユーザーのともバック グラウンドでいずれかを実行する名前を指定できます。実行コマンドを使用してを見てみましょう。

ヘルプ コマンド
----------------

Help コマンドは、コマンドを実行、その主要な機能、その代替のパラメーター、コマンド、またはフロント エンド ユーザーのともバック グラウンドでいずれかを実行する名前を指定するため、コマンドを実行するため、また構文について使用するコマンドの使用について説明します。Help コマンドを宣言するために使用する構文を次に示します。

.. code-block:: bash

		ptconfigure RunCommand help

次のスクリーン ショットは、help コマンドの働きについて絵を示しています。



.. code-block:: bash

 kevell@corp:/# ptconfigure RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************

実行コマンドを使用する方法
-----------------------------

実行を指定するために使用する構文コマンドを以下に示します。


.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered


 +-------------------------+--------------------------------------------+-------------------------------------------------------------------+
 | パラメーター            | 関数                                       | 使い方                                                            |
 +=========================+============================================+===================================================================+
 |command=”ls -lah /tmp”   | これは、ユーザーがコマンドとその目的を指   | これを使用することにより、ユーザは、その要件に従って、独自の      |
 |                         | 定することができます。                     | コマンドを指定することができる。                                  |
 +-------------------------+--------------------------------------------+-------------------------------------------------------------------+
 |run-as-user=”ubuntu”     | ユーザーの名前を指定することができ、       | これを使用することにより、ユーザーは自分の要件に応じて自分の必    |
 |                         | このユーザーを使用することにより。         | 要なユーザーログインを指定することができます。                    |
 +-------------------------+--------------------------------------------+-------------------------------------------------------------------+
 |” –background            | これは、ユーザーがどこにバックグラウンド   | これを使用することにより、ユーザは、その要件に従って使用する、    |
 |                         | で、またはフロントエンドのいずれかで特定   | プラットフォームを指定することができる。                          |
 |                         | のコマンドを実行するために指定すること     |                                                                   |
 |                         | ができます。|                              |                                                                   |
 +-------------------------+--------------------------------------------+-------------------------------------------------------------------+

.. code-block:: bash


 kevell@corp:/# ptconfigure run-command install --yes --command="ls -lah /tmp" --run-as-user="kevells" --background

 *******************************
 *        Pharaoh Tools        *
 *         Run Command        *
 *******************************
 Use NoHup?: (Y/N) 
 y
 cd /home/kevells
 su kevells -c ls -lah /tmp
 nohup ls -lah /tmp &
 exit
 Creating /tmp/ptconfigure-temp-script-11430033105.sh
 chmod 755 /tmp/ptconfigure-temp-script-11430033105.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-11430033105.sh Permissions
 Executing /tmp/ptconfigure-temp-script-11430033105.sh
 su: invalid option -- 'a'
 Usage: su [options] [LOGIN] 

 Options:
  -c, --command COMMAND         pass COMMAND to the invoked shell
  -h, --help                    display this help message and exit
  -, -l, --login                make the shell a login shell
  -m, -p,
  --preserve-environment        do not reset environment variables, and
                                keep the same shell
  -s, --shell SHELL             use SHELL instead of the default in passwd

 nohup: redirecting stderr to stdout
 total 17M
 drwxrwxrwt  9 root          root          4.0K Mar 30 20:05 .
 drwxr-xr-x 28 root          root          4.0K Mar 28 17:58 ..
 -rwxr-xr-x  1 root          root           229 Mar 30 10:39 ptconfigure-temp-script-10148944050.sh
 -rwxr-xr-x  1 root          root           155 Mar 30 12:52 ptconfigure-temp-script-1093307841.sh
 -rwxr-xr-x  1 root          root            68 Mar 30 20:05 ptconfigure-temp-script-11430033105.sh
 -rwxr-xr-x  1 root          root           146 Mar 30 15:46 ptconfigure-temp-script-29072719650.sh
 -rwxr-xr-x  1 root          root           261 Mar 30 14:30 ptconfigure-temp-script-39464139952.sh
 -rwxr-xr-x  1 root          root           155 Mar 30 14:03 ptconfigure-temp-script-4842774525.sh
 -rwxr-xr-x  1 root          root            64 Mar 30 19:04 ptconfigure-temp-script-64533089928.sh
 -rwxr-xr-x  1 root          root           229 Mar 30 14:00 ptconfigure-temp-script-78930437679.sh
 -rwxr-xr-x  1 root          root           146 Mar 30 14:03 ptconfigure-temp-script-81890547014.sh
 -rw-r--r--  1 root          root            65 Mar 30 09:53 cxtracker.start.log
 drwxr-xr-x  2 elasticsearch elasticsearch 4.0K Mar 30 09:54 elasticsearch
 drwxr-xr-x  2 elasticsearch elasticsearch 4.0K Mar 30 09:54 hsperfdata_elasticsearch
 drwxr-xr-x  2 root          root          4.0K Mar 30 09:53 hsperfdata_root
 drwxr-xr-x  2 tomcat7       tomcat7       4.0K Mar 30 09:54 hsperfdata_tomcat7
 drwxrwxrwt  2 root          root          4.0K Mar 30 09:54 .ICE-unix
 srwxrwxrwx  1 mongodb       nogroup          0 Mar 30 09:53 mongodb-27017.sock
 -rw-r--r--  1 root          root           15M Mar 13  2014 mysql-server-wsrep-5.6.16-25.5-amd64.deb
 -rw-r--r--  1 root          root          668K Mar 30 14:03 netbeans-8.0-linux.sh
 -rw-r--r--  1 root          root           85K Mar 30 14:03 netbeans-8.0-linux.sh.1
 -rw-r--r--  1 root          root          1.1M Mar 30 15:46 netbeans-8.0-linux.sh.2
 srwxrwxr-x  1 kevells        kevells           0 Mar 30 09:57 qtsingleapp-hipcha-2c5e-3e8
 -rw-rw-r--  1 kevells        kevells           0 Mar 30 09:57 qtsingleapp-hipcha-2c5e-3e8-lockfile
 drwxr-xr-x  2 tomcat7       root          4.0K Mar 30 09:54 tomcat7-tomcat7-tmp
 -r--r--r--  1 root          root            11 Mar 30 09:53 .X0-lock
 drwxrwxrwt  2 root          root          4.0K Mar 30 09:53 .X11-unix
 Temp File /tmp/ptconfigure-temp-script-11430033105.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 RunCommand: Success
 ------------------------------
 Installer Finished
 ******************************


利点
------------

* ヘルプ コマンドを宣言するために使用されるパラメーター、インストールしない大文字と小文字は他と比較される間、加えられた利点であります。
* それは裕福な両方セント OS とも Ubuntu のように。
* ユーザーは、名前、ユーザーのともバック グラウンドでいずれかを実行するコマンドやフロント エンドを指定できます。
* ヘルプ コマンド実行のコマンドを実行する方法でユーザーのガイド、またその目的。
 

