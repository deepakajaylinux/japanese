========
Mkdir
========


あらすじ
------------

このモジュールはディレクトリの作成に役立ちます。ユーザーは、または実行時のディレクトリを作成するディレクトリの作成を宣言しながら、パスを指定できます。ことができますリモートまたはローカル マシンのいずれかを実行します。私たちを見てみましょうどのようにこのモジュール ディレクトリを作成するのに役立ちますについて。

ヘルプ コマンド
---------------------

ヘルプ コマンド同様目的に関してユーザーを導くように Mk ディレクトリに含まれているオプションについてヘルプ コマンドは MK ディレクトリの代替パラメーターが一覧表示されます。また、宣言時または実行時に 2 つの異なる方法でディレクトリを作成するための構文について説明します。.MK dir のヘルプ コマンドを以下に示します。

.. code-block:: bash

	ptconfigure mkdir help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットに MK ディレクトリ下の help コマンドについて視覚化します。


.. code-block:: bash

	kevell@corp:/# ptconfigure Mkdir help
	******************************


        This command handles file copying functions.

         Mkdir, mkdir

        - path
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure mkdir path
        example: ptconfigure mkdir path --yes --path="/path/to/new/directory"

	------------------------------
	End Help
	******************************
      
代替パラメーター
-------------------------

ヘルプ コマンドを使用して、ディレクトリの作成中 mkdir のではなく mkdir 関数も使用できます。

Mk Dir を作成します。
---------------------

Mk Dir を作成する 2 つの異なる方法で実行できます。

.. rubric:: Either at run-time

.. code-block:: bash

	Example: ptconfigure mkdir path

.. rubric:: Or, at the time of declaration

.. code-block:: bash

	Example: ptconfigure mkdir path --yes --path="/path/to/new/directory"

The following screen shot depicts the second way of creating a directory.

.. code-block:: bash

	kevell@corp:/# ptconfigure mkdir path --yes --path="/kevellsdoc"
	
	[Pharaoh Logging] [Mkdir] Executing mkdir /kevellsdoc
	******************************


	Mkdir Result: Success
	------------------------------
	Mkdir Finished
	******************************

利点
------------

* パラメーター ヘルプで使用されるディレクトリ操作の作成しない大文字と小文字は他と比較される間、加えられた利点であります。
  宣言時または実行時にディレクトリの作成 2 つの異なる方法で定義できます。
* ことができます両方のローカル コンピューターまたはリモート コンピューターで実行されます。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
 

