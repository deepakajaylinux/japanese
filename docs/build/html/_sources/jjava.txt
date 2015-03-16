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
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):

 Creating /tmp/ptconfigure-temp-script-37090112192.sh
 chmod 755 /tmp/ptconfigure-temp-script-37090112192.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-37090112192.sh Permissions
 Executing /tmp/ptconfigure-temp-script-37090112192.sh
 --2015-03-16 15:52:21--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.167, 131.103.20.168
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.167|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [application/zip]
 Saving to: ‘6c383e2868bd.zip’

    [          <=>                                                                                          ] 2,06,54,011 2.98KB/s   in 12m 14s

 2015-03-16 16:04:59 (27.5 KB/s) - ‘6c383e2868bd.zip’ saved [20654011]

 /tmp/oraclejdk: Scheme missing.
 FINISHED --2015-03-16 16:04:59--
 Total wall clock time: 12m 39s
 Downloaded: 1 files, 20M in 12m 14s (27.5 KB/s)
  End-of-central-directory signature not found.  Either this file is not
  a zipfile, or it constitutes one disk of a multi-part archive.  In the
  latter case the central directory and zipfile comment will be found on
  the last disk(s) of this archive.
 unzip:  cannot find zipfile directory in one of /tmp/oraclejdk.zip or
        /tmp/oraclejdk.zip.zip, and cannot find /tmp/oraclejdk.zip.ZIP, period.
 /tmp/ptconfigure-temp-script-37090112192.sh: 6: cd: can't cd to /tmp/oraclejdk
 mv: cannot stat ‘/tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz’: No such file or directory
 tar: jdk-7u60-linux-x64.tar.gz: Cannot open: No such file or directory
 tar: Error is not recoverable: exiting now
 mkdir: missing operand
 Try 'mkdir --help' for more information.
 cp: missing destination file operand after ‘/tmp/oraclejdk/jdk1.7.0_60/*’
 Try 'cp --help' for more information.
 chmod: missing operand after ‘a+x’
 Try 'chmod --help' for more information.
 update-alternatives: error: alternative path /bin/java doesn't exist
 update-alternatives: error: alternative path /bin/javac doesn't exist
 update-alternatives: error: alternative path /bin/javaws doesn't exist
 update-alternatives: error: alternative /bin/java for java not registered; not setting
 update-alternatives: error: alternative /bin/javac for javac not registered; not setting
 update-alternatives: error: alternative /bin/javaws for javaws not registered; not setting
 Archive:  /tmp/oraclejdk.zip
 Temp File /tmp/ptconfigure-temp-script-37090112192.sh Removed
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


