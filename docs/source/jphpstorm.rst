=================
PHPStorm
=================

あらすじ
----------------

PhpStorm は、PHP ＆ ptconfigure の最新の動向を保持、様々 な近代的なツールを統合し、主要な PHP フレームワークのサポートをさらに多くの機能拡張をもたらします。開発環境の自動構成 （コーディング標準、ファイルの関連付け、等）可能です。Ubuntu で、セント快適です OS。

ヘルプ コマンド
------------------------

このコマンドは目標と ptconfigure Php 嵐モジュールの下に利用可能なコマンドについて機能することができます。また、嵐の Php モジュールをインストールするコマンドについて説明します。インストールの前に、ユーザーはこのヘルプ コマンドは、その機能を説明を読むことができます。

.. code-block:: bash
   
	       ptconfigure PHPStorm help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、PHP の嵐の下で help コマンドについて視覚化します。


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPStorm help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  PHPStorm, phpstorm

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************

インストール
------------------

、下記のコマンドを使用できます、ユーザーが自分のマシンに git ツールをインストールする場合


.. code-block:: bash

	ptconfigure gittools install

上記のコマンドを入力した後、次の手順インストールの処理中に、表で説明されているよう


.. cssclass:: table-bordered


 +---------------------------+------------------------------------------------+------------+----------------------------------------------+
 | パラメーター              | 代替パラメーター                               | オプション | コメント                                     |
 +===========================+================================================+============+==============================================+
 |Install Git Tools? (Y/N)   | 代わりに使用したのPHPStorm我々は使用すること   | Y(Yes)     | ユーザーは、Yと入力することができ、          |
 |                           | ができますphpstorm                             |            | インストールプロセスを続行したい場合         |
 +---------------------------+------------------------------------------------+------------+----------------------------------------------+
 |Install Git Tools? (Y/N)   | 代わりに使用したのPHPStorm我々は使用すること   | N(No)      | ユーザーは、Yと入力することができ、          | 
 |                           | ができますphpstorm                             |            | インストールプロセスを続行したい場合|        |
 +---------------------------+------------------------------------------------+------------+----------------------------------------------+


次のスクリーン ショットは、絵インストール上記に説明したプロセスを示しています。



.. code-block:: bash

 
 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package gitk from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-cola from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************


利点
-------------------

* より多くの設定可能として、きちんとあなたのコードを維持するには
* 開発環境の自動構成と良いインターフェイスです。
* より良いコードのヒント & デバッグ
* 禅のコーディングは Devops で利用可能です。
* 複数のカーソルと簡単なキーボード ショート カットの作成、編集、および問題の間を移動します。
* より多くのカスタム属性、カスタマイズ可能なワークフローと強力なカスタマイズ。
* 開発者ツールの最新バージョンをインストールする使用されます。
 

