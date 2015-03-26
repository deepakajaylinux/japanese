==============
Simpletest
==============


概要
-----------

SimpleTest は、オープン ソースの単体テスト、PHP プログラミング言語のためのフレームワークです。Simpletest フレームワークをすばやく行うため、単体テストと eassily ことができます。SimpleTest モック オブジェクトをサポートして、HTML ページを解析することができのリンクをクリックして、フォームの送信のようなものをシミュレートするスクリプト可能な HTTP クライアントと web アプリケーションの回帰テストを自動化するために使用することができます。

Helpコマンド
-------------

このコマンドは、simpletest の使用状況を判断するのに役立ちます。Simpletest の代替パラメーターを示します。また、simpletest モジュールの機能の構文について説明します。Simpletest のヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

        ptconfigure Simpletest help

上記のコマンドの絵の表現は以下します。

.. code-block:: bash

 kevell@corp:/# ptconfigure Simpletest help
 ******************************


  This command allows you to install Simpletest from a GC Repo.

  Simpletest

        - install
        Installs the simpletest
        example: ptconfigure Simpletest install

 ------------------------------
 End Help
 ******************************


インストール
-----------------

端末に simpletest モジュールをインストールするために使用されるコマンドは以下します。


.. code-block:: bash

        ptconfigure Simpletest install

上記のコマンドは xcache とその依存関係の最新バージョンをインストールすることを目指しています.

上記のコマンドの絵の表現は以下します。

