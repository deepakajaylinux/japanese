=============
Aptana 
=============

概要
------

Aptanaのは、Webアプリケーションを構築するためのオープンソースの統合開発環境（IDE）である。使用このコマンドは、ユーザーがAptanaのをインストールできるようにする。これは、Eclipse上.BasedオープンソースのWeb開発である、それはサポートしてJavaScriptを、HTML、DOMとコード補完、アウトライン、JavaScriptのデバッグ、エラーや警告の通知と統合されたドキュメントとCSS。追加のプラグインは、Aptanaのは、PHPやPython、Perlをサポートできるようにする。 Aptanaのは、Windows、Mac OS XおよびLinux上のスタンドアロンとして、またはEclipseのプラグインとして利用可能です。

Helpコマンド
--------------

helpコマンドは、とだけでなく、Aptanaのモジュールに含まれているオプションについての目的について、ユーザーをリードしています。また、Aptanaのをインストールするための構文について説明します。 Aptanaのモジュールのhelpコマンドは、以下のように示されている。

.. code-block:: bash

		ptconfigure Aptana help

helpコマンドを宣言するための構文は、ケースという追加の利点であると小文字は区別されません。次のスクリーンショットは、Aptanaの下に、helpコマンドについてあなたを視覚化。

.. code-block:: bash

 kevell@corp:/# ptconfigure Aptana help

 If you use this command, you can install the Aptana, open-source Web development IDE.

 Aptana, aptana

	- install
        Installs Aptana. 
        example: ptconfigure aptana install

      
	  - uninstall
        Uninstalls Aptana.
        example: ptconfigure aptana uninstall

 ------------------------------
 End Help
 ******************************


インストール
-----------------

ユーザーがマシンにAptanaのをインストールするために使用するコマンドを以下に示します。

.. code-block:: bash

	ptconfigure Aptana install

スクリーンショット形式で示すように上記のコマンドを入力した後、次の処理が発生します。


.. cssclass:: table-bordered

 +---------------------------+---------------------------------------------+----------------+------------------------------------------+
 | パラメータ                | 代替パラメータ                              | オプション     | 注釈                                     |
 +===========================+=============================================+================+==========================================+
 |Install Aptana?(Y/N)       | 代わりに、Aptanaのを使用するユーザーは、    | Y              | それはptconfigure下にAptanaのモジュ      |
 |                           | aptanaのを使用することができます            |                | ールをインストールします                 |
 +---------------------------+---------------------------------------------+----------------+------------------------------------------+
 |Install Aptana?(Y/N)       | 代わりに、Aptanaのを使用するユーザーは、    | N              | ユーザーは、Nとして、彼らが入力できるイ  |
 |                           | aptanaのを使用することができます            |                | ンストールを終了したい場合は|            |
 +---------------------------+---------------------------------------------+----------------+------------------------------------------+


