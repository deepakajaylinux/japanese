===== 
JAVA
=====

あらすじ
------------

このモジュールは、オラクルの java JDK 1.7 のバージョンをインストールするのに役立ちます。それはまた構成の java、javac、新しい oracle バージョンと一緒に javaws を容易にします。

ヘルプ コマンド
---------------------

Help コマンドと同様、目的に関するユーザー ガイドとして java モジュールに含まれているオプションについて。ヘルプ コマンドは java モジュールの代替パラメーターが一覧表示されます。また、Java JDK 1.7 をインストールするための構文について説明します。Java モジュールのヘルプ コマンドが表示されます以下の通りです。

.. code-block:: bash

		ptconfigure Java help

ヘルプ コマンドを宣言する構文は大文字小文字を区別する加えられた利点であります。次のスクリーン ショットは、java のモジュールの下に、help コマンドについて視覚化します。


.. code-block:: bash

 kevell@corp:/# ptconfigure java help
 ******************************


 This command allows you to install Java JDK 1.7 .

 Java, java, java17

        - install
        Installs a version of Oracle Java JDK 1.7. It will also configure java,
        javac and javaws to be provided by the new Oracle version.
        example: ptconfigure java17 install

 ------------------------------
 End Help
 ******************************


インストール
----------------

ジャワ JDK 1.7 の oracle バージョンをインストールするユーザーのコンピューターには、単に以下のようにコマンドを使用して実行できます。


.. code-block:: bash
	
		ptconfigure Java install

上記のコマンドを入力した後、次のプロセスが発生します表形式で表示されます。

.. cssclass:: table-bordered

 +--------------------------+--------------------------------------------+--------------+-------------------------------------------+
 | パラメータ               | 代替パラメータ                             | オプション   | 注釈                                      |
 +==========================+============================================+==============+===========================================+
 |Install The Oracle Java   | の代わりに Oracle Java JDK 1.7,            | Y(Yes)       | ユーザーは、Yと入力することができ、       |
 |JDK 1.7? (Y/N)            | 以下の選択肢を使用することもできる:        |              | インストールプロセスを続行したい場合      |
 |                          | Java, java, java17                         |              |                                           |
 +--------------------------+--------------------------------------------+--------------+-------------------------------------------+
 |Install The Oracle Java   | の代わりに Oracle Java JDK 1.7,            | N(No)        | ユーザーは、Nと入力することができ、       |
 |JDK 1.7? (Y/N)            | 以下の選択肢を使用することもできる:        |              | インストールプロセスを終了したい場合は    |
 |                          | Java, java, java17|                        |              |                                           |
 +--------------------------+--------------------------------------------+--------------+-------------------------------------------+


.. code-block:: bash

 kevell@corp:/# ptconfigure java17 install
 Install The Oracle Java JDK 1.7? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):
 /opt
 Creating /tmp/ptconfigure-temp-script-96883431452.sh
 chmod 755 /tmp/ptconfigure-temp-script-96883431452.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-96883431452.sh Permissions
 Executing /tmp/ptconfigure-temp-script-96883431452.sh
 --2015-04-09 16:27:08--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.168, 131.103.20.167
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.168|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 141966331 (135M) [application/zip]
 Saving to: Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢

 100%[====================================================================================================>] 14,19,66,331  110KB/s   in 12m 36s

 2015-04-09 16:39:46 (183 KB/s) - Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢ saved [141966331/141966331]

 Archive:  /tmp/oraclejdk.zip
 6c383e2868bd47e56385921e11ec155ac54faa13
   creating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/
  inflating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz  
 update-alternatives: using /opt/bin/java to provide /usr/bin/java (java) in auto mode
 update-alternatives: using /opt/bin/javac to provide /usr/bin/javac (javac) in auto mode 
 update-alternatives: using /opt/bin/javaws to provide /usr/bin/javaws (javaws) in auto mode
 Temp File /tmp/ptconfigure-temp-script-96883431452.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Java: Success
 ------------------------------
 Installer Finished
 ******************************



利点
------------

* ヘルプおよびインストール操作で使用されるパラメーター大文字小文字が区別されません中に他の人に比べて利点であります。
* それは両方の Ubuntu と同様、裕福なセントの OS として。
* Javaws、java、javac の構成は、新しい oracle バージョンの助けを借りてことができます。


