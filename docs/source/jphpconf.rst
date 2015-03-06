============
phpconf
============


あらすじ
---------

このモジュールをインストールするのと同様 php の設定を管理するよう支援します。ユーザーは、インストールの実行の時に彼らの要件に従って構成をフレームすることができます。


ヘルプ コマンド
------------------

ヘルプ コマンドこの php 設定での作業にユーザーをリードします。また、インストールに使用するコマンドを指定します。ヘルプ コマンドも使用することができますの代替パラメーターを一覧表示します。Php 設定オプションのために使用されるコマンドは以下の通りです。

.. code-block:: bash

	ptconfigure PHPConf help

スクリーン ショット下に与えられたは、php の設定でヘルプの使用に関する表現を示します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  PHPConf, php-configure, php-configuration, php-conf, phpconf

        - install
        Installs a configuration for PHP
        example: ptconfigure phpconf install

 ------------------------------
 End Help
 ******************************


インストール
---------------

Php の設定をインストールの要件に従って構成をフレームすることができます、ユーザーにとって有益です。インストールに使用するコマンドは次のとおりです。


.. code-block:: bash

		ptconfigure PHPConf install

表形式で表示されますを入力した後、次の操作上記のようにコマンドに発生します。


.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf install
 Install PHP Conf? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Conf!        *
 *******************************
 Set non-default value for user_ini.filename? Default is .user.ini (Y/N)
 y
 What value for user_ini.filename?

 Set non-default value for user_ini.cache_ttl? Default is 300 (Y/N)
 
 Set non-default value for engine? Default is On (Y/N)

 Set non-default value for short_open_tag? Default is On (Y/N)

 Set non-default value for asp_tags? Default is Off (Y/N)

 Set non-default value for precision? Default is 14 (Y/N)

 Set non-default value for y2k_compliance? Default is On (Y/N)

 Set non-default value for output_buffering? Default is 4096 (Y/N)

 Set non-default value for output_handler? Default is  (Y/N)

 Set non-default value for zlib.output_compression? Default is Off (Y/N)

 Set non-default value for zlib.output_compression_level? Default is -1 (Y/N)

 Set non-default value for zlib.output_handler? Default is  (Y/N)

 Set non-default value for implicit_flush? Default is Off (Y/N)

 Set non-default value for unserialize_callback_func? Default is  (Y/N)

 Set non-default value for serialize_precision? Default is 17 (Y/N)

 Set non-default value for allow_call_time_pass_reference? Default is Off (Y/N)

 Set non-default value for safe_mode? Default is Off (Y/N)

 Set non-default value for safe_mode_gid? Default is Off (Y/N)

 Set non-default value for safe_mode_exec_dir? Default is  (Y/N)

 Set non-default value for safe_mode_allowed_env_vars? Default is PHP_ (Y/N)

 Set non-default value for safe_mode_protected_env_vars? Default is LD_LIBRARY_PATH (Y/N)

 Set non-default value for open_basedir? Default is  (Y/N)

 Set non-default value for disable_functions? Default is pcntl_alarm,pcntl_fork,pcntl_waitpid,pcntl_wait,pcntl_wifexited,pcntl_wifstopped,pcntl_wifsignaled,pcntl_wexitstatus,pcntl_wtermsig,pcntl_wstopsig,pcntl_signal,pcntl_signal_dispatch,pcntl_get_last_error,pcntl_strerror,pcntl_sigpr ocmask,pcntl_sigwaitinfo,pcntl_sigtimedwait,pcntl_exec,pcntl_getpriority,pcntl_setpriority, (Y/N)

 Set non-default value for disable_classes? Default is  (Y/N)

 Set non-default value for ignore_user_abort? Default is On (Y/N)

 Set non-default value for realpath_cache_size? Default is 16k (Y/N)

 Set non-default value for realpath_cache_ttl? Default is 120 (Y/N)

 Set non-default value for zend.enable_gc? Default is On (Y/N)

 Set non-default value for expose_php? Default is On (Y/N)

 Set non-default value for max_execution_time? Default is 30 (Y/N)

 Set non-default value for max_input_time? Default is 60 (Y/N)

 Set non-default value for max_input_nesting_level? Default is 64 (Y/N)

 Set non-default value for max_input_vars? Default is 1000 (Y/N)

 Set non-default value for memory_limit? Default is 128M (Y/N)



 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPConf: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
------------

.. cssclass:: table-bordered

 +-------------------------+-----------------------------------------+--------------+----------------------------------------------------+
 | パラメーター            | 代替パラメーター                        | 必要な       | コメント                                           |
 +=========================+=========================================+==============+====================================================+
 |Install PHPConf?(Y/N)    | の代わりにPHP Confこれらの代替名を使    | Y(Yes)       | ユーザーは、Yとして入力することができます          |
 |                         | 用することができます: php-configure,    |              | nstallationプロセスを続行したい場合                |
 |                         | php-conf                                |              |                                                    |
 +-------------------------+-----------------------------------------+--------------+----------------------------------------------------+
 |Install PHPConf? (Y/N)   | の代わりにPHP Confこれらの代替名を使    | N(No)        | ユーザーは、Nと入力することができ、                |
 |                         | 用することができます: php-configure,    |              | インストールプロセスを終了したい場合は             |
 |                         | php-conf|                               |              |                                                    |
 +-------------------------+-----------------------------------------+--------------+----------------------------------------------------+


ユーザー インストールの実行中、インストール プロセスの進行、モジュール構成の既定値を指定し、また問い合わせをユーザーの要件に従って構成をデフォルト以外の値を言及します。インストール中に構成の仕様を以下に示します。

* User_ini.filename の値
* user_ini.cache_ttl の値ですか？
* エンジンの値です。
* short_open_tag の値です。
* asp_tags の値です。
* 精度の値です。
* y2k_compliance の値です。
* :output_buffering の値です。
* 出力ハンドラーの値です。
* zlib.output_compression の値です。
* zlib.output_compression_level の値です。
* zlib.output_handler の値です。
* implicit_flush の値です。
* unserialize_callback_func の値です。
* 値の精度をシリアル化します。
* allow_call_time_pass_reference の値です。
* セーフモードの値です。
* safe_mode_gid の値です。
* safe_mode_exec_dir の値ですか？
* safe_mode_allowed_env_vars の値です。
* オープン basedir 値です。
* 無効にする機能の値。
* disable_classes の値ですか？
* ignore_user_abort の値
* realpath_cache_size の値ですか？
* realpath_cache_ttl の値です。
* zend.enable_gc の値です。
* 暴露記事 _php の値です。
* max_execution_time の値です。
* に関する注記の値です。
* max_input_nesting_level の値です。
* max_input_vars の値です。
* memory_limits の値です。

設定機能の既定値を見て後、ユーザーは彼らの行動を決めることができます。(名) として入力できる場合は、既定値を持つ樽構成値を指定する必要がある場合は Y として入力することができます。スクリーン ショット以下のように視覚的に上記に説明したプロセスについて説明します。


利点
--------

* インストール、ヘルプ コマンドを定義するために使用されるパラメーターの大文字と小文字は区別されません。
* ユーザー インストールの実行時構成機能をフレームすることができます。
* それ動作しますよくセント OS と windows の両方。
 