.. code-block:: bash


 kevell@corp:/# ptconfigure Simpletest install
 Install Simpletest? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Simpletest!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-89998877570.sh
 chmod 755 /tmp/ptconfigure-temp-script-89998877570.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-89998877570.sh Permissions
 Executing /tmp/ptconfigure-temp-script-89998877570.sh
 --2015-03-23 18:06:49--  http://sourceforge.net/projects/simpletest/files/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz
 Resolving sourceforge.net (sourceforge.net)... 216.34.181.60
 Connecting to sourceforge.net (sourceforge.net)|216.34.181.60|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: http://sourceforge.net/projects/simpletest/files/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz/download [following]
 --2015-03-23 18:06:50--  http://sourceforge.net/projects/simpletest/files/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz/download
 Connecting to sourceforge.net (sourceforge.net)|216.34.181.60|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: http://downloads.sourceforge.net/project/simpletest/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz?r=&ts=1427114211&use_mirror=softlayer-sng [following]
 --2015-03-23 18:06:51--  http://downloads.sourceforge.net/project/simpletest/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz?r=&ts=1427114211&use_mirror=softlayer-sng
 Resolving downloads.sourceforge.net (downloads.sourceforge.net)... 216.34.181.59
 Connecting to downloads.sourceforge.net (downloads.sourceforge.net)|216.34.181.59|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: http://softlayer-sng.dl.sourceforge.net/project/simpletest/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz [following]
 --2015-03-23 18:06:52--  http://softlayer-sng.dl.sourceforge.net/project/simpletest/simpletest/simpletest_1.1/simpletest_1.1.0.tar.gz
 Resolving softlayer-sng.dl.sourceforge.net (softlayer-sng.dl.sourceforge.net)... 216.12.198.152
 Connecting to softlayer-sng.dl.sourceforge.net (softlayer-sng.dl.sourceforge.net)|216.12.198.152|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 287537 (281K) [application/x-gzip]
 Saving to: ‘simpletest_1.1.0.tar.gz’

 100%[=======================================================================================================>] 2,87,537    20.0KB/s   in 17s    

 2015-03-23 18:07:10 (16.2 KB/s) - ‘simpletest_1.1.0.tar.gz’ saved [287537/287537]

 simpletest/README
 simpletest/VERSION
 simpletest/LICENSE
 simpletest/HELP_MY_TESTS_DONT_WORK_ANYMORE
 simpletest/arguments.php
 simpletest/authentication.php
 simpletest/autorun.php
 simpletest/browser.php
 simpletest/collector.php
 simpletest/compatibility.php
 simpletest/cookies.php
 simpletest/default_reporter.php
 simpletest/detached.php
 simpletest/dumper.php
 simpletest/eclipse.php
 simpletest/encoding.php
 simpletest/errors.php
 simpletest/exceptions.php
 simpletest/expectation.php
 simpletest/form.php
 simpletest/frames.php
 simpletest/http.php
 simpletest/invoker.php
 simpletest/mock_objects.php
 simpletest/page.php
 simpletest/php_parser.php
 simpletest/recorder.php
 simpletest/reflection_php4.php
 simpletest/reflection_php5.php
 simpletest/remote.php
 simpletest/reporter.php
 simpletest/scorer.php
 simpletest/selector.php
 simpletest/shell_tester.php
 simpletest/simpletest.php
 simpletest/socket.php
 simpletest/tag.php
 simpletest/test_case.php
 simpletest/tidy_parser.php
 simpletest/unit_tester.php
 simpletest/url.php
 simpletest/user_agent.php
 simpletest/web_tester.php
 simpletest/xml.php
 simpletest/extensions/pear_test_case.php
 simpletest/extensions/testdox.php
 simpletest/extensions/testdox/test.php
 simpletest/test/acceptance_test.php
 simpletest/test/adapter_test.php
 simpletest/test/all_tests.php
 simpletest/test/arguments_test.php
 simpletest/test/authentication_test.php
 simpletest/test/bad_test_suite.php
 simpletest/test/browser_test.php
 simpletest/test/collector_test.php
 simpletest/test/command_line_test.php
 simpletest/test/compatibility_test.php
 simpletest/test/cookies_test.php
 simpletest/test/detached_test.php
 simpletest/test/dumper_test.php
 simpletest/test/eclipse_test.php
 simpletest/test/encoding_test.php
 simpletest/test/errors_test.php
 simpletest/test/exceptions_test.php
 simpletest/test/expectation_test.php
 simpletest/test/form_test.php
 simpletest/test/frames_test.php
 simpletest/test/http_test.php
 simpletest/test/interfaces_test.php
 simpletest/test/interfaces_test_php5_1.php
 simpletest/test/live_test.php
 simpletest/test/mock_objects_test.php
 simpletest/test/page_test.php
 simpletest/test/parse_error_test.php
 simpletest/test/php_parser_test.php
 simpletest/test/parsing_test.php
 simpletest/test/parsing_test.php
 simpletest/test/recorder_test.php
 simpletest/test/reflection_php5_test.php
 simpletest/test/remote_test.php
 simpletest/test/shell_test.php
 simpletest/test/shell_tester_test.php
 simpletest/test/simpletest_test.php
 simpletest/test/socket_test.php
 simpletest/test/tag_test.php
 simpletest/test/test_with_parse_error.php
 simpletest/test/unit_tests.php
 simpletest/test/unit_tester_test.php
 simpletest/test/autorun_test.php
 simpletest/test/url_test.php
 simpletest/test/user_agent_test.php
 simpletest/test/visual_test.php
 simpletest/test/web_tester_test.php
 simpletest/test/xml_test.php
 simpletest/test/support/collector/collectable.1
 simpletest/test/support/collector/collectable.2
 simpletest/test/support/upload_sample.txt
 simpletest/test/support/supplementary_upload_sample.txt
 simpletest/test/support/latin1_sample
 simpletest/test/support/spl_examples.php
 simpletest/test/support/empty_test_file.php
 simpletest/test/support/test1.php
 simpletest/test/support/failing_test.php
 simpletest/test/support/passing_test.php
 simpletest/test/support/recorder_sample.php
 simpletest/test/site/file.html
 simpletest/docs/en/docs.css
 simpletest/docs/en/index.html
 simpletest/docs/en/overview.html
 simpletest/docs/en/unit_test_documentation.html
 simpletest/docs/en/group_test_documentation.html
 simpletest/docs/en/mock_objects_documentation.html
 simpletest/docs/en/partial_mocks_documentation.html
 simpletest/docs/en/reporter_documentation.html
 simpletest/docs/en/expectation_documentation.html
 simpletest/docs/en/web_tester_documentation.html
 simpletest/docs/en/form_testing_documentation.html
 simpletest/docs/en/authentication_documentation.html
 simpletest/docs/en/browser_documentation.html
 simpletest/docs/fr/docs.css
 simpletest/docs/fr/index.html
 simpletest/docs/fr/overview.html
 simpletest/docs/fr/unit_test_documentation.html
 simpletest/docs/fr/group_test_documentation.html
 simpletest/docs/fr/mock_objects_documentation.html
 simpletest/docs/fr/partial_mocks_documentation.html
 simpletest/docs/fr/reporter_documentation.html
 simpletest/docs/fr/expectation_documentation.html
 simpletest/docs/fr/web_tester_documentation.html
 simpletest/docs/fr/form_testing_documentation.html
 simpletest/docs/fr/authentication_documentation.html
 simpletest/docs/fr/browser_documentation.html
 Temp File /tmp/ptconfigure-temp-script-89998877570.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 Simpletest: Success
 ------------------------------
 Installer Finished
 ******************************



アンインストール
--------------------


端末に simpletest モジュールをアンインストールするために使用されるコマンドは以下します。

.. code-block:: bash

        ptconfigure Simmpletest uninstall

上記のコマンドの絵の表現は以下します。

.. code-block:: bash


 kevell@corp:/# ptconfigure Simpletest uninstall
 Uninstall Simpletest? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Simpletest!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-749272393.sh
 chmod 755 /tmp/ptconfigure-temp-script-749272393.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-749272393.sh Permissions
 Executing /tmp/ptconfigure-temp-script-749272393.sh
 Temp File /tmp/ptconfigure-temp-script-749272393.sh Removed
 ... All done!
 *******************************
 
 Single App Uninstaller:
 ------------------------------
 Simpletest: Success
 ------------------------------
 UnInstaller Finished
 ******************************


メリット
-----------

* 簡単に別のテストを実行し 
* クイック テストの開発を促進を支援 
* web インタ フェースをテストするために必要な 
* 簡単に何が間違っている区別する開発者ことができます