.. code-block:: bash


 kevell@corp:/# ptconfigure aptana install
 Install Aptana? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Aptana !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-88784131186.sh
 chmod 755 /tmp/ptconfigure-temp-script-88784131186.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-88784131186.sh Permissions
 Executing /tmp/ptconfigure-temp-script-88784131186.sh
 --2015-04-01 11:14:14--  https://github.com/aptana/studio3/releases/download/v3.6.1/Aptana_Studio_3_Setup_Linux_x86_64_3.6.1.zip
 Resolving github.com (github.com)... 192.30.252.129
 Connecting to github.com (github.com)|192.30.252.129|:443... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: https://s3.amazonaws.com/github-cloud/releases/339002/397875ee-6c0b-11e4-8d77-2f8197e58a3a.zip?response-content-  
 disposition=attachment%3B%20filename%3DAptana_Studio_3_Setup_Linux_x86_64_3.6.1.zip&response-content-type=application/octet- 
 stream&AWSAccessKeyId=AKIAISTNZFOVBIJMK3TQ&Expires=1427867115&Signature=CMxDcsoZ2rhtmlb5JZkd2KE6QK0%3D [following]
 --2015-04-01 11:14:15--  https://s3.amazonaws.com/github-cloud/releases/339002/397875ee-6c0b-11e4-8d77-2f8197e58a3a.zip?response-content- 
 disposition=attachment%3B%20filename%3DAptana_Studio_3_Setup_Linux_x86_64_3.6.1.zip&response-content-type=application/octet- 
 stream&AWSAccessKeyId=AKIAISTNZFOVBIJMK3TQ&Expires=1427867115&Signature=CMxDcsoZ2rhtmlb5JZkd2KE6QK0%3D
 Resolving s3.amazonaws.com (s3.amazonaws.com)... 54.231.13.80
 Connecting to s3.amazonaws.com (s3.amazonaws.com)|54.231.13.80|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 123680508 (118M) [application/octet-stream]
 Saving to: â€˜Aptana_Studio_3_Setup_Linux_x86_64_3.6.1.zip.1â€™ 
 inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/ListAllMyBucketsResponse$ListAllMyBucketsHandler.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/CallingFormat.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/QueryStringAuthGenerator.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/Utils.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/CallingFormat$PathCallingFormat.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/Response.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/ListAllMyBucketsResponse.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/AWSAuthConnection.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/S3Object.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/ListEntry.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/Bucket.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/CallingFormat$VanityCallingFormat.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/LocationResponse$LocationResponseHandler.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/CallingFormat$SubdomainCallingFormat.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/GetResponse.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/CommonPrefixEntry.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/ListBucketResponse$ListBucketHandler.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/LocationResponse.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/s3/ListBucketResponse.class  
   creating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/thirdparty/
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/thirdparty/Base64$InputStream.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/thirdparty/Base64$OutputStream.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.amazon.s3_3.0.0.1385945603/com/amazon/thirdparty/Base64.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.editor.js_3.0.3.1413588685.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.ibm.icu_50.1.1.v201304230130.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.equinox.p2.publisher_1.3.0.v20140129-1405.jar  
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/LICENSE.txt  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/shared_ui.jar  
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/META-INF/
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/META-INF/MANIFEST.MF  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/META-INF/eclipse.inf  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/META-INF/APPCELER.RSA  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/META-INF/APPCELER.SF  
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/imp_rel_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/template.pdn  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/imp_dec.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/method_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/create_python_module.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/action.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/create_method_obj.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/create_class_obj.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/__imp_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/class_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/old_imp_rel_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/create_attrpub_obj.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/attrpub_obj.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/imp_obj.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/xml_tag.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/new/imp_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_l_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jython_run.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/forward_nav.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/toggle_tabs.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/error_decoration.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/expand.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/terminate_all.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/home_nav.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/static_co.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_run.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_perspective.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/relaunch_errors.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/relaunch_background_disabled.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/custom_init.png  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/relaunch1.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/decoration_static_obj.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/field_protected_obj.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/relaunch.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/package_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/annotation_obj.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/tabs_active.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_nonexist_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/history_list.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/folder.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/warning_decoration.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/refresh_nav.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/failures.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/parameters_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/fields_co.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/collapseall.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_logo.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/backward_nav.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/pylint.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/environment_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/field_private_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/showerr_tsk.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/magic_co.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/search_docs.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_comment_black.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_coverage.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/correction_move.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_lsrc_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_nature.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/gotten_from.txt  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/tabs_inactive.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/remove_nature.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/field_public_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_file.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/file.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/private_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/close.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_src_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/decoration_class_obj.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/builtin_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/mainfunction.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_desc_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/template.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_refactor.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/protected_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/add_correction.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/cython_file.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/copy.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_module.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/sample.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_16x16.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/search.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/sync_ed.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/cython.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/relaunch_background_enabled.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/build_var_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/project_source_folder.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/alphab_sort_co.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_unit.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/terminate.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/warning.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/save.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/packagefolder_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/remove.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/python_comment.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/error_small.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/library_obj.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/pydev_package_explorer.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/cpyqual_menu.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/filter.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/workset.gif  
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/custom_python_file.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/pythonNature.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/icons/jar_remove_l_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.shared_ui_3.0.0.1389225860/plugin.xml  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.compare.core_3.5.300.v20130514-1224.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.editor.common.override_1.0.0.1351531287.jar  
   creating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/LICENSE.TXT  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/debug.jar  
   creating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/META-INF/
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/META-INF/MANIFEST.MF  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/META-INF/eclipse.inf  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/META-INF/APPCELER.RSA  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/META-INF/APPCELER.SF  
   creating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/icons/
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/icons/python.gif  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/icons/term_debug_server.gif  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/icons/start_debug_server.gif  
  inflating: /opt/Aptana_Studio_3/plugins/com.python.pydev.debug_3.0.0.1388187472/plugin.xml  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.core.contenttype_3.4.200.v20130326-1255.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.equinox.preferences_3.5.100.v20130422-1538.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.workbench_3.0.0.1407781207.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.radrails.rails.core_3.0.2.1345651386.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.w3c.dom.svg_1.1.0.v201011041433.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.apache.lucene.analysis_3.5.0.v20120725-1805.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.equinox.p2.updatechecker_1.1.200.v20130327-2119.jar  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/license.html  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/macosx/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/macosx/redtty  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/linux/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/linux/x86_64/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/linux/x86_64/redtty  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/linux/x86/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/linux/x86/redtty  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/win32/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/win32/redttyw.exe  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/os/win32/wintty.dll  
 extracting: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/.aptanarc  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/schema/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/schema/processConfigurations.exsd  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/schema/terminalHyperlinkDetectors.exsd  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/scripting/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/scripting/ruble/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/scripting/ruble/terminal.rb  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/OSGI-INF/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/OSGI-INF/l10n/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/OSGI-INF/l10n/bundle.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/contexts.xml  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/META-INF/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/META-INF/p2.inf  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/META-INF/MANIFEST.MF  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/META-INF/APPCELER.RSA  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/META-INF/APPCELER.SF  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/icons/
 extracting: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/icons/terminal.png  
 extracting: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/icons/terminal_add.png  
 extracting: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/icons/terminal_small_add.png  
 extracting: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/icons/terminal_small.png  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/IProcessConfiguration.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/Utils.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/messages.properties  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalElementFactory.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$8.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditorInput.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$4.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$7.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$5.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$2.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/ShowTerminalEditorAction.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$6.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$3.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/TerminalEditor$1$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/editor/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/TerminalPlugin.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/hyperlink/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/hyperlink/IHyperlinkDetector.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/ProcessConfigurations.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/VT100TerminalControl 
  $3.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/TextCanvas.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/ThemedStyleMap.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/
  VT100TerminalControl.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/
 ThemedTextLineRenderer.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/VT100TerminalControl
 $1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/emulator/VT100TerminalControl
 $2.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/configurations/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/configurations/
 NixBashConfiguration.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/configurations/
 WindowsMingwConfiguration.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/configurations/
 AbstractProcessConfiguration.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/IProcessListener.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/ProcessLauncher$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/TerminalCloseHelper.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/hyperlink/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/hyperlink/
 URLHyperlinkDetector.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/hyperlink/HyperlinkManager.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/StreamsProxyOutputStream.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/handlers/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/handlers/
 OpenTerminalHandler.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/handlers/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/handlers/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/internal/ProcessLauncher.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/widget/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/widget/TerminalComposite$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/widget/TerminalComposite$3.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/widget/TerminalComposite.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/widget/TerminalComposite$2.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/preferences/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/preferences/PreferenceInitializer.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/preferences/TerminalPreferencePage.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/preferences/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/preferences/IPreferenceConstants.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/preferences/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/Messages.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$7.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$1$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$4.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$10.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$8.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$2.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$6.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$5.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$3.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/views/TerminalView$9.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/
 LocalTerminalOutputListener.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/IOutputFilter.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/LocalTerminalConnector$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/com/aptana/terminal/connector/LocalTerminalConnector.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.terminal_3.0.0.1407781207/plugin.xml  
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/LICENSE.txt  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/plugin.properties  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/refactoring.jar  
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/META-INF/
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/META-INF/MANIFEST.MF  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/META-INF/eclipse.inf  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/META-INF/APPCELER.RSA  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/META-INF/APPCELER.SF  
   creating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/icons/
 extracting: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/icons/logo.png  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/icons/methpub_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/icons/logo.ufo  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/icons/class_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.python.pydev.refactoring_3.0.0.1389225860/icons/attrpub_obj.gif  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.jetty.servlet_8.1.14.v20131031.jar  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/license.html  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/schema/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/schema/parser.exsd  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/.options  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/libs/
 extracting: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/libs/jaxen-1.1.2-src.zip  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/libs/jaxen-1.1.2.jar  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/OSGI-INF/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/OSGI-INF/l10n/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/OSGI-INF/l10n/bundle.properties  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/META-INF/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/META-INF/MANIFEST.MF  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/META-INF/eclipse.inf  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/META-INF/APPCELER.RSA  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/META-INF/APPCELER.SF  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/IPropertyContainer.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaHandler$PropertyName.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaPrimitive.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/ISchemaContext.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaProperty.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaArray.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaBoolean.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaObject.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaNumber.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaHandler$TypeName.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaArray$ArrayState.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/Schema$SchemaState.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaString.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaObject$ObjectState.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaNull.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/IState.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/IContextHandler.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaHandler.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaBuilder.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaReader.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaTypeGroup.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaEventType.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/SchemaContext.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/json/Schema.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/internal/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/internal/parsing/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/internal/parsing/ParserPool.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/ILexeme.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/IRange.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/Lexeme.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/ITypePredicate.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/Range.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/lexer/ILexemeModel.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/IParseState.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParserPoolFactory$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParseStateCacheKey.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParseState.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParsingEngine$IParserPoolProvider.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/IParser.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/IParseStateCacheKey.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParserPoolFactory.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParseResult.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParsingEngine$CacheValue.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParsingPlugin.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/WorkingParseResult.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/IRecoveryStrategy.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/util/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/util/ParseUtil$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/util/ParseUtil.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/util/ParseUtil$QueueEntry.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/util/ParseUtil$IASTVisitor.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/util/ParseUtil$2.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeNavigator.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeAttributeIterator.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeXPath.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeNavigator$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeIterator.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeNavigator$3.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/xpath/ParseNodeNavigator$2.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/InsertionRecoveryStrategy.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/AbstractParser.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParseStateCacheKeyWithComments.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/IParserPool.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ParsingEngine.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ParseNode$NameNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/TextNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ParseRootNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/IParseError.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/IParseNodeAttribute.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ParseNodeAttribute.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ParseError.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/IParseRootNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/IParseNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/TextNode$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ILanguageNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/INameNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ParseNode$1.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/ast/ParseNode.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/InsertionRecoveryStrategy
 $CandidateToken.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/parsing/IDebugScopes.class  
   creating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/AttributeUsage.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/messages.properties  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/SchemaElement.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/ValidatingReader.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/IValidatingReaderLogger.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/InvalidTransitionException.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/ISchemaElement.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/SchemaInitializationException.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/SchemaBuilder.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/SchemaFreeformElement.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/SchemaBuilder$Element.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/Messages.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/com/aptana/sax/Schema.class  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.parsing_3.0.0.1380642747/plugin.xml  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.equinox.p2.operations_2.3.0.v20130711-1809.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.scripting_3.1.0.1397674205.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.ui.externaltools_3.2.200.v20130508-2007.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.core_3.3.0.1409799816.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.editor.findbar_3.0.0.1408146668.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.apache.batik.util.gui_1.6.0.v201011041432.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.editor.diff_3.0.0.1365788962.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.php.debug.epl_3.3.0.1407783092.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.ui.navigator_3.5.300.v20130517-0139.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.editor.html.formatter_3.0.3.1407781207.jar  
  inflating: /opt/Aptana_Studio_3/plugins/com.aptana.jira.ui_1.0.0.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.emf.ecore.xmi_2.9.1.v20131212-0545.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.equinox.p2.metadata.repository_1.2.100.v20130327-2119.jar  
  inflating: /opt/Aptana_Studio_3/plugins/org.eclipse.equinox.app_1.3.100.v20130327-1442.jar  
  inflating: /opt/Aptana_Studio_3/epl-v10.html  
  inflating: /opt/Aptana_Studio_3/version.txt  
  inflating: /opt/Aptana_Studio_3/artifacts.xml  
 extracting: /opt/Aptana_Studio_3/AptanaStudio3.sh  
   creating: /opt/Aptana_Studio_3/configuration/
   creating: /opt/Aptana_Studio_3/configuration/org.eclipse.update/
  inflating: /opt/Aptana_Studio_3/configuration/org.eclipse.update/platform.xml  
   creating: /opt/Aptana_Studio_3/configuration/org.eclipse.equinox.simpleconfigurator/
  inflating: /opt/Aptana_Studio_3/configuration/org.eclipse.equinox.simpleconfigurator/bundles.info  
   creating: /opt/Aptana_Studio_3/configuration/.settings/
  inflating: /opt/Aptana_Studio_3/configuration/.settings/org.eclipse.equinox.p2.metadata.repository.prefs  
  inflating: /opt/Aptana_Studio_3/configuration/.settings/org.eclipse.equinox.p2.artifact.repository.prefs  
  inflating: /opt/Aptana_Studio_3/configuration/config.ini  
   creating: /opt/Aptana_Studio_3/p2/
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/1413827594660.profile.gz  
 extracting: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/1413827559587.profile.gz  
 extracting: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/1413827559061.profile.gz  
 extracting: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.lock  
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.data/
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.data/.settings/
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.data/.settings/
 org.eclipse.equinox.p2.metadata.repository.prefs  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.data/.settings/
 org.eclipse.equinox.p2.artifact.repository.prefs  
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.data/ 
 org.eclipse.equinox.internal.p2.touchpoint.eclipse.actions/
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/.data/
 org.eclipse.equinox.internal.p2.touchpoint.eclipse.actions/jvmargs  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/profileRegistry/profile.profile/1413827596983.profile.gz  
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/.settings/
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/.settings/org.eclipse.equinox.p2.metadata.repository.prefs  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.engine/.settings/org.eclipse.equinox.p2.artifact.repository.prefs  
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/
   creating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/
 com.aptana.feature.rcp_root.gtk.linux.x86_64_3.6.0.201410201044-7q7fFA2FEB7f0Xksz0bSy9-Gg8I4  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/
 com.aptana.feature.rcp_root_3.6.0.201410201044-7q7fFA2FEB7f0Xksz0bSy9-Gg8I4  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/org.eclipse.rcp_root_4.3.2.v20140221-1700  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/
 com.aptana.rcp.product.root.feature_root_3.6.1.201410201044-20102014104527  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/org.eclipse.platform_root_4.3.2.v20140221-1852  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/binary/
 com.aptana.rcp.product_root.gtk.linux.x86_64_3.6.1.201410201044-20102014104527  
  inflating: /opt/Aptana_Studio_3/p2/org.eclipse.equinox.p2.core/cache/artifacts.xml  
 Temp File /tmp/ptconfigure-temp-script-86059641805.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Aptana: Success
 ------------------------------
 Installer Finished
 ******************************


