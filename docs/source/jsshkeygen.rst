============
SshKeygen
============
 
 
あらすじ
----------
 
キー値を生成する援助です。このモジュールは 2 つの種類のキーを持っています。彼らは dsa, rsa です。dsa キー ビット値は 1024年と rsa キーのビット値は 768 以上。その後だけそれは機能します。Ubuntu で、セント タスクに便利です OS。
 
ヘルプ コマンド
----------------
 
このヘルプ コマンドを特定のモジュールのインストール方法について説明します。Help コマンドは、エンドユーザーが動作するように簡単です。次のコマンドは、インストールに関するユーザー ガイド付き。
 
.. code-block:: bash
		
		ptconfigure Sshkeygen  help
 
コマンドを与えた後、コマンドはヘルプ オプションをリストアップします。次のスクリーン ショットは、このモジュールの使用のための視覚効果を与えます。
 

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeygen help
 ******************************


  This command allows you to install an SSH Key Pair.

  SshKeygen, ssh-keygen, sshkeygen

        - install
        Installs a new SSH Key
        example: ptconfigure ssh-keygen install
        example: ptconfigure ssh-keygen install --yes --bits=4096 --type=rsa --path="/home/dave/.ssh/id_rsa" --comment="Daves"

        - uninstall
        Removes an SSH Key
        example: ptconfigure ssh-keygen uninstall

 ------------------------------
 End Help
 ****************************** 
 
インストール
----------------
 
インストールは、モジュールをインストールするこの ptconfigure の下で、下記のコマンドを使用するだけで困難なプロセスではありません。
 
.. code-block:: bash

		ptconfigure sshkeygen install


Ssh の入力を入力した後キー gen を正常にインストールされます。次のスクリーン ショットは、このモジュールの使用のための視覚効果を与えます。
 
 

.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-keygen install
 Install SSH Key Generation? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         sshkeygen!        *
 *******************************
 Enter number of bits for SSH Key (multiple of 1024):
 1024
 Choose Key type (rsa/dsa)
 (0) rsa 
 (1) dsa 
 1
 Enter path to store private key (public key will be same with .pub):
 /root/SSH/abcd
 Plain text comment appended to public key. None is fine
 kevell
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 SshKeygen: Success
 ------------------------------
 Installer Finished
 ******************************

 



オプション
--------------
 
.. cssclass:: table-bordered

 +---------------------------+-------------------------+--------------+------------------------------------------------------------+
 | パラメーター              | ディレクトリ (既定値)   | オプション   | コメント                                                   |
 +===========================+=========================+==============+============================================================+
 |Install Key Generation     | Yes                     |              | それはptconfigure下に鍵生成をインストール                  |
 +---------------------------+-------------------------+--------------+------------------------------------------------------------+
 |Install Key Generation     | No                      |              | それは、処理を終了する。                                   |
 +---------------------------+-------------------------+--------------+------------------------------------------------------------+
 |Choose key type            | rsa                     | 0            | これは、選択したキータイプの下に鍵生成をインストール       |
 +---------------------------+-------------------------+--------------+------------------------------------------------------------+
 |Choose key type            | dsa                     | 1            | これは、選択したキータイプの下に鍵生成をインストール       |
 +---------------------------+-------------------------+--------------+------------------------------------------------------------+
 |path                       | /root/ssh/filename      | -            | これは、公開鍵と秘密鍵を使用してファイルを作成し|          |
 +---------------------------+-------------------------+--------------+------------------------------------------------------------+


 
 
利点
-----------
 
我々 は、リモートの場所から作業できます。ユーザーがパスのシステムを指示します。自動生成が可能です。我々 はあなたが必要なときにファイルを追加できます。我々 はパスワードなしキーを共有することができます。非大文字小文字を区別します。
 

