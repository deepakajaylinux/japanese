PTVirtualize
=============

概要
---------------



ptconfigureと比較しながら、 ptvirtualizeは、仮想マシンと開発環境管理のための機能を提供し、仮想マシンの管理ツールです。

Devopsを使用することにより、仮想マシンの構成を管理しても、非常に複雑な開発環境に貢献異なるタイプのを容易にする。

これは、標準化と仮想化環境へのセットアップを管理、自動化を容易にします。その機能は、構成管理、テストの自動管理、自動展開、ビルドとリリース管理、開発環境の管理が含まれており、それらの機能が実行されます。

ptvirtualizeでは構成管理、システム自動化とインフラストラクチャは、PHPで囲まれている。実行するには、コンパイル·ステップが存在しないようにPHPスクリプトを編集すると、本当に簡単です。


ptvirtualizeは、オブジェクト指向のデータ型だけでなく、データに適用することができる操作の種類だけでなく、豊かであること。したがって、手続き型プログラミング技術よりオブジェクト指向プログラミング技術を比較しながら、オブジェクト指向プログラミングは、新しいタイプのオブジェクトが追加されたときに変更する必要のないモジュールを作成するために、エンドユーザーを可能にする。

余分なモジュールが必要な場合、ユーザは、フレームとそれらの要件に応じてモジュールを設計し、彼らは含めることができようにptvirtualizeは、拡張可能です。

必要に応じて、テンプレートオプション外テンプレートの機能を使用して、追加することができる。 SSHオプションでは、SSHキーの値を設定できます。 SFTPは読みやすさを促進し、仮想ボックスを使用して、2つの異なるOS間での能力を記述します。

必要条件
-----------------

あなたがptvirtualizeを使用したい場合は、 Virualボックスは仮想ボックスゲストの追加機能と一緒に、あなたのマシンにインストールされているかどうか確認してください

バーチャルボックスをインストールするためのコード
----------------------------------------------------

.. code-block:: bash

        sudo ptconfigure virtualbox install --yes --guess --with-guest-additions

インストール
---------------

お使いのマシンにptvirtualizeツールをインストールするには、次の2つの方法があります：

1)Installation via ptconfigure

2)Installing ptvirtualize alone

ptconfigure経由のインストール
----------------------------------

あなたがあなたのマシンにptconfigureツールを持っている場合、それは以下のようなコードを使用してptvirtualizeをインストールするには簡単です、


.. code-block:: bash


        sudo ptconfigure ptvirtualize install --yes --guess

インストール時に独自のディレクトリを選択しながら、ここでの単語の推測は無視することができます。

一人でptvirtualizeのインストール
-----------------------------------

あなたがptconfigureツールに依存することなく、あなたのマシンにptvirtualizeツールをインストールしたい場合は、コマンドを使用して簡単です、

.. code-block:: bash

        sudo apt-get install php5 git
        
このコマンドは、ご使用のマシンにPHP5とのgitをインストールします。それは、次のコマンドを使用した後、 ::

        git clone http://github.com/PharaohTools/ptvirtualize && sudo php ptvirtualize/install-silent

インストール時に場所を選択したくない場合は、上記のようにコマンドを使用することができる。あなたがそうしたい場合は、次のコマンドを使用します::

        git clone http://github.com/PharaohTools/ptvirtualize && sudo php ptvirtualize/install

使用量の方法論
-----------------------

ここでは、私たちはツールとその使用法の下でコマンドを使用する方法を見てみましょう。

あなたは、単に次のコマンドを入力した場合、 ::

    ptvirtualize

下のスクリーンショットに示すように、あなたは、このツールの下で利用可能なすべてのモジュールの表示を取得します。 ::

 kevell@Corp:/# ptvirtualize
 ******************************
 Pharaoh Tools - Virtualize
 ******************************


 Virtualize by Golden Contact Computing
 -------------------

 About:
 -----------------
 Virtualize is for controlling Virtual Machines in Development Environments.

 -------------------------------------------------------------

 Available Commands:
 ---------------------------------------

 AutoSSH - AutoSSH - Use your Papyrus details to automatically SSH or SFTP into your Virtualize box
 Box - Box - Manage Base Boxes for Virtualize
 Destroy - Destroy - Stop a Virtualize Box
 Flirtify - Virtualize Flirtify - Generate a Phalgrantfile
 Halt - Halt - Stop a Virtualize Box
 Invoke - SSH Invocation Functions
 PharaohTools - Pharaoh Tools Provisioner Integration
 Provision - Provision - Stop a Virtualize Box
 Resume - Resume - Stop a Virtualize Box
 SFTP - SFTP Functionality
 Shell - Shell Provisioner Integration
 Status - Status - Stop a Virtualize Box
 SystemDetection - System Detection - Detect the Running Operating System
 Up - Up - Create and Start a Virtualize Box
 Virtualbox - Virtualbox Provider Integration 

 ******************************


Helpコマンド
---------------

これは、 helpコマンドを使用するように簡単です、

  ptvirtualize ModuleName help

このコマンドは、特定のモジュールがどのように動作するのに役立ちますし、また、それが実行できるアクションが何であるかについて。
下のスクリーンショットは、 helpコマンドは、モジュールAutoSSHを説明するために使用され、どのように説明しています。 ::

    kevell@Corp:/#ptvirtualize AutoSSH help

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

簡単な例
---------------

それではここでptvirtualizeに関する短い例について見てみましょう。

ディレクトリを作成する、または単にあなたの新しいファラオプロジェクトます。mkdir / VAR / WWW /私のテストプロジェクト&& CDの/ var / www /の私のテスト·プロジェクトとして、現在のWebプロジェクトを使用

あなたはそれがすでに、それは次のようにコマンドを使用して簡単ですがない場合は、あなたのマシンにVirtualBoxをインストールし、 ::

    sudo ptconfigure virtualbox install --yes --guess --with-guest-additions

次のコマンドを使用してデフォルトptconfigure構成管理オートパイロットファイルを追加::

    sudo ptconfigure cleofy install-generic-autopilots --yes --guess --template-group=ptvirtualize

flirtify ptvirtualize flirt now --template-group=default-php

インストール、設定、現在は、仮想マシンのptvirtualizeを起動




ptvirtualizeモジュールと遊ぶ
------------------------------------

.. toctree::
   :maxdepth: 3



 jautossh_virtualize
 jbox_virtualize
 jdestroy_virtualize
 jflirtify_virtualize
 jhalt_virtualize
 jinvoke_virtualize
 jpharaohtools_virtualize
 jresume_virtualize
 jsftp_virtualize
 jshell_virtualize
 jstatus_virtualize
 jsystemdetection_virtualize
 jup_virtualize
 jvirtualbox_virtualize