アンインストール
---------------------------

ユーザーがマシンにAptanaのをアンインストールするために使用されるコマンドを以下に示します。

.. code-block:: bash

	ptconfigure Aptana uninstall

スクリーンショット形式で示すように上記のコマンドを入力した後、次の処理が発生します。


.. cssclass:: table-bordered

 +---------------------------+----------------------------------------------+---------------+-------------------------------------------+
 | パラメータ                | 代替パラメータ                               | オプション    | 注釈                                      |
 +===========================+==============================================+===============+===========================================+
 |UnInstall Aptana?(Y/N)     | 代わりに、 Aptanaの使用 ユーザーは、         | Y             | それはptconfigure下Aptanaのモジュ         |
 |			     | Aptanaのを使用することができます             |               | ールをアンインストールします              |
 +---------------------------+----------------------------------------------+---------------+-------------------------------------------+
 |UnInstall Aptana?(Y/N)     | 代わりに、 Aptanaの使用 ユーザーは、         | N             | ユーザーが終了している アンインストール   |
 |			     | Aptanaのを使用することができます|            |               |                                           |
 +---------------------------+----------------------------------------------+---------------+-------------------------------------------+
 
.. code-block:: bash


 kevell@corp:/# ptconfigure aptana uninstall
 Uninstall Aptana? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Aptana !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-57031832585.sh
 chmod 755 /tmp/ptconfigure-temp-script-57031832585.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-57031832585.sh Permissions
 Executing /tmp/ptconfigure-temp-script-57031832585.sh
 Temp File /tmp/ptconfigure-temp-script-57031832585.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 Aptana: Success
 ------------------------------
 Installer Finished
 ******************************






