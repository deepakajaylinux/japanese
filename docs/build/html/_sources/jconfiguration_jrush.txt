==================
JConfiguration
==================

概要
------------

このモジュールは基関数のデータを処理する既定のモジュールの一部です。今後のテーマにリセットを構成する方法を見てみましょう。

Helpコマンド
--------------------

モジュールの目的に関するユーザー ヘルプ コマンドについて説明します。それは宣言で使用することができます、代替パラメーターが一覧表示されます。それは構成およびリセットするための 2 つの異なる構文を指定します。ヘルプ オプションを使用するコマンドを次に示します。


.. code-block:: bash

		jrush jconf help

次のスクリーン ショットは、help コマンドの働きについて絵を示しています。


.. code-block:: bash

 kevell@corp:/# jrush jconf help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command is part of Default Modules and handles Databasing Functions.

  JConfiguration, jconfigure, jconfiguration, jconf

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy jconf conf joomla
      example: ptdeploy jconf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user=""

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy jconf reset drupal
      example: ptdeploy jconf reset --yes --platform=joomla30

      
 ------------------------------
 End Help
 ****************************************

どのように構成する
----------------------

のconfigure Joomlaのに使用するコマンドを以下に示します。

.. code-block:: bash

		jrush jconf conf joomla

上記のコマンドを入力した後、それが要求されます

.. cssclass:: table-bordered

 +----------------------------------+---------------------------------------+------------+-------------------------------------------+
 | パラメータ                       | 代替パラメータ                        | オプション | 注釈                                      |
 +==================================+=======================================+============+===========================================+
 |Do you want to configure          | の代わりに conf 我々はまた、使用す    | Y          | ユーザーの願い、設定する場合、それらは、  |
 |Joomla? (Y/N)	                    | ることができます configure.           | 		 | Yなどの入力をすることができます           |
 +----------------------------------+---------------------------------------+------------+-------------------------------------------+
 |Do you want to configure          | の代わりに conf 我々はまた、使用す    | N          | ユーザーが設定を希望しない場合、それらは、|
 |Joomla? (Y/N)                     | ることができます configure.           |            | Nとして入力をすることができます|          |
 +----------------------------------+---------------------------------------+------------+-------------------------------------------+

構成するユーザーの収入、それは場合は、次のデフォルト以外の値を設定したいかどうかがユーザーに問い合わせます。それはまたデフォルト値を指定します。

* Set non-default values for log_path?
* Set non-default values for temp_path?
* Set non-default values for MetaAuthor?
* Set non-default values for MetaDesc?
* Set non-default values for MetaKeys?
* Set non-default values for MetaRights?
* Set non-default values for MetaTitle?
* Set non-default values for MetaVersion?
* Set non-default values for access?
* Set non-default values for cache_handler?
* Set non-default values for cachetime?
* Set non-default values for frontediting?
* Set non-default values for assest_id?
* Set non-default values for user?
* Set non-default values for db?
* Set non-default values for host?
* Set non-default values for password?


最後に、スクリーン ショットで示されている構成のプロセスを取得完了しました。

