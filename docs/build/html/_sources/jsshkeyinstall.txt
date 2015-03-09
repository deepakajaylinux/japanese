===============
SshKeyInstall
===============

あらすじ
----------------

Ssh 鍵のインストール インストール ssh キー新しいユーザー用に使用します。認証は、パスワード認証よりも安全です。これは、システムがインターネット上に表示される場合に特に重要です。公開鍵認証、認証エンティティを持つ公開キーと秘密キー。各キーは、特別な数学的なプロパティを持つ多数です。Ubuntu や CentOS を適しています。

ヘルプ コマンド
-------------------------

ヘルプ コマンド目的に関してユーザーをガイドし、オプションについてに含まれるだけでなくからモジュールを取り付けます。それは Sshkeyinstall モジュールの代替パラメーターが一覧表示されます。また、Sshkeyinstall モジュールをインストールするための構文について説明します。Sshkeyinstall モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash
 
		ptconfigure Sshkeyinstall help

Help コマンドを宣言する構文非大文字と小文字は、追加の利点があります。次のスクリーン ショットは Sshkeyinstall の下で help コマンドについてユーザーを視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyInstall help

 ******************************


  This command allows you to install an SSH Public key for a user

  SshKeyInstall, sshkeyinstall, ssh-key-install

        - public-key
        Add an SSH Public Key to an account
        example: ptconfigure ssh-key-install public-key
        example: ptconfigure ssh-key-install public-key --yes --public-key-data="zzzzz"
        example: ptconfigure ssh-key-install public-key --yes --public-key-file="id_rsa.pub" --user-name=dave

 ------------------------------
 End Help
 ******************************



インストール
------------------

インストールには、更新されたバージョンで、インストールを行うために必要な Sshkeyinstall のインストールが含まれます。それはモジュールをインストールする Sshkeyinstall ptconfigure Sshkeyinstall の下でちょうど、下記のコマンドを使用してマニフェスト プロセスです。


.. code-block:: bash

 		ptconfigure  Sshkeyinstall  public-key

それは質問攻めにコマンド入力活性化後。

ユーザーが [はい] を入力するときに自動的にシステムからのチェックと Sshkeyinstall がインストールされます。ない場合、インストールを終了します。次のスクリーン ショット demonstSshkeyinstallte Sshkeyinstall それ。


オプション
--------------

.. cssclass:: table-bordered

 +------------------------+-------------------------------------------------+-------------+--------------------------------------------+
 | パラメーター           | パラメーターの代替                              | オプション  | コメント                                   |
 +========================+=================================================+=============+============================================+
 |Install Sshkeyinstall?  | 代わりに使用したの SshKeyInstall我々は使用す    | Y           | それはファラオのツールでptconfigure下      | 
 |(Y/N)                   | ることができますSshkeyinstall, ssh-key-install  |             | Sshkeyinstallをインストールします          |
 +------------------------+-------------------------------------------------+-------------+--------------------------------------------+
 |Install Sshkeyinstall?  | 代わりに使用したの SshKeyInstall我々は使用す    | N           | システム出口インストール                   |
 |(Y/N)                   | ることができますSshkeyinstall, ssh-key-install| |             |                                            |
 +------------------------+-------------------------------------------------+-------------+--------------------------------------------+


利点
----------------

* Sshkeyinstall は Ubuntu や CentOS で裕福です
* Sshkeyinstall ホールド アップ非大文字小文字を区別することができます。
* Sshkeyinstall は柔軟です
* Sshkeyinstall 使用インストールから
* Sshkeyinstall セキュリティをサポートします。
 

