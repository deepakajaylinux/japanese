==========
File
==========

あらすじ
-------------

ファイルはコンピューターのファイルに含まれるデータの種類を認識するための標準的なプログラムです。ファイル コマンドは引数として用意されていると各ファイル システム オブジェクト (ファイル、ディレクトリまたはリンクなど) を分類しようとすると (すなわち、入力)。ファイルは、それを分類する試みで各引数をテストします。この順序で実行されるテストの 3 つのセットがあります: ファイル システム テスト、マジック ナンバー テスト、および言語テスト。

最初のオブジェクトの i ノード (ファイルに関する情報が含まれています) から情報を取得する stat システム コールを使用して、ファイル システム テストです。

多数のであるマジック ナンバーが 2 番目のテスト チェックで埋め込まれたまたは (すなわち、ファイルの種類) のファイル形式を示す多くの種類のファイルの先頭付近に。


プレーン テキストであるかどうかを判断する言語テストが採用するファイルの種類を決定する、最初の 2 つのテストに失敗すること (すなわち、人間が判読できる文字の完全で構成) と、どのような HTML (ハイパー テキスト マークアップ言語) やソース コードなどのプレーン テキストの場合

ヘルプ コマンド
-----------------

このコマンドは、モジュール ファイルの使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash
        
	        ptconfigure file help

.. code-block:: bash

 kevell@corp:/# ptconfigure File help
 ******************************


  This command allows you to modify files or check their existence

  File, file

        - create
        Create a new system file
        example: ptconfigure file create --file="somename"

        - delete
        Delete a system file
        example: ptconfigure file delete --file="somename"

        - exists
        Check the existence of a file
        example: ptconfigure file exists --filename="somename"

        - append
        Append a line to a file
        example: ptconfigure file append --filename="somename" --line="a line"

        - should-have-line
        Ensure that a file contains a particular line
        example: ptconfigure file should-have-line --filename="somename" --line="a line"

 ------------------------------
 End Help
 ******************************




作成します。
------------

ユーザーは新しいシステム ファイルを作成する必要がある場合、特定のコマンドの下、プロセスが実行されます。
 

.. code-block:: bash

                ptconfigure file create --file="somename"


下記のコマンドに存在するファイルを上書きします。


.. code-block:: bash
         
	       ptconfigure file create --file="somename” --overwrite-existing

下記コマンドを書き込み用ファイル内のデータ

.. code-block:: bash
           
		ptconfigure file create –file="somename” --data="things to put in the file" 


.. code-block:: bash

 kevell@corp:/# ptconfigure file create --file="somename"

 [Pharaoh Logging] [File] Creating File somename
 File somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************



削除
----------

ユーザーはシステム ファイルを削除する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
		ptconfigure file delete --file="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure file delete --file="somename"

 [Pharaoh Logging] [File] Deleting File somename
 somename Deleted
 File somename not exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************




存在します。
-------------

ユーザーは、ファイルの存在を確認する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash

		ptconfigure file exists --filename="somename"


.. code-block:: bash

 kevell@corp:/# ptconfigure file exists --filename="somename"

 Enter File Path:
 /home/kevells/Desktop/somename
 File /home/kevells/Desktop/somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************



追加
------------

ユーザーをファイルに行を追加する必要がある場合、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
		ptconfigure file append --filename="somename" --line="a line"


オプション-の行を追加する行を挿入します。

.. code-block:: bash

 kevell@corp:/# ptconfigure file append --filename="somename" --line="a line"

 Enter File Path:
 /home/kevells/Desktop/somename                             
 Enter the input for append:
 this is for test
 [Pharaoh Logging] [File] Reading File /home/kevells/Desktop/somename
 [Pharaoh Logging] [File] Writing File /home/kevells/Desktop/somename
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************






べきである持っているライン
-----------------------------

ユーザーが特定の行がファイルに含まれていることを確保するために、特定のコマンドの下、プロセスが実行されます。


.. code-block:: bash
	
		ptconfigure file should-have-line --filename="somename" --line="a line"


オプション-ニーズをチェックするステートメントの行します。


オプション
---------------
                              

.. cssclass:: table-bordered


 +------------------------+------------------------------------------------------------------------+
 | Parameters             | Alternative Parameter                                                  |
 +========================+========================================================================+
 |ptconfigure file help   | 2代替パラメータのいずれかがコマンド - で使用することができます File,   |
 |                        | file eg: ptconfigure File Install/ ptconfigure file Install|           |
 +------------------------+------------------------------------------------------------------------+




利点
-----------

* を指定する特殊な形式のファイルを含む位置敏感なテスト;デフォルト位置敏感なテストと状況依存のテストは実行されません。
 
