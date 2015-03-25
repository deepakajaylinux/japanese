==========
JFeature
==========

概要
---------------

JFeatures は、世界で最も人気のあるソフトウェア パッケージを作成、整理、管理、および web サイト、ブログ、イントラネットのコンテンツを公開するために使用の 1 つです。ユーザーを押して zip ファイルを別のファイルとすべての機能が追加されます。その拡張性の高いアーキテクチャのおかげでも web アプリケーションを構築する素晴らしい拠点です。それのために使用段階移行のコンポーネントを管理します。それ Ubuntu や CentOS と利便性。

Helpコマンド
----------------------

Help コマンドと同様、目的に関するユーザー ガイドとして JFeatures モジュールに含まれているオプションについて。それは JFeatures モジュールの代替パラメーターが一覧表示されます。また、JFeatures モジュールをインストールするための構文について説明します。JFeatures モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		ptconfigure JFeatures help

Help コマンドを宣言する構文は、大文字と小文字、追加の利点があります。次のスクリーン ショットは JFeatures の下で help コマンドについてユーザーを視覚化します。

.. code-block:: bash

 kevell@corp:/# jrush JFeature help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command manages the JFeature Component for Stage Migration.

  JFeature, jfeature

        - folder-defaults
          Reset the feature file storage folders being used to the default
          example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"

        - feature-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"

        - feature-pull
          perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
          example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

        - feature-push
          perform a push on an installed feature so it is saved locally.
          example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

        - group-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"

        - group-install-all
          Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
          Directory for group files, and install or update all found groups.
          example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"

        - group-push
          perform a push of a group profile into a locally saved file.
          example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"

        - group-pull
          perform a pull on all installed features in the specified group so they are integrated into the site, db and
          file changes executed.
          example jrush jfeature group-pull --group-id="XX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-name="my group" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-unique="XX1234" --config-file="/var/www/website/configuration.php"

 ------------------------------
 End Help
 ****************************************



代替パラメータ
-----------------------------------

宣言で定義することができます、代替パラメーターを次に示します。

JFeature, jfeature


Folder-default
----------------------

このプロセスは、ファイルの格納フォルダーに対する既定の設定に使用されます。プリセットの設定またはフォルダーで選択されていない場合に使用する値。ユーザーとの対話が必要です。この目的を果たす最も一般的に選択したオプションを既定値に設定します。

フォルダー既定プロセスのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

	 Jrush JFeature folder-defaults

次のスクリーンショットは、その機能を示しています。


.. code-block:: bash

 	folder-defaults
        Reset the feature file storage folders being used to the default
        example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"


Feature-install
----------------------

このプロセスは、データベースを移行するためのメタデータをインストールするために使用します。ここで機能ファイル名と構成ファイル名を要求します。ユーザーが 1 つずつすべて上記詳細を入力します。それ以外の場合、ユーザーは、すべて同じ単一の行として入力できます。次のコマンドは jfeature をインストールする使用されます。

.. code-block:: bash

	 Jrush JFeature feature-install


スクリーンショットは、その機能を示しています。


.. code-block:: bash

       feature-install
       Install the metadata for a database migration, fileset, or both from the GC Features component
       example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"


Feature-Pull
-------------------

フィーチャープルがインストールされている機能で、プルを実行するために使用される。インテグレーションファイルに変更があってもよいによるexecuted.The次のコマンドは、構成ファイルをプルするために使用することができる

.. code-block:: bash

	 Jrush JFeature feature-pull


上記の当該コマンドを入力した後の Ip アドレスと時間を頼みます。これに基づいてプルを実行することができます。次のスクリーン ショットでは、その機能について説明します。

.. code-block:: bash

	feature-pull
        perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
        example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
        example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

Feature-Push
--------------------

機能のプッシュ機能がインストールにプッシュを実現するために使用します。プッシュが完了するとローカルに保存することができます。機能のプッシュに使用するコマンド。

.. code-block:: bash

	 Jrush JFeature feature-push


入力後、上記の当該コマンド要求ユニークなプロファイルと構成ファイルとプッシュ型します。ユーザーが 1 つまたはすべて同じ行に入力します。これは、スナップショットを次のように説明できます。

.. code-block:: bash

 	feature-push
        perform a push on an installed feature so it is saved locally.
        example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

Group-install
-------------------

このプロセスは、データベースを移行するためのメタデータをインストールするために使用します。ここで機能グループ ファイル名と構成ファイル名を要求します。ユーザーが 1 つずつすべて上記詳細を入力します。それ以外の場合、ユーザーは同じ行にすべてのものとして入力できます。

.. code-block:: bash

	 Jrush JFeature group-install

スクリーンショットは、その機能を示しています。


.. code-block:: bash

	group-install
        Install the metadata for a database migration, fileset, or both from the GC Features component
        example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"


Group-install-all
-----------------------------

このプロセスはデータベース移行ファイルのメタデータをインストールに使用する設定。グループ構成機能のコンポーネントです。インストールと更新が可能です。次のコマンドは、グループのすべてのインストールに使用されます。

.. code-block:: bash

	 Jrush JFeature group-install-all


構成ファイルを確認上記当該コマンドを入力します。ユーザーは、構成ファイルの名前を入力できます。次のスクリーン ショット ガイド グループすべてをインストールするユーザー。

.. code-block:: bash

	group-install-all
        Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
        Directory for group files, and install or update all found groups.
        example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"



Group-push
-----------------

このプロセスは、ローカル ファイルへのグループ プロファイルのプッシュを実行できます。ここでユニークなグループと構成ファイルの名前を言及することができます。次のコマンドをローカルにグループ プロファイルをプッシュするために使用ファイルを保存します。

.. code-block:: bash

	 Jrush JFeature group-push

次のスクリーン ショット ガイド グループ プッシュをインストールするユーザー。

.. code-block:: bash

	 group-push
         perform a push of a group profile into a locally saved file.
         example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"


メリット
-----------------

* よくすべてのタイプのユーザーのためにサポート 
* アップグレードが容易 
* 検索検索賢くより、
* 強力な拡張 
* より少ない時間で行う符号化を使うし、より jfeature コマンド 
* Ubuntu で、セント OS かによく 
* 非大文字小文字の区別





