=======
Chown
=======

あらすじ
----------

このモジュールは、所有者のパーミッションを変更する使用できます。個々 のファイルに対するアクセス許可を変更することができますまたはディレクトリ。その前にファイルおよびディレクトリを作成する時に割り当てられる既定のアクセス許可の対応をする必要があります。

ヘルプ コマンド
-----------------

このヘルプ コマンドを特定のモジュールのインストール方法について説明します。Help コマンドは、エンドユーザーが動作するように簡単です。また、宣言に使用される代替パラメーターを一覧表示されます。次のコマンドの取り扱いについてユーザー ガイドこのモジュール。

.. code-block:: bash
	
	ptconfigure chown help

コマンドを与えた後、コマンドはヘルプ オプションをリストアップします。次のスクリーン ショットは、このモジュールの使用のための視覚効果を与えます。


.. code-block:: bash

	Kevell@corp:/# ptconfigure chown help
	******************************

	 This command handles file user ownership changing functions.

	  Chown, chown

        - path
        Will change the user ownership of a path
        example: ptconfigure chown path --yes --guess --recursive --path=/a/file/path --owner=golden

	------------------------------
	End Help
	******************************

パス
-------

それは少し以下のコマンドを使用してptconfigureの下で、このモジュールのための優れたプロセスであり、


.. code-block:: bash

	ptconfigure chown path –yes—guess—recursive—path=/ptconfigure—owner=Kevells

その後、入力を入力します。
所有権のユーザーを入力します。
所有者名を入力した後
Chown 結果成功が表示されます。


これは次のスクリーン ショットで視覚的に表示されます。

.. code-block:: bash

	kevell@corp:/# ptconfigure chown path --yes --guess --recursive --path=/phj.php --owner=deepak

	Enter ownership user:
	deepak
	[Pharaoh Logging] [Chown] Executing chown -R deepak /phj.php
	******************************


	Chown Result: Success
	------------------------------
	Chown Finished
	******************************

代替パラメータ
----------------------------

利用可能な2つの代替パラメータがあります。

Chown, chown


利点
--------

* モジュールはptconfigureでいつでも所有者を変更することができます。
* 1 つのファイルを変更した場合に再帰処理をしている間、全体のフォルダーが変更もできます。
* 我々 は、所有者の現在の状態を確認できます。

