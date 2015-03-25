==========
AutoSSH
==========


概要
-----------

このモジュールは autoSSH ptvirtualize ボックスにユーザーを容易にします。Autossh は、小さな、接続を監視することができる場合はそれが低下またはが応答を停止、トンネルを再起動 SSH のフロント エンド。


autossh を使用して ssh を ssh 促進 (からローカルからリモート、リモートからローカル 1 つ) のループを作成し、送信テストを取り戻すと予測されるデータ。


私たちを見てみましょう自動機能 ssh の今後のトピック。

Helpコマンド
-------------------

Help コマンドと同様、目的に関するユーザー ガイドとして自動 SSH モジュールに含まれているオプションについて。それは自動 SSH モジュールの代替パラメーターが一覧表示されます。また、cli、sftp_put、sftp_get コマンドを使用する構文について説明します。自動 SSH モジュールのヘルプ コマンドが表示されます以下の通りです。


.. code-block:: bash

		ptvirtualize AutoSSH help


ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、help コマンドの下で自動 SSH について視覚化します。

.. code-block:: bash


 kevell@corp:/# ptvirtualize AutoSSH help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to autoSSH a ptvirtualize box

  AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your ptvirtualize Box
        example: ptvirtualize auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

 ------------------------------
 End Help
 ******************************


AutoSSHの機能
----------------------

上記のヘルプ コマンドで示されているこの自動車の主要な機能には ssh モジュールが含まれています


* cli
* sftp_put
* sftp_get


Cli
------

アクティブ化したり、自動 ssh ユーザー環境でビルド後、次のコマンドを使用して、SSH Cli ユーザー ptvirtualize ボックスを開くに使用される cli を作成できます。


.. code-block:: bash

		ptvirtualize auto-ssh cli --yes --guess


Cli は自動 ssh が生成される場所特定の環境で利用可能なクライアントをリストするために使用されます。

Sftp_put
-----------

この関数は、配置または必要なファイルやデータ ソースから移動する先の特定の環境の自動 ssh が生成される場所に使用されます。これは下記のコマンドを使用して行うことができます。


.. code-block:: bash

		ptvirtualize auto-ssh sftp-put --yes --guess --source="path/to/source --target=/path/to/target

上記のコマンドは、ユーザー ptvirtualize ボックスに、ファイルを配置します。次のスクリーン ショットは、プロセスを視覚的に表現します。

Sftp_get
-----------

この関数は、取得または先の特定の環境の自動 ssh が生成される場所のソースから必要なファイルやデータをフェッチするために使用されます。これは下記のコマンドを使用して行うことができます。

.. code-block:: bash

		ptvirtualize auto-ssh sftp-get --yes --guess --source="path/to/source --target=/path/to/target

上記のコマンドを取得またはユーザー ptvirtualize ボックスからファイルを受信します。次のスクリーン ショットは、プロセスを視覚的に表現します。

代替パラメータ
-----------------------------

* AutoSSH
* auto-ssh
* autossh
* ssh
* SSH

上記のリスト内の代替パラメーターは宣言で使用できます。

メリット
-----------

* パラメーター ヘルプで使用されるインストールと国連のインストール操作しない大文字と小文字は他と比較される間、加えられた利点であります。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* Cli 機能リスト アウト自動 SSH による特定の環境で利用可能なクライアントです。
* Sftp_put、Sftp_get を配置し、自動 SSH を使用して、特定の環境のソースと宛先の間それぞれのファイルをフェッチできます。Cli では、
  宣言するための構文、取得は明確に描かれている help コマンドで。


