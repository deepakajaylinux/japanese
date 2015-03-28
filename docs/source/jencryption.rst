============
Encryption
============

概要
------------

このモジュールは、ユーザーがファイルの暗号化または復号化することができます。

暗号化は、唯一認可された当事者がそれを読むことができるような方法でメッセージや情報を符号化するプロセスです。暗号化は、盗聴を防ぐことはできませ自体の行いますが、インターセプタにメッセージの内容を拒否します。暗号化方式では、平文と呼ばれるメッセージ又は情報は、復号化された場合にのみ読み取ることができる暗号文を生成し、暗号化アルゴリズムを使用して暗号化される。技術的な理由から、暗号化方式は、通常はアルゴリズムによって生成された擬似ランダムキーを使用しています。これは、適切に設計された暗号化方式のため、大規模な計算資源と熟練が必要とされる、鍵を所有することなく、メッセージを解読するために、原理的には可能であるが、。許可された受信者は、簡単に受信者にではなく、権限のないインタセプタに創始者によって提供されたキーでメッセージを解読することができます。

私たちは、ファイルや文字列の暗号化と復号化にこのモジュールを使用する方法を見てみましょう。

helpコマンド
-------------------

helpコマンドは、このモジュールを取り扱うでユーザーを支援する簡単なユーザマニュアルです。これは、宣言で使用することができる別のパラメータを指定する。また、それらを使用するための構文と一緒に、この暗号化モジュールの下で可能な機能を指定します。ヘルプオプションの宣言に使用されるコマンドは、以下の通りです

.. code-block:: bash

	ptconfigure encryption help

helpコマンドを宣言するための構文は、追加的な利点である大文字と小文字を区別しませんです。次のスクリーンショットは、暗号化の下で、helpコマンドについてあなたを視覚化。

.. code-block:: bash



 kevell@corp:/# ptconfigure encryption help

 ******************************


 This command allows you to encrypt or decrypt a file.  

 Encryption, encrypt  

 - install        
	Encrypts a file or string        
 	example: sudo ptconfigure encryption install --yes --unencrypted-data=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion        
	 --encryption-target-file=/tmp/encrypted --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions=""                
	 --encryption-file-owner="" --encryption-file-group=""                

 - uninstall        
	Decrypts an encrypted file or string        
	example: sudo ptconfigure encryption uninstall --yes --encrypted-data=/tmp/encrypted        
	 --encryption-target-file=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion --encryption-key=/root/.ptconfigure/SSH/key                	 --encryption-file-permissions="" --encryption-file-owner="" --encryption-file-group=""                

 ------------------------------
 End Help
 ******************************

インストール
---------------------

この機能は、ユーザーが以下のように単純にコマンドを使用して、ファイルまたは文字列を暗号化することができ、

.. code-block:: bash
	
	 sudo ptconfigure encryption install --yes --unencrypted-data=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion
 	--encryption-target-file=/tmp/encrypted --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions=""                
	 --encryption-file-owner="" --encryption-file-group=""                

この機能を実装するには、ユーザーは、上記の構文の形式で次のフィールドを指定する必要が、

* encryption target file
* encryption key
* SSH key
* encryption file permission
* encryption file owner
* encryption file group


.. code-block:: bash

 kevell@corp:/# sudo ptconfigure encryption install --yes --unencrypted-data="/home/kevells/Desktop/graphs" --encryption-target-file="/home/kevells/Desktop/graphs" --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions="755" --encryption-file-owner="kevells" --encryption-file-group="kevells"

 *******************************
 *        Pharaoh Tools        *
 *         Encryption !        *
 *******************************
 [Pharaoh Logging] Package php5-mcrypt from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Encryption: Success
 ------------------------------
 Installer Finished
 ******************************



アンインストール
---------------------------

この機能は、ユーザーが暗号化されたファイルまたは文字列を復号化することができる。これは、以下のコマンドを使用して達成することができる

.. code-block:: bash

	sudo ptconfigure encryption uninstall --yes --encrypted-data=/tmp/encrypted
	 --encryption-target-file=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion --encryption-key=/root/.ptconfigure/SSH/key                	 --encryption-file-permissions="" --encryption-file-owner="" --encryption-file-group=""                

この機能を実装するには、ユーザーは、上記の構文の形式で次のフィールドを指定する必要が、

* encryption target file
* encryption key
* SSH key
* encryption file permission
* encryption file owner
* encryption file group

別のパラメータ
------------------------------

宣言で使用することができるいずれかがこのモジュールの別のパラメータであり、

* Encryption
* encrypt

メリット
-------------

* 追加された利点である大文字と小文字を区別しませんヘルプと暗号化と復号化の国連の操作で使用されるパラメータを比較しながら、
  他の人に。
* これは、Ubuntuと同様にセントOSの両方に裕福なです。
* 唯一許可された人はそれらを使用することができますので、*これは、セキュリティで保護されたモードです。
