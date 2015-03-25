====================
EnvironmentConfig
====================

概要
-------------

このモジュールは、プロジェクトに必要な環境を構成するユーザーを促進します。私たちを見てみましょう、環境を構成する方法、不要な環境を削除する方法リスト今後のテーマで利用可能な環境の一覧オプションを使用する方法。

Helpコマンド
--------------------

その代替のパラメーター宣言で使用されている、モジュールの目的に関するユーザー ヘルプ コマンドについて説明します。環境の構成のリストである 3 つの機能を強調表示、構成、削除します。また、3 つの主要な機能を使用する構文を指定します。助けを宣言するために使用する構文は以下の通りです。


.. code-block:: bash

		ptdeploy envconfig help

次のスクリーン ショットは、help コマンドの働きについて絵を示しています。

.. code-block:: bash


 kevell@corp:/# ptdeploy EnvironmentConfig help
 ******************************


  This command is part of a default Module and provides you with a method by which you can
  configure environments for your project from the command line. Currently compliant with
  both ptdeploy and ptconfigure.


  EnvironmentConfig, environmentconfig, environment-config, envconfig, env-config

        - list
        List current environments
        example: ptconfigure envconfig list --yes

        - configure, config
        Configure the environments for your project to use
        example: ptconfigure envconfig config
        example: ptconfigure envconfig config --keep-current-environments

        - delete, del
        Configure the environments for your project to use
        example: ptconfigure envconfig delete
        example: ptconfigure envconfig del --environment-name="staging"


 ------------------------------
 End Help
 ******************************


どのように環境を構成するには
----------------------------------------------

環境構成の目的のため、ユーザーは、次のコマンドを使用できます。


.. code-block:: bash

		ptdeploy envconfig config

入力した後、次の操作上のコマンド起こる示すよう。

Step 1: Configure Environments Here? (Y/N)

ユーザは、入力YまたはNに持っている

Step 2: Use existing environment Settings? (Y/N)

ユーザは、入力YまたはNに持っている

場合は、ユーザー入力の Y として既に既存の続行されます。

として環境に関する情報が要求される場合は N と入力します。

Value for: Name of the environment

Value for: Default temp dir(Location)

上記の手順後ユーザーは、次の詳細を入力する必要があります。

Enter target?

Enter user?

Enter password?

Add Another Server? (Y/N)

ユーザは、入力YまたはNに持っている

最後に、環境の構成を取得成功に描かれている、以下のスクリーン ショット。

.. code-block:: bash

 kevell@corp:/# ptconfigure envconfig config
 Configure Environments Here? (Y/N) 
 Y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevells
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /home/kevells
 Enter user ?
 kevells
 Enter password ?
 123456
 Add Another Server? (Y/N)
 N
 ******************************


 Success
 In Environment Configuration
 ******************************


環境を構成するとき、ユーザーが現在の環境と設定したい場合彼ら使用できます、次のコマンド:

.. code-block:: bash

		ptdeploy envconfig config --keep-current-environments


上記のコマンドを入力した後、次の詳細を表形式で示すように要求は。


.. cssclass:: table-bordered

 +-------------------------------------+------------+------------------------------------------------------------------------------+
 | パラメータ                          | オプション | 注釈                                                                         |
 +=====================================+============+==============================================================================+
 |Configure Environments Here? (Y/N)   | Y          | ユーザーは、現在の環境を設定する場合                                         |
 |                                     |            | 彼らはYとして入力できる環境                                                  |
 +-------------------------------------+------------+------------------------------------------------------------------------------+
 |Configure Environments Here? (Y/N)   | N          | ユーザーは、環境を構成することを望まない場合は                               |
 |                                     |            | 彼らは、Nとして入力することができ、現在の環境                                |
 +-------------------------------------+------------+------------------------------------------------------------------------------+
 |Use existing environment             | Y          | ユーザーは、既存の環境設定を使用したい場合                                   |
 |settings? (Y/N)                      |            | Y.として彼らが入力できる                                                     |
 +-------------------------------------+------------+------------------------------------------------------------------------------+
 |Use existing environment             | N          | ユーザは、既存の環境設定を使用したくない場合、                               |
 |settings? (Y/N)                      |            | それらはN.として入力することができる                                         |
 +-------------------------------------+------------+------------------------------------------------------------------------------+
 |Do you want to add another           | Y          | ユーザーが別の環境を追加したい場合は、 Yと入力をすることができます           |
 |environment? (Y/N)                   |            |                                                                              |
 +-------------------------------------+------------+------------------------------------------------------------------------------+
 |Do you want to add another           | N          | ユーザが別の環境を追加したくない場合、それらはN.として入力することができ     |
 |environment? (Y/N)|                  |            |                                                                              |
 +-------------------------------------+------------+------------------------------------------------------------------------------+ 





