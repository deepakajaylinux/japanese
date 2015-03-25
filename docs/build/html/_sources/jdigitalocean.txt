================
DigitalOcean
================


概要
------------

このモジュールはデジタル海洋上のサーバーの処理で、ユーザーを支援します。それはデジタルの海に箱の処理でユーザーのすべての基本的なニーズを包みます。今後のトピックでは、このモジュールでは、このモジュールの下にデジタル海のさまざまな機能を使用する方法について説明します。


Helpコマンド
-------------------

Help コマンドは、簡単なユーザー マニュアルとして機能します。このモジュールの主な目的について説明します。アウトの宣言で使用することができます、代替パラメーターが表示されます。また、それもハイライト構文と共にこのモジュールの下にデジタルの海を使用してそれらを使用するためのさまざまな機能です。ヘルプ オプションを宣言するために使用されるコマンドは、次に示す


.. code-block:: bash

		ptconfigure DigitalOcean help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、デジタルの海の下で help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure DigitalOcean help
 ******************************


    This is an extension provided for Handling Servers on Digital Ocean.

    DigitalOcean, digitaloceanv1, digital-ocean-v1

        - box-add
        Lets you add boxes to Digital Ocean, and adds them to your papyrusfile
        example: ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" --digital-ocean-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your digital ocean account - Careful - its irreversible
        example: ptconfigure digital-ocean box-destroy-all --yes --guess

        - save-ssh-key
        Will let you save a local ssh key to your Digital Ocean account, so you can ssh in to your nodes
        securely and without a password
        example: ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - list
        Will display data about your digital ocean account
        example: ptconfigure digital-ocean list
        example: ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys

 ------------------------------
 End Help
 ******************************

デジタルオーシャンの特長
--------------------------------

このモジュールは下記のようにデジタルの海を使用してさまざまな機能上の help コマンドで示されています。


* Box_Add
* Box_Destroy
* Box_Destroy_All
* Save_ssh_Key
* List


Box_Add
------------

この機能、デジタルの海にボックスを追加することを目的とし、手にパピルス ファイルにそれらを追加します。これは単に、下記の構文を使用してによって実装することができます。


.. code-block:: bash

	ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"


上記のコマンドを実装するには、ユーザー上記の述べられた構文の形式で、次のフィールドを指定しなければなりません。


* Digital ocean Ssh-key path
* Digital ocean Ssh_key name



Box_Destroy
----------------

この機能ボックスを指定された環境と手を破壊することを目指してパピルス ファイルからそれらを削除します。これは単に、下記の構文を使用してによって実装することができます。


.. code-block:: bash

	ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" 
        --digital-ocean-ssh-key-name="bastion"

上記のコマンドを実装するには、ユーザー上記の述べられた構文の形式で、次のフィールドを指定しなければなりません。


* Digital ocean Ssh-key path
* Digital ocean Ssh_key name

Box_Destroy_All
----------------------

この機能デジタル海アカウントですべてのボックスを破壊することを目指します。ユーザーはそれは不可逆的なプロセスですので、この機能を実装するときに注意しなければなりません。この関数を実装するには、ユーザーは、以下に示すようにコマンドを適用する必要があります。


.. code-block:: bash
   
	ptconfigure digital-ocean box-destroy-all --yes --guess


Save_Ssh_key
-------------------

この機能を保存するローカル ssh に、デジタルの海に、ユーザーができるように ssh 安全にパスワードなしのそれぞれのノードにユーザーことができます。これは、以下のコマンドを使用して達成することができます。


.. code-block:: bash

	ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

上記のコマンドを実装するには、ユーザー上記の述べられた構文の形式で、次のフィールドを指定しなければなりません。


* Digital ocean Ssh-key path
* Digital ocean Ssh_key name

List
-------

この機能を使用するとのデジタル海アカウントに関するすべてのデータを一覧表示することができます。これは単に、以下のコマンドを使用して実装することができます。       

.. code-block:: bash

	ptconfigure digital-ocean list

Or

.. code-block:: bash

        ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys


代替パラメータ
----------------------------

これのいずれかの宣言で使用することができますこのモジュールの代替のパラメーターは、

 DigitalOcean,   digitaloceanv1,   digital-ocean-v1


メリット
-----------

* パラメーター宣言するヘルプを使用して apt の他のさまざまな機能は区別されません。
* それは裕福な両方セント os とも Ubuntu のように。
* このモジュール デジタル海の処理でユーザーのニーズをすべてを包み込みます。



