===========
Dapperfy
===========

概要
------------

Dapperfyは彼らのプロジェクトのためのオートパイロットのファイルの標準セットを作成する際に、ユーザーを助け、サポートするデフォルトのコアモジュールの細かい部分です。ユーザーは、デフォルトのアプリケーションの設定を行うことができます。たとえば、次のようにMySQLの管理者ユーザ、ホスト、合格。
私たちは今後のトピックからこのモジュールの下にDapperの標準とDapperのリスト関数を使用する方法を見てみましょう。

helpコマンド
--------------------

、とも宣言に使用される構文：helpコマンドは、その主な用途としてdapperfyに関するすべての必要な情報、宣言で使用できる代替パラメータのリストを包んで、dapperfyの主な機能（標準、リスト例）何これらの興味深い機能している。以下のコマンドは、dapperfy下のヘルプオプションを宣言するために使用されている

.. code-block:: bash


	ptdeploy Dapperfy help

以下のスクリーンショットは、helpコマンドの操作方法の絵で示している。

.. code-block:: bash

 kevell@corp:/# ptdeploy Dapperfy help
 ******************************


  This command is part of a default Module Core and provides you with a method by which you can
  create a standard set of Autopilot files for your project from the command line.
  You can configure default application settings, ie: mysql admin user, host, pass


  Dapperfy, dapperfy

        - list
        List all of the autopilot files in your build/config/ptdeploy/autopilots
        example: ptdeploy dapperfy list

        - standard
        Create a standard set of autopilots to manage
        example: ptdeploy dapperfy standard

        The start of the command will be ptdeploy autopilot execute *filename*

        
 --------------
  Drupal Module:

  The Drupal module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Drupal site. This module adds the 'drupal' action to dapperfy.

  - drupal
  create drupal tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy drupal --yes --guess

 --------------
  Joomla Module:

  The Joomla module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Joomla site. This module adds the 'joomla' action to dapperfy.

  - joomla, joomla30
  create joomla tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy joomla --yes --guess

  - joomla-phlagrant, joomla30-phlagrant
  create joomla tailored automated deployment ptdeploy autopilots for your Phlagrant Virtual Machines
  example: ptdeploy dapperfy joomla-phlagrant --yes --guess
 --------------
  Wordpress Module:

  The Wordpress module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Wordpress site. This module adds the 'wordpress' action to dapperfy.

  - wordpress
  create wordpress tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy wordpress --yes --guess
 ------------------------------
 End Help
 ******************************

Dapperの標準を使用する方法
---------------------------------------

dapperfy標準のために使用されるコマンドは、以下の通りです

.. code-block:: bash

	ptdeploy dapperfy standard

上記のコマンドを入力した後、以下の表に示すように、次の処理は、ステップバイステップごとに発生します。

.. cssclass:: table-bordered

 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+
 | パラメータ              | 別のパラメータ      | 別のパラメータ | 注釈                                                                |
 +=========================+=====================+================+=====================================================================+
 |Dapperfy This? (Y/N)     | dapperfy, Dapperfy  | Y(Yes)         | ユーザーは、Yと入力することができますdapperfyingプロセスを          |
 |                         |                     |                | 続行したい場合                                                      |
 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+
 |Dapperfy This? (Y/N)     | dapperfy, Dapperfy  | N(No)          | ユーザーは、Nと入力することができますdapperfyingプロセスを終了      |
 |                         |                     |                | したい場合は                                                        |
 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+
 |Use existing environment |                     | Y(Yes)         | ユーザーは、Yと入力することができ、既存の環境設定を続行したい場合は |
 |settings? (Y/N)          |                     |                |                                                                     |
 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+
 |Use existing environment |                     | N(No)          | ユーザー願いが新しい環境設定を続行する場合、                        |
 |settings? (Y/N)          |                     |                | それらはNとして入力をすることができます                             |
 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+
 |Do you want to add       |                     | Y(Yes)         | ユーザーは、Yとして彼らができる入力をdapperfying                    |
 |another environment?     |                     |                | ための別の環境を追加したい場合                                      |
 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+
 |Do you want to add       |                     | N(No)          | ユーザはN.としてそれらを入力することができるがdapperfying           |
 |another environment?     |                     |                | ために別の環境を追加する必要性にない場合|                           |
 +-------------------------+---------------------+----------------+---------------------------------------------------------------------+


スクリーンショットの2つの異なるタイプのdapperfyingプロセスの図的表現を定義するユーザーのために有用であり得る。第二のスクリーンショットは、既存の環境設定を使用して意欲を指定する方法を示している。

.. code-block:: bash


 kevell@corp:/# ptdeploy dapperfy standard
 Dapperfy This? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 ******************************


 Success
 In Dapperfy
 ******************************

Dapperfyリストの使い方
---------------------------------

リスト機能の主な目的は、特定の場所で利用可能なユーザーはプロジェクトのオートパイロットのすべてのファイルをリストすることです。 dapperfyの下のリストを使用するための構文は、以下の通りです

.. code-block:: bash

	ptdeploy dapperfy list

下図のスクリーンショットは、dapperfyの下のリストオプションの動作を示している。

メリット
-----------

* これは、セントのOSのように裕福な両方のUbuntuで、同様である。
* 宣言で使用されるパラメータは、大文字と小文字を区別しません。
* ユーザーは、自分のプロジェクトのために利用可能なオートパイロットファイルのリストを表示することができます。
* dapperfyingながら、ユーザーが必要とする環境設定を指定することができます。
* 多くの環境では、dapperfyに追加することができます。
