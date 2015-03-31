==============
JSUnit
==============

概要
---------

JsUnitはは、JavaScriptのためのオープンソースのユニットテストフレームワークです。それは本質的にJavaScriptにのJUnitのポートです。また、含まれる複数のブラウザと異なるOSを実行しているみとめマシン上でのテストの実行を自動化するためのプラットフォームです。これは、ユニットテストフレームワークのためのxUnitアーキテクチャのインスタンスです。 


helpコマンド
---------------

helpコマンドは、とだけでなく、 JsUnitはモジュールに含まれているオプションについての目的について、ユーザーをガイドします。また、
JsUnitはモジュールをインストールするための構文について説明します。 JsUnitはモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash

	ptconfigure JSUnit help

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash

 kevell@corp:/# ptconfigure JSUnit help 

 ****************************** 


  This command allows you to install JSUnit from a GC Repo. 

  JSUnit 

        - install 
        Installs JSUnit 
        example: ptconfigure JSUnit install 

 ------------------------------ 
 End Help 
 ****************************** 



インストール
---------------


端末上JsUnitはモジュールをインストールするために使用されるコマンドは、以下に記載されている

.. code-block:: bash

	ptconfigure JSUnit install 

上記のコマンドの絵画表現は、以下に記載されている

.. code-block:: bash


 kevell@corp:/# ptconfigure JSUnit install 

 Install JS Unit? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *          JS Unit !         * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-53509153053.sh 
 chmod 755 /tmp/ptconfigure-temp-script-53509153053.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-53509153053.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-53509153053.sh 
 --2015-03-26 11:35:31--  http://softlayer-sng.dl.sourceforge.net/project/jsunit/jsunit/2.2/jsunit2_2.zip 
 Resolving softlayer-sng.dl.sourceforge.net (softlayer-sng.dl.sourceforge.net)... 216.12.198.152 
 Connecting to softlayer-sng.dl.sourceforge.net (softlayer-sng.dl.sourceforge.net)|216.12.198.152|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 7799171 (7.4M) [application/octet-stream] 
 Saving to: ‘jsunit2_2.zip’  

 100%[========================================================================================================>] 77,99,171   11.6KB/s   in 9m 
 35s 

 2015-03-26 11:45:07 (13.2 KB/s) - ‘jsunit2_2.zip’ saved [7799171/7799171] 

 Archive:  jsunit2_2.zip 
  inflating: jsunit/bin/mac/start-firefox.sh  
  inflating: jsunit/bin/mac/start-opera9.sh  
  inflating: jsunit/bin/mac/start-safari.sh  
  inflating: jsunit/bin/mac/stop-firefox.sh  
  inflating: jsunit/bin/mac/stop-opera9.sh  
  inflating: jsunit/bin/mac/stop-safari.sh  
  inflating: jsunit/bin/unix/start-firefox.sh  
  inflating: jsunit/bin/unix/start-mozilla.sh  
  inflating: jsunit/bin/unix/start-opera9.sh  
  inflating: jsunit/bin/unix/stop-firefox.sh  
  inflating: jsunit/bin/unix/stop-mozilla.sh  
  inflating: jsunit/bin/unix/stop-opera9.sh  
  inflating: jsunit/app/BaseUiManager.js  
  inflating: jsunit/app/ClassicUiManager.js  
  inflating: jsunit/app/ModernUiManager.js  
  inflating: jsunit/app/css/jsUnitStyle.css  
  inflating: jsunit/app/css/modernStyle.css  
  inflating: jsunit/app/emptyPage.html  
  inflating: jsunit/app/jsUnitCore.js  
  inflating: jsunit/app/jsUnitParams.js  
  inflating: jsunit/app/jsUnitTestManager.js  
  inflating: jsunit/app/jsUnitTracer.js  
  inflating: jsunit/app/main-counts-errors.html  
  inflating: jsunit/app/main-counts-failures.html  
  inflating: jsunit/app/main-counts-runs.html  
  inflating: jsunit/app/main-counts.html  
  inflating: jsunit/app/main-data.html  
  inflating: jsunit/app/main-frame.html  
  inflating: jsunit/app/main-loader.html  
  inflating: jsunit/app/main-problems.html  
  inflating: jsunit/app/main-progress.html  
  inflating: jsunit/app/main-results.html  
  inflating: jsunit/app/main-status.html  
  inflating: jsunit/app/modernUi.html  
  inflating: jsunit/app/testContainer.html  
  inflating: jsunit/app/testContainerController.html  
  inflating: jsunit/bin/mac/readme.txt  
  inflating: jsunit/bin/mac/start-firefox.scpt  
  inflating: jsunit/bin/mac/start-opera9.scpt  
  inflating: jsunit/bin/mac/start-safari.scpt  
  inflating: jsunit/bin/mac/stop-firefox.scpt  
  inflating: jsunit/bin/mac/stop-opera9.scpt  
  inflating: jsunit/bin/mac/stop-safari.scpt  
  inflating: jsunit/build.xml        
  inflating: jsunit/build_aggregate.xml  
  inflating: jsunit/css/jsUnitStyle.css  
  inflating: jsunit/css/modernStyle.css  
  inflating: jsunit/doc/generate_jsdoc.sh  
  inflating: jsunit/doc/gotapi.xml   
  inflating: jsunit/doc/js_docs_out/Clock.html  
  inflating: jsunit/doc/js_docs_out/GLOBALS.html  
  inflating: jsunit/doc/js_docs_out/JsUnitAssertionArgumentError.html  
  inflating: jsunit/doc/js_docs_out/JsUnitError.html  
  inflating: jsunit/doc/js_docs_out/JsUnitFailure.html  
  inflating: jsunit/doc/js_docs_out/JsUnitTestSuite.html  
  inflating: jsunit/doc/js_docs_out/MockXmlHttpRequest.html  
  inflating: jsunit/doc/js_docs_out/Utilities.html  
  inflating: jsunit/doc/js_docs_out/allclasses-frame.html  
  inflating: jsunit/doc/js_docs_out/allclasses-noframe.html  
  inflating: jsunit/doc/js_docs_out/help-doc.html  
  inflating: jsunit/doc/js_docs_out/index-all.html  
  inflating: jsunit/doc/js_docs_out/index.html  
  inflating: jsunit/doc/js_docs_out/logo_jsunit.jpg  
  inflating: jsunit/doc/js_docs_out/overview-frame.html  
  inflating: jsunit/doc/js_docs_out/overview-jsUnitAjax.js.html  
  inflating: jsunit/doc/js_docs_out/overview-jsUnitCore.js.html  
  inflating: jsunit/doc/js_docs_out/overview-jsUnitMockTimeout.js.html  
  inflating: jsunit/doc/js_docs_out/overview-summary-jsUnitAjax.js.html  
  inflating: jsunit/doc/js_docs_out/overview-summary-jsUnitCore.js.html  
  inflating: jsunit/doc/js_docs_out/overview-summary-jsUnitMockTimeout.js.html  
  inflating: jsunit/doc/js_docs_out/overview-summary.html  
  inflating: jsunit/doc/js_docs_out/overview-tree.html  
  inflating: jsunit/doc/js_docs_out/stylesheet.css  
  inflating: jsunit/doc/jsunit.ppt   
  inflating: jsunit/doc/summary.txt  
  inflating: jsunit/images/bl0.gif   
  inflating: jsunit/images/br0.gif   
  inflating: jsunit/images/green.gif  
  inflating: jsunit/images/logo_jsunit.jpg  
  inflating: jsunit/images/nt0.gif   
  inflating: jsunit/images/pivotal.gif  
  inflating: jsunit/images/red.gif   
  inflating: jsunit/images/tl0.gif   
  inflating: jsunit/images/tr0.gif   
  inflating: jsunit/java/bin/jsunit.jar  
  inflating: jsunit/java/lib/axis_1.4/LICENSE  
  inflating: jsunit/java/lib/axis_1.4/NOTICE  
  inflating: jsunit/java/lib/axis_1.4/axis-ant.jar  
  inflating: jsunit/java/lib/axis_1.4/axis.jar  
  inflating: jsunit/java/lib/axis_1.4/jaxrpc.jar  
  inflating: jsunit/java/lib/axis_1.4/log4j-1.2.8.jar  
  inflating: jsunit/java/lib/axis_1.4/saaj.jar  
  inflating: jsunit/java/lib/axis_1.4/wsdl4j-1.5.1.jar  
  inflating: jsunit/java/lib/commons_discovery_0.2/LICENSE  
  inflating: jsunit/java/lib/commons_discovery_0.2/commons-discovery.jar  
  inflating: jsunit/java/lib/commons_httpclient_3.0.1/LICENSE.txt  
  inflating: jsunit/java/lib/commons_httpclient_3.0.1/commons-httpclient-3.0.1.jar  
  inflating: jsunit/java/lib/commons_logging_1.1/LICENSE.txt  
  inflating: jsunit/java/lib/commons_logging_1.1/commons-logging-1.1.jar  
  inflating: jsunit/java/lib/javax/javax.servlet.jar  
  inflating: jsunit/java/lib/jdom_1.0/LICENSE.txt  
  inflating: jsunit/java/lib/jdom_1.0/jdom.jar  
  inflating: jsunit/java/lib/jetty_5.1.11/LICENSE.TXT  
  inflating: jsunit/java/lib/jetty_5.1.11/org.mortbay.jetty.jar  
  inflating: jsunit/java/lib/jetty_5.1.11/start.jar  
  inflating: jsunit/java/lib/jetty_5.1.11/stop.jar  
  inflating: jsunit/java/lib/junit_4.1/cpl-v10.html  
  inflating: jsunit/java/lib/junit_4.1/junit.jar  
  inflating: jsunit/java/lib/nekohtml_0.9.5/LICENSE  
  inflating: jsunit/java/lib/nekohtml_0.9.5/LICENSE_apache  
  inflating: jsunit/java/lib/nekohtml_0.9.5/nekohtml.jar  
  inflating: jsunit/java/lib/webwork_2.2.2/license  
  inflating: jsunit/java/lib/webwork_2.2.2/oscore.jar  
  inflating: jsunit/java/lib/webwork_2.2.2/rife-continuations.jar  
  inflating: jsunit/java/lib/webwork_2.2.2/webwork-2.2.2.jar  
  inflating: jsunit/java/lib/xerces_2.8.0/LICENSE  
  inflating: jsunit/java/lib/xerces_2.8.0/LICENSE-SAX.html  
  inflating: jsunit/java/lib/xerces_2.8.0/LICENSE.DOM-documentation.html  
  inflating: jsunit/java/lib/xerces_2.8.0/LICENSE.DOM-software.html  
  inflating: jsunit/java/lib/xerces_2.8.0/LICENSE.resolver.txt  
  inflating: jsunit/java/lib/xerces_2.8.0/xercesImpl.jar  
  inflating: jsunit/java/lib/xwork_1.1/license  
  inflating: jsunit/java/lib/xwork_1.1/ognl.jar  
  inflating: jsunit/java/lib/xwork_1.1/xwork-1.1.jar  
  inflating: jsunit/jsunit.properties.sample  
  inflating: jsunit/lib/jsUnitAjax.js  
  inflating: jsunit/lib/jsUnitMockTimeout.js  
  inflating: jsunit/licenses/MPL-1.1.txt  
  inflating: jsunit/licenses/apache2.txt  
  inflating: jsunit/licenses/gpl-2.txt  
  inflating: jsunit/licenses/index.html  
  inflating: jsunit/licenses/lgpl-2.1.txt  
  inflating: jsunit/licenses/mpl-tri-license-c.txt  
  inflating: jsunit/licenses/mpl-tri-license-html.txt  
  inflating: jsunit/logging.properties  
  inflating: jsunit/readme.txt       
  inflating: jsunit/testRunner.html  
  inflating: jsunit/tests/TestPageTest.html  
  inflating: jsunit/tests/UiManagerTest.html  
  inflating: jsunit/tests/failingTest.html  
  inflating: jsunit/tests/jsUnitAjaxTest.html  
  inflating: jsunit/tests/jsUnitAssertionTests.html  
  inflating: jsunit/tests/jsUnitFrameworkUtilityTests.html  
  inflating: jsunit/tests/jsUnitMockTimeoutTest.html  
  inflating: jsunit/tests/jsUnitOnLoadTests.html  
  inflating: jsunit/tests/jsUnitParamsTests.html  
  inflating: jsunit/tests/jsUnitRestoredHTMLDivTests.html  
  inflating: jsunit/tests/jsUnitSetUpTearDownTests.html  
  inflating: jsunit/tests/jsUnitTestLoadData.html  
  inflating: jsunit/tests/jsUnitTestManagerTests.html  
  inflating: jsunit/tests/jsUnitTestSetUpPages.html  
  inflating: jsunit/tests/jsUnitTestSuite.html  
  inflating: jsunit/tests/jsUnitTestSuiteTests.html  
  inflating: jsunit/tests/jsUnitUtilityTests.html  
 Temp File /tmp/ptconfigure-temp-script-53509153053.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 JSUnit: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


メリット
----------

ブラウザ内でJavaScriptをテストするすべてのあなたのターゲットのブラウザでテストを実行できることです。これはブラウザでJavaScriptの実装で矛盾の古い問題に対処するには長い道のりを行く。
