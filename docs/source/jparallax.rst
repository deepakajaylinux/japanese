============
Parallax
============

あらすじ
----------

視差はユーザーのマシンでマルチタスク機能を促進します。他の人に比べてしないインストールとヘルプを定義するパラメーターが大文字と小文字を区別します。インストール時またはインストール プロセスの実行時に、マルチタスク機能を定義する方が簡単です。

ヘルプ コマンド
-----------------

ヘルプ コマンドこの視差での作業にユーザーをリードします。また、視差と 2 つのタイプのインストールを宣言する構文をインストールするために使用されるコマンドを指定します。ヘルプ コマンドも使用することができますの代替パラメーターを一覧表示します。視差の下のヘルプ オプションを使用するコマンドは以下の通りです。

.. code-block:: bash

	ptconfigure parallax help

Help コマンドの入力後の結果の表示は、以下のスクリーン ショットで表されます。


.. code-block:: bash


	kevell@corp:/# ptconfigure Parallax help
	******************************



	This Module lets you execute commands in parallel

        Parallax, parallax

        - cli
        Go through all questions to execute parallel programs
        example: ptconfigure parallax cli
        example: ptconfigure parallax cli --yes --command-1="pwd" --command-2="ls"

        - child
        Unlikely you'll use this, its used by cli to spawn child processes
        example: parallax cli child

	------------------------------
	End Help
	******************************

インストール
--------------

ユーザー要件に従って 2 つの異なる方法でインストールを定義することができますとしてインストールするための視差と行く簡単です。これら 2 つの方法は以下のように定義されます。

* でインストール コマンドを定義する際に必要なマルチタスクの種類を言及します。
* または、running(Run-time) のインストール中にタスクの種類を言及します。

インストール コマンドを宣言する時に複数のタスクを指定するために使用するコマンドを次に示します。


.. code-block:: bash

	ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"

このコマンドを言及した後、視差はコマンド 1 で上で指定したコマンド 2 としてタスクの両方を実行します。2 つのタスクを並列実行し、結果が表示されます。スクリーン ショット以下添付型の宣言の上で定義した非常に良い例です。


.. code-block:: bash

	kevell@corp:/# ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"
	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------

	In Cli


	******************************



実行時にマルチ タスクを宣言するために使用するコマンドを次に示します。

.. code-block:: bash

	ptconfigure parallax cli child

上記のコマンドを入力した後、次のプロセスが発生します。

.. cssclass:: table-bordered

 +-----------------------+---------------------------------------------+--------------+--------------------------------------------------+
 | パラメータ            | 代替パラメータ                              | オプション   | 注釈                                             |
 +=======================+=============================================+==============+==================================================+
 |Run Commands in        | の代わりに parallax, 以下の選択肢を使       | Y(Yes)       | ユーザーは、Yと入力することができ、              |
 |Parallel? (Y/N)        | 用することもできる Parallax                 |              | インストールプロセスを続行したい場合             |
 +-----------------------+---------------------------------------------+--------------+--------------------------------------------------+
 |Run Commands in        | の代わりに parallax, 以下の選択肢を使       | N(No)        | ユーザーは、Nと入力することができ、              |
 |Parallel? (Y/N)        | 用することもできる Parallax                 |              | インストールプロセスを終了したい場合は|          |
 +-----------------------+---------------------------------------------+--------------+--------------------------------------------------+


ユーザーがインストールを続行する場合、ユーザーの要件に従って複数のタスクを指定できます。完了後、複数のタスクを指定する場合に、ユーザーを停止する彼らを停止できます none を入力するだけ。

最後に、その状態と完了したタスクの結果は最後に定義されます。次のスクリーン ショットについて上記のプロセスをグラフィカルに表示することができます。

.. code-block:: bash

   
	kevell@corp:/# ptconfigure parallax cli child
	
	Run Commands in Parallel? (Y/N) 
	y
	Enter Command to include next. Enter none to end.
	pwd
	Enter Command to include next. Enter none to end.
	who
	Enter Command to include next. Enter none to end.

	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------

	In Cli


	******************************



利点
----------

* ユーザーは、実行時に、またはその要件に従って事前に定義された方法で並列タスクを定義できます。
* 最後の結果と完了したタスクの進捗状況は明らかに複数のタスクの完了後に報告されます。
* を宣言するために使用する構文は追加の利点がある他の人に比較しながら大文字小文字を区別しません。
* 両方セント Os で裕福なと同様に大文字小文字を区別は。
 