次のスクリーンショットは、絵画的に、上記のプロセスを表しています。


.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig config --keep-current-environments
 Configure Environments Here? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 N
 ******************************


 Success
 In Environment Configuration
 ******************************




環境設定を削除する方法
-------------------------------------------------------

環境構成を削除する必要がある場合、次のコマンドを入力することができます。


.. code-block:: bash

		ptdeploy envconfig del --environment-name="kevells"

ユーザーは、上記のように削除したい環境の名前を指定できます。

上記のコマンドを入力した後、それが要求されます

Step 1: Delete Environments Here?

警告メッセージとしてを示してい


.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 


ユーザーは、 YまたはNを指定する必要があります


Step 2: Environment Kevells(Name of the specified environment that is supposed to delete) found. Are you sure want to delete it? (Y/N)

ユーザーは、 YまたはNを指定する必要があります

最後に、スクリーン ショットに示すように、指定された環境が削除されます。

.. code-block:: bash

 kevell@corp:/# ptconfigure envconfig del --environment-name="kevells"
 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 Y
 Environment kevells found. Are you sure you want to delete it? (Y/N) 
 Y
 [Pharaoh Logging] Removing environment kevells.
 ******************************


 Success
 In Environment Configuration
 ******************************



環境の名前を指定せずによって環境を削除する別の方法は、コマンドを使用して示すように。


.. code-block:: bash

		ptdeploy envconfig delete

上記のコマンドを入力した後、それが要求されます

Step 1: Delete Environments Here?

警告メッセージとしてを示してい

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 


ユーザーは、 YまたはNを指定する必要があります

スクリーンショットに示すように、最後に、環境が削除されます


.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig delete
 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 Y
 PHP Notice:  Undefined index: environment-name in /opt/ptdeploy/ptdeploy/src/Modules/EnvironmentConfig/Model/EnvironmentConfigAllLinux .php on line 161
 PHP Notice:  Undefined index: environment-name in /opt/ptdeploy/ptdeploy/src/Modules/EnvironmentConfig/Model/EnvironmentConfigAllLinux .php on line 161
 ******************************


 Success
 In Environment Configuration
 ******************************



環境構成を一覧表示する方法
--------------------------------------------------

場合は、ユーザー環境の構成に関する詳細情報の一覧を表示する場合、彼らのようにを入力できます。

.. code-block:: bash

		ptdeploy envconfig list

上記のコマンドを入力した後、それは意志が尋ね

List Environment Here? (Y/N)

Y として指定した場合の出力のスクリーン ショットに示すように表示が生成されます。

.. code-block:: bash

 kevell@corp:/# ptdeploy envconfig list
 List Environments Here? (Y/N) 
 Y
 ******************************


 array(2) {
  [0]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(13) "default-local"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(9) "127.0.0.1"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
  [1]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(18) "default-local-8080"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(14) "127.0.0.1:8080"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
 }

 In Environment Configuration
 ******************************


代替パラメータ
--------------------------------
 
Envconfig の代わりに、次のパラメーターを宣言で使用することができます。

* EnvironmentConfig
* environmentconfig
* environment-config
* env-config

メリット
------------

* それは裕福な両方セント OS とも ubuntu のように。
* パラメーターの宣言で使用しない大文字と小文字は他と比較される間、加えられた利点であります。
* このモジュールは、環境を構成する方法、ユーザーをリード削除不要な環境をどのように利用
  可能環境のリストの [リスト] オプションを使用する方法。


