==================
JenkinsSudoNoPass
==================

あらすじ
------------

ジェンキンスさんは、人気のビルド サーバーです。ジェンキンスさんはソフトウェア開発のための継続的な統合サービスを提供します。Jenkinssudonopass は、システム sudo ファイルにエントリを隣接するようにユーザーを容認します。これはパスワードを持つ関数ユーザー ジェンキンスを入れてください。これは Ubuntu のために適して、
centOS。

ヘルプ コマンド
-----------------------

ヘルプ コマンド同様目的に関してユーザーを管理するように jenkinssudonopass モジュールに含まれているオプションについて。ヘルプ コマンドは jenkinssudonopass の代替パラメーターが一覧表示されます。また、版に jenkinssudonopass を使用するための構文について説明します。Jenkinssudonopass のヘルプ コマンドは以下の通りです。


.. code-block:: bash

	ptconfigure Jenkinssudonopass help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、jenkinssudonopass の下で help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure JenkinsSudoNoPass help
 ******************************


  This command allows you to add an entry to the system sudo file that will
  allow your Jenkins user to have passwordless sudo. This is required for
  quite a few of the Jenkins builds provided by Golden Contact, as Jenkins
  will perform test execution, software installs and more, silently.

  JenkinsSudoNoPass, jenkinssudonopass, jenkins-sudo-nopass, jenkins-sudo-passwordless

        - install
        Installs the Jenkins sudo without password entry
        example: ptconfigure jenkins-sudo-nopass install

 ------------------------------
 End Help
 ******************************



インストール
-----------------

このコマンドは、パスの単語エントリなしジェンキンス sudo をインストールする承認します。ユーザーが jenkinssudonopass をインストールするとき、次のコマンドをインストールするユーザーをガイドします。


.. code-block:: bash

                ptconfigure Jenkinssudonopass install

このコマンドを入力した後、システムはユーザーの願い求めています。他のプロセスのスクリーン ショットを介してインストールをについて説明します。


.. code-block:: bash

 kevell@corp:/# ptconfigure jenkinssudonopass install
 Install Sudo w/o Pass for Jenkins User? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Jenk Sudo Ps        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-2682022801.sh
 chmod 755 /tmp/ptconfigure-temp-script-2682022801.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-2682022801.sh Permissions
 Executing /tmp/ptconfigure-temp-script-2682022801.sh
 The following will be written to /etc/sudoers
 Please check if it looks wrong
 It may break your system if wrong !!!
 jenkins ALL=NOPASSWD: ALL
 Temp File /tmp/ptconfigure-temp-script-2682022801.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsSudoNoPass: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
--------------

.. cssclass:: table-bordered


 +-----------------------------+------------------------------------------------------+------------+-----------------------------------------+
 | パラメーター                | 代替パラメーター                                     | オプション | コメント                                |
 +=============================+======================================================+============+=========================================+
 |Install sudo w/o for         | その代わりjenkinssudonopassの、                      | Y          | ユーザーは、Yと入力することができ、     |  
 |Jenkins user? (Y/N)          | 次の代替を使用することもできる: JenkinsSudoNoPass,   |            | インストールプロセスを続行したい場合    |
 |                             | jenkins-sudo-nopass, jenkins-sudo-passwordless       |            |                                         |
 +-----------------------------+------------------------------------------------------+------------+-----------------------------------------+
 |Install sudo w/o for         | その代わりjenkinssudonopassの、                      | N          | ユーザーは、Nと入力することができ、     |
 |Jenkins user? (Y/N)          | 次の代替を使用することもできる: JenkinsSudoNoPass,   |            | インストールプロセスを終了したい場合は  |
 |                             | jenkins-sudo-nopass, jenkins-sudo-passwordless|      |            |                                         |
 +-----------------------------+------------------------------------------------------+------------+-----------------------------------------+


利点
------------

* オープン ソースの連続的な統合のプロセス。
* Jenkinssudonopass は、自動化ビルドです。
* ビルドと削除ヒューマン エラー問題、スクリプトによってコンピューターは反復的なタスクを実行する時だけで良いです。
* Jenkinssudonopass の展開に時間を費やす必要があります。
* 汎用性と柔軟性。