.. code-block:: bash

 kevell@corp:/# jrush jconf conf joomla
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 Do you want to configure Joomla? (Y/N) 
 Y
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationDataJoomla3.php on line 141
 Set non-default value for log_path? Default is /logs (Y/N) 

 Set non-default value for tmp_path? Default is /tmp (Y/N) 

 Set non-default value for MetaAuthor? Default is 1 (Y/N) 

 Set non-default value for MetaDesc? Default is  (Y/N) 

 Set non-default value for MetaKeys? Default is  (Y/N) 
 
 Set non-default value for MetaRights? Default is  (Y/N) 

 Set non-default value for MetaTitle? Default is 1 (Y/N) 

 Set non-default value for MetaVersion? Default is 0 (Y/N) 

 Set non-default value for access? Default is 1 (Y/N) 
 
 Set non-default value for cache_handler? Default is file (Y/N) 

 Set non-default value for cachetime? Default is 15 (Y/N) 

 Set non-default value for caching? Default is 0 (Y/N) 

 Set non-default value for captcha? Default is 0 (Y/N) 

 Set non-default value for cookie_domain? Default is  (Y/N) 

 Set non-default value for cookie_path? Default is  (Y/N) 

 Set non-default value for dbprefix? Default is jos_ (Y/N) 

 Set non-default value for dbtype? Default is mysqli (Y/N) 

 Set non-default value for debug? Default is 0 (Y/N) 

 Set non-default value for debug_lang? Default is 0 (Y/N) 

 Set non-default value for display_offline_message? Default is 1 (Y/N) 

 Set non-default value for editor? Default is jce (Y/N) 

 Set non-default value for error_reporting? Default is default (Y/N) 

 Set non-default value for feed_email? Default is author (Y/N) 

 Set non-default value for feed_limit? Default is 10 (Y/N) 

 Set non-default value for force_ssl? Default is 0 (Y/N) 

 Set non-default value for fromname? Default is  (Y/N) 

 Set non-default value for ftp_enable? Default is 0 (Y/N) 

 Set non-default value for ftp_host? Default is  (Y/N) 

 Set non-default value for ftp_pass? Default is  (Y/N) 
 
 Set non-default value for ftp_port? Default is 21 (Y/N) 

 Set non-default value for ftp_root? Default is  (Y/N) 

 Set non-default value for ftp_user? Default is  (Y/N) 

 Set non-default value for gzip? Default is 1 (Y/N) 

 Set non-default value for helpurl? Default is http://help.joomla.org/proxy/index.php?option=com_help&keyref=Help{major}{minor}:{keyref} (Y/N) 

 Set non-default value for lifetime? Default is 60 (Y/N) 

 Set non-default value for list_limit? Default is 20 (Y/N) 

 Set non-default value for live_site? Default is  (Y/N) 

 Set non-default value for mailer? Default is mail (Y/N) 

 Set non-default value for mailfrom? Default is  (Y/N) 

 Set non-default value for memcache_compress? Default is 0 (Y/N) 

 Set non-default value for memcache_persist? Default is 1 (Y/N) 

 Set non-default value for memcache_server_host? Default is localhost (Y/N) 

 Set non-default value for memcache_server_port? Default is 11211 (Y/N) 

 Set non-default value for offline? Default is 0 (Y/N) 

 Set non-default value for offline_image? Default is  (Y/N) 

 Set non-default value for offline_message? Default is This site is down for maintenance.<br /> Please check back again soon. (Y/N) 

 Set non-default value for offset? Default is Europe/London (Y/N) 

 Set non-default value for offset_user? Default is UTC (Y/N) 

 Set non-default value for robots? Default is  (Y/N) 

 Set non-default value for secret? Default is  (Y/N) 

 Set non-default value for sef? Default is 1 (Y/N) 

 Set non-default value for sef_rewrite? Default is 1 (Y/N) 

 Set non-default value for sef_suffix? Default is 0 (Y/N) 

 Set non-default value for sendmail? Default is /usr/sbin/sendmail (Y/N) 

 Set non-default value for session_handler? Default is database (Y/N) 

 Set non-default value for sitename? Default is  (Y/N) 

 Set non-default value for sitename_pagetitles? Default is 1 (Y/N) 

 Set non-default value for smtpauth? Default is 0 (Y/N) 

 Set non-default value for smtphost? Default is localhost (Y/N) 

 Set non-default value for smtppass? Default is  (Y/N) 

 Set non-default value for smtpport? Default is 25 (Y/N) 

 Set non-default value for smtpsecure? Default is none (Y/N) 

 Set non-default value for smtpuser? Default is  (Y/N) 

 Set non-default value for unicodeslugs? Default is 0 (Y/N) 

 Set non-default value for memcached_persist? Default is 1 (Y/N) 

 Set non-default value for memcached_compress? Default is 0 (Y/N) 

 Set non-default value for memcached_server_host? Default is localhost (Y/N) 

 Set non-default value for memcached_server_port? Default is 11211 (Y/N) 

 Set non-default value for proxy_enable? Default is 0 (Y/N) 

 Set non-default value for proxy_host? Default is  (Y/N) 

 Set non-default value for proxy_port? Default is  (Y/N) 

 Set non-default value for proxy_user? Default is  (Y/N) 

 Set non-default value for proxy_pass? Default is  (Y/N) 

 Set non-default value for mailonline? Default is 1 (Y/N) 

 Set non-default value for session_memcache_server_host? Default is localhost (Y/N) 

 Set non-default value for session_memcache_server_port? Default is 11211 (Y/N) 

 Set non-default value for session_memcached_server_host? Default is localhost (Y/N) 

 Set non-default value for session_memcached_server_port? Default is 11211 (Y/N) 

 Set non-default value for frontediting? Default is 1 (Y/N) 

 Set non-default value for asset_id? Default is 1 (Y/N) 

 Set non-default value for user? Default is  (Y/N) 

 Set non-default value for db? Default is  (Y/N) 

 Set non-default value for host? Default is  (Y/N) 

 Set non-default value for password? Default is  (Y/N) 

 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 85
 PHP Warning:  file(): Filename cannot be empty in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 85
 PHP Warning:  Invalid argument supplied for foreach() in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 90
 Please check Joomla 3.x Series Settings file: 

 Is this Okay? (Y/N) 
 Y
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 119
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 120
 Removing old settings file ...
 
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 114
 Moving new settings file  in...
 PHP Notice:  Undefined index: config-file in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on line 115
 PHP Warning:  file_put_contents(): Filename cannot be empty in /opt/jrush/jrush/src/Modules/JConfiguration/Model/JConfigurationAllOS.php on li ne 115
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 1Joomla Configuration Finished
 ****************************************



設定している間、それは意志がユーザーとしてを要求
 


.. code-block:: bash

	Please check Jomla 3.x Series Settings file:

Is this Okay? (Y/N)

ユーザーは、 YまたはNを指定する必要が

リセットする方法
--------------------

The command used for reset is shown below:

.. code-block:: bash
 
		jrush jconf reset drupal

以下に示すスクリーン ショットを視覚的にリセットのプロセスについて示しています

メリット
-----------

* それは裕福な両方セント OS とも ubuntu のように。
* パラメーターの宣言で使用しない大文字と小文字は他と比較される間、加えられた利点であります。
* ユーザーは、構成中、デフォルト以外の値を指定できます。


