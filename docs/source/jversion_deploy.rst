=========
Version
=========

概要
----------------

このモジュールは ptdeploy の下で更新されたバージョンをインストールするために使用します。リビジョン コントロールがスタンドアロン アプリケーションとして最もよく実行バージョン管理も Ubuntu やセント OS などのオペレーティング システムのさまざまな種類に埋め込まれます。ほとんどのバージョンは、複数の開発者が同時に同じファイルを編集するを許可します。中央のリポジトリに変更をする「をチェック」最初の開発者常に成功します。システムは中央のリポジトリにさらに変更をマージする機能を提供して他の開発者は、チェックイン時に 1 人の開発者からの変更を保存する可能性があります。Ubuntu や CentOS をサポートしています。


Helpコマンド
-----------------------

Help コマンドは、ptdeploy のバージョンについてのユーザーをリードします。バージョンのモジュールに含まれるオプション。Help コマンドは、ptdeploy モジュールの下のバージョンの代替パラメーターを一覧表示されます。また、バージョンの構文について説明します。バージョンのヘルプ コマンドを以下に示します。


.. code-block:: bash

		ptdeploy  version help

次のスクリーン ショットは ptdeploy の完全な努力を示しています。

.. code-block:: bash


 kevell@corp:/# ptdeploy Version help
 ******************************


  This command is part of Default Modules and handles Application Versioning, allowing for rollbacks and the like.

  Version, version, vrs

          - specific
          Will change back the *current* symlink to whichever available version you pick
          example: ptdeploy version specific --limit=4 --container=/var/www/applications/the-app --version=2

          - latest
          Will change back the *current* symlink to the latest created version
          example: ptdeploy version latest
          example: ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

          - rollback
          Will change back the *current* symlink to the latest created version but one
          example: ptdeploy version rollback
          example: ptdeploy version rollback --limit=3 --container=/var/www/applications/the-app


      You can also apply a limit to the number of Versions to keep by using the --limit parameter
          example: ptdeploy version latest --limit=3

 ------------------------------
 End Help
 ******************************


代替パラメータ
--------------------------------

バージョンで利用可能な2つの選択肢があります。彼らです

Version, version, VERSION

インストール
----------------

インストールには、更新されたバージョンで、インストールを行うために必要なバージョンのインストールが含まれます。それは ptdeploy の下でのバージョンのモジュールをインストールするマニフェスト プロセスです。ちょうど、下記のコマンドを使用してバージョン


.. code-block:: bash

		ptdeploy version Install

コマンドを活性化した後、入力をcatechizeます。

ユーザーは自動的に yes と入力とシステムからのチェックイン バージョンがインストールされます。ない場合、インストールを終了します。次のスクリーン ショットは、バージョンとその機能を示しています。

オプション
------------

.. cssclass:: table-bordered

 +--------------------------+-----------------+---------------------------------------+----------------------------------------------+
 | パラメータ               | オプション      | 代替パラメータ                        | 注釈                                         |
 +==========================+=================+=======================================+==============================================+
 |Install version?(Y/N)	    | Yes	      | 代わりに使用できるユーザをバージ      | ptdeployモジュールの下で正常にインストール   |
 |			    |		      | ョンを使用しての Version, VERSION     |                                              |
 +--------------------------+-----------------+---------------------------------------+----------------------------------------------+
 |Install version?(Y/N)	    | No	      | 代わりに使用できるユーザをバージ      | 画面を終了                                   |
 |			    |		      |	ョンを使用しての Version, VERSION|    |	      				             |
 +--------------------------+-----------------+---------------------------------------+----------------------------------------------+


メリット
---------------

* 新しいバージョンを更新することができます。
* Ubuntu や CentOS を適しています。
* 非大文字小文字の区別 
* オートメーションが可能 
* コマンドを入力する簡単な



