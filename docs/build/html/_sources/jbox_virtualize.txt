=======
Box
=======

概要
------------

このモジュールで処理し、ptvirtualize で利用可能なボックスを管理するユーザーを支援します。ボックスの関数の処理でこのモジュールのしくみを見てみましょう。


Helpコマンド
---------------------

Help コマンドと同様、目的に関するユーザー ガイドとしてボックス モジュールに含まれているオプションについて。アウト ボックスのモジュールの代替パラメーターが表示されます。また、追加、削除、パッケージ リストのコマンドを使用する構文について説明します。ボックスのモジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash
		
		ptvirtualize Box help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、ボックスの下には、help コマンドについて視覚化します。

.. code-block:: bash

 kevell@corp:/# ptvirtualize Box help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to manage the Base boxes available to you in ptvirtualize

  Box, box

        - add
        Initialises the Box as usable by ptvirtualize
        example: ptvirtualize box add
        example: ptvirtualize box add --yes --guess
            --source="/home/dave/file.box" # where the box file is
            --target="opt/ptvirtualize/boxes" # will guess the dir next to ptvirtualize install dir
            --name="vanillaubuntu"

        - remove
        Removes the box as usable by ptvirtualize
        example: ptvirtualize box remove

        - package
        Packages a box as usable by ptvirtualize
        example: ptvirtualize box package
        example ptvirtualize box package --yes --guess
            --name="Vanilla Ubuntu 12.04 amd 64"
            --vmname="a4dc638f-2721-40c4-a943-2f2565c83fee" # use name or id of virtual machine
            --provider="virtualbox" # guess will use virtualbox
            --group="ptvirtualize"
            --slug="" # guess can generate this based on name field
            --description="A Vanilla install of Ubuntu..."
            --home_location="http://www.someplace.net/" # guess will set this to http://www.ptvirtualizeboxes.co.uk/
            --target="/opt/ptvirtualize/boxes" # save location, will guess /opt/ptvirtualize/boxes

        - list
        List boxes installed in ptvirtualize
        example: ptvirtualize box list

 ------------------------------
 End Help
 ******************************

ptvirtualizeボックスの機能
----------------------------------

示されている上記のヘルプ コマンドの ptvirtualize ボックスの機能は次のとおり：


* Add
* Remove
* Package
* List

Add
-----

Ptvirtualize の追加は可能なものとしてボックスを初期化するため使用されます。Ptvirtualize ボックスを追加するため、次の構文を使用できます。


.. code-block:: bash

		ptvirtualize box add

or

.. code-block:: bash

	ptvirtualize box add --yes --guess
	--source="/home/dave/file.box	(This line describes where the box is)
	--target="opt/ptvirtualize/boxes"	(This line guess the dir next to ptvirtualize install dir)
	--name="vanillaubuntu"

In the above mentioned ways the box can be added to a ptvirtualize.

Remove
-----------

この関数は ptvirtualize で使用可能なボックスを削除するため使用されます。これを行うことができます以下のコマンドを使用して。


.. code-block:: bash

		ptvirtualize box remove

上記の方法では、ptvirtualize から、ボックスを削除できます。


Package
-----------

この関数は ptvirtualize パッケージとして使用可能なボックスを使用します。これは、次のコマンドを使用して実装することができます。


.. code-block:: bash

		ptvirtualize box package

or

.. code-block:: bash

	ptvirtualize box package --yes --guess
	name="Vanilla Ubuntu 12.04 amd 64"
	vmname="a4.............." (This two lines represents the name and id of virtual machine)
	--provider="virtualbox" (guess will use virtual box)
	--group="ptvirtualize"
	--slug="" (The guess can generate this based on the name field)
	--description="A vanilla install of Ubuntu..."
	--home_location="http://www.someplace.net/" (guess will set this to http://www.ptvirtualizeboxes.co.uk/
	--target="/opt/ptvirtualize/boxes" (The location for saving)



最後に、ボックスは、ptvirtualize によって使用できるようにパッケージします。


List
-----

この関数は ptvirtualize にインストールされているボックスをリストするために使用されます。これは、次のコマンドを使用して行うことができます。


.. code-block:: bash

		ptvirtualize box list

上記のコマンドを使用して、新しくインストールされる ptvirtualize のボックスの一覧が表示されます。

代替パラメータ
-------------------------------

* Box
* box


上記のリストでは、代替のパラメーターのいずれかの宣言で使用できます。

メリット
-----------

* ヘルプで使用するパラメーターは大文字小文字を区別しながら他の人に比べて、追加の利点は。
* 両方の Ubuntu と同様、それは裕福なセントの OS として。
* 構文を使用して追加の削除、パッケージ化、リスト大文字と小文字が区別されません。


