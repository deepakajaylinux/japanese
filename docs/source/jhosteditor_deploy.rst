======================
Host Editor
======================

概要
------------------

このモジュールは ptdeploy の下で Apache 仮想ホスト エディターを処理するためにサポートします。それは 2 つの方法で機能することができます。彼らは追加し、削除します。バーチャル ホストのエディターは、apache は非常に簡単に追加する仮想ホストをように書かれて PHP ツールです。バーチャル ホストのエディターは、ユーザーを追加、編集、またはユーザーの web サーバ上の仮想ホスト情報の削除を有効になります。Ubuntu とセントを使用すると便利です OS。Ptdeploy の下で、apache のバーチャル ホストのエディターがどのように機能することができますか見てみましょう。


Helpコマンド
-----------------------

このヘルプ コマンドは、hosteditor を作成するユーザーをガイドします。Hosteditor のヘルプ コマンドを以下に示します。

.. code-block:: bash

	ptdeploy Hosteditor help

開始後の入力上記のコマンドでは、仮想ホスト エディターを追加する機能します。それの教理のスクリーン ショットで機能します。

.. code-block:: bash

 kevell@corp:/# ptdeploy HostEditor help 

 ****************************** 

  This command is part of Default Modules and handles Host File Management Functions. 

  HostEditor, hosteditor, he, hostEditor 

          - add 
          add a Host File entry 
          example: ptdeploy hosteditor add 
          example: ptdeploy hosteditor add --yes 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1 
              --host-name=dave.com 

          - rm 
          remove a Host File entry 
          example: ptdeploy hosteditor rm 
          example: ptdeploy hosteditor rm --yes 
              --host-ip=127.0.0.1 # guess will ignore this, and remove any entry matching the host name 
              --host-name=dave.com 

 ------------------------------ 
 End Help 
 ****************************** 



代替パラメータ
-----------------------------------

宣言で定義することができます、代替パラメーターを次に示します。

HostEditor, hosteditor, he, hostEditor 


Add
-------

これは、エディターのホストを作成するユーザーを容易にします。よると、ユーザーが入力できる彼らの願いを。

.. code-block:: bash

		sudo ptdeploy hosteditor add

として、上記のコマンドの入力後、ユーザーは、次のプロセスを埋めることができます。

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor add 

 Do you want to add a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 
 
 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          karuna 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block::  bash

 kevell@corp:/# ptdeploy hosteditor add --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 kumar 
 ****************************** 

 1Host Editor Finished 
 ****************************** 




削除する
--------------

Hosteditor を削除するためのターミナル コマンドは rm です。このコマンドの一般的な形式は、rm です。rm とあなたはいけないかどうか、それはエラー メッセージが表示されます、次のホストに移動し、正しいパスを指定した場合、ホストを削除します。

次のコマンドは、仮想ホストを削除するために使用。

.. code-block:: bash
   
		sudo ptdeploy hosteditor rm

以下のスクリーンショットは、その機能を説明することができます。

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor rm 

 Do you want to remove a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 

 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          nithin 
 127.0.0.1          kumar 
 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy hosteditor rm --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 nithin 
 ****************************** 
 
 1Host Editor Finished 
 ****************************** 


メリット
---------------

* マルチ ユーザーに一度にアクセスできます。
* ユーザーは、追加またはホストを削除できます。
* 非大文字小文字を区別します。