プラットフォームと言語サポート
-----------------------------------

Aptana Studio 3は、PHPアプリケーション開発のための次のサポートを提供します。

* シンタックスカラーリングは、環境設定で選択したテーマに応じた。
* コードアシスト。
* 構文エラーの注釈。
* オートインデントとコードフォーマット。
* ハイパーリンク要素の上にホバリングし、Ctrlキーを押して、クラス、関数や変数に。
* たPHPDocのポップアップをドキュメントを添付したアイテムの上にマウスを移動。
* 読み、特定のPHPの要素をクリックしたときに出現マーカーを書き込む。


Aptanaバージョン1.5は、PHPのアドオンプラグイン経由でPHPアプリケーションを開発するためのサポートを提供しました。これが含まれる：


* 内蔵のPHPサーバーのAptana内プレビューに、

* 完全なコードアシスト、コードがアウトラインと、コードが書式設定、

* 統合されたPHPデバッガ、

* Smartyの年に建てられ、

* 型階層ビューは、

* 宣言に移動し、

* 統合されたPHPのマニュアル


メリット
----------

* これは、インストールおよびアンのAptanaをインストールするために使用されている
* 非大文字と小文字の区別
* 完全なコードアシスト、コードがアウトライン、コードは書式設定
* それはサポートしていますUbuntuとcentos.
* 統合されたPHPデバッガ

