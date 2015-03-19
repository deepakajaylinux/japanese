======================
Host Editor
======================

概要
------------------

このモジュールは、ptdeploy下のApacheバーチャルホストエディタを処理するためにサポートしています。それは2つの方法で機能することができる。彼らは、追加および削除されます。バーチャルホストエディタは風をのapacheに、仮想ホストを追加するために書かれたPHPのツールです。バーチャルホストエディタは、追加、編集、またはユーザのウェブサーバ上の仮想ホスト情報を削除することを可能にします。これは、UbuntuとセントのOSで動作すると便利です。のは、Apacheバーチャルホストエディタで機能する方法を見てみましょう
ptdeploy。


Helpコマンド
-----------------------

このhelpコマンドは、仮想ホストを作成するためのユーザーをガイドします。これはまた、仮想ホストを追加する仮想ホストを削除し、仮想ホストを有効にして、仮想ホストを無効にする表示されます。

Apachevhosteditorためのhelpコマンドを以下に示します。

.. code-block:: bash

	ptdeploy Apachevhosteditor help

後、上記のコマンドを入力し、それが仮想ホストエディタを追加するために機能して開始します。これは、スクリーンショットで関数を教理。

.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheVHostEditor help
 ******************************


  This command is part of Default Modules and handles Apache VHosts Functions.

  ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted

          - add
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - add-balancer
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com

          - list
          List current Virtual Hosts
          example: ptdeploy vhe list

          - enable
          enable a Server Block
          example: ptdeploy vhe enable

          - disable
          disable a Server Block
          example: ptdeploy vhe disable

 ------------------------------
 End Help
 ******************************

代替パラメータ
-----------------------------------

次の宣言で定義することができる代替パラメータは次のとおりです。

ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted.

加える
-------

これは仮想ホストを作成するためのユーザーを容易にします。バーチャルホストを追加する際には、VHE-ドキュメントルート、VHE-FILE-EXT、VHE-apacheのコマンド、VHE-IPポートを尋ね、VHEホストDIR、VHE-テンプレート缶VHE-デフォルト·テンプレート名。ユーザは、自分の希望に応じて入力することができます。

.. code-block:: bash

	sudo ptdeploy vhe add

上記のコマンドとして入力した後、ユーザーは、以下のプロセスを埋めることができます。

.. cssclass:: table-bordered

 +-----------------------+------------------------+----------------------------------+----------------------------------------------------+
 | パラメータ            | パラメータ             | オプション                       | 注釈                                               |
 +=======================+========================+==================================+====================================================+
 |ptdeploy vhe add       | Yes                    | これは、ドキュメントルート       | ptdeploy下に指定されたドキュメント                 | 
 |(Default)              |                        | をユーザーに尋ねることができます | ルートに追加された仮想ホスト                       |
 +-----------------------+------------------------+----------------------------------+----------------------------------------------------+
 |What’s the server name | -                      | これは、サーバー名の入力を       | ptdeployの下に追加のサーバー名                     |
 |                       |                        | 求めることができます             |                                                    |
 +-----------------------+------------------------+----------------------------------+----------------------------------------------------+
 |What IP:Port (default) | 127.0.0.1:80           | これは、IPポートをユーザーに求   | ときにデフォルト値を入力として、ユーザー入力が     |
 |                       |                        | めることができます               | IPのために追加：ポート                             |
 +-----------------------+------------------------+----------------------------------+----------------------------------------------------+
 |What file extension    | None                   | 缶これは、拡張機能をユーザーに   | ユーザーは、ファイル拡張子として入力を提供します   |
 |should be used?        |                        | 要求する                         |                                                    |
 |(Default)              |                        |                                  |                                                    |
 +-----------------------+------------------------+----------------------------------+----------------------------------------------------+
 |ptdeploy vhe add       | No                     | できるそれはユーザーに入力を     | これは、プロセスを終了することができ               |
 |                       |                        | 要求します。|                    |                                                    |
 +-----------------------+------------------------+----------------------------------+----------------------------------------------------+


最後に、このシステムはバーチャルホストのtemplatesディレクトリを要求することができます。テンプレートで利用可能な5つのオプションがあります。次のように彼らは。

0 for doc root-no-suffix

1 for doc –src-suffix used for document screen suffix

2 for doc –web-suffix used for document web suffix

3 for doc –www-suffix used for world wide web suffix

4 for docroot-suffix used for document root suffix

ユーザーは、自分のニーズに応じて値を選択したい。その後、システムは、IPアドレスとrootユーザーなどが正しいか間違っている、バーチャルホスト名を尋ねることができます。ユーザーがイエスと言うなら、それはバーチャルホストのディレクトリが表示され、このバーチャルホストを有効にする？


ユーザーの答えははい、それは他のバーチャルホストを有効にすることができ、それは終了することができます。

.. code-block:: bash

 kevells@corp:/# ptdeploy vhe add
 Do you want to add a VHost? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 root
 What URL do you want to add as server name?
 www.vh.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What File Extension should be used? Enter nothing for None (probably .conf on this system)

 What is your VHost Template directory? Enter nothing for default templates

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-suffix
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 0
 Please check VHost: NameVirtualHost 127.0.0.1:80
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.vh.com
	DocumentRoot root
	<Directory root>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Order allow,deny
		allow from all
	</Directory>
 </VirtualHost>

 Is this Okay? (Y/N) 

 ******************************


 Apache VHost Editor Finished
 ******************************

削除する
--------------

仮想ホスト（複数可）を削除するためのターミナルコマンドはRMです。このコマンドの一般的なフォーマットはRMです。あなたはそれのための正しいパスを指定した場合、RMは仮想ホストを削除し、そうでない場合は、エラー·メッセージが表示され、次のホストに移動します。時には、それは確認をお願いしますその場合には、仮想ホストの書き込み権限がない可能性があります。あなたがそれを削除したい場合は、yesと入力。

削除された名前は、仮想ホストへの最後のリンクで、かつ、どのプロセスが持っていない場合

仮想ホストのオープンは、仮想ホストが削除され、それが使用していたスペースは、再使用のために使用されている。

名前は、仮想ホストへの最後のリンクであったが、すべてのプロセスがまだ持っている場合

仮想ホストのオープンは、仮想ホストはそれを参照する最後の仮想ホスト記述子がクローズされるまでは存在し続ける。

名前がシンボリックリンクを参照する場合、リンクが削除されます。次のコマンドは、仮想ホストを削除するために使用。

.. code-block:: bash
   
		sudo ptdeploy vhe rm –yes –guess –vhe-deletion-vhost=www.kevell.com

以下のスクリーンショットは、その機能を説明することができます。

.. code-block:: bash

 - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm
 Do you want to delete VHost/s? (Y/N) 
 y
 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf

 0
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 yes
 Site 000-default disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite 000-default.conf done
 VHost 000-default.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************

リスト
--------

仮想ホスト（デフォルトではカレントディレクトリ）についての情報を一覧表示します。アルファベット順にソートエントリ。必須の引数は、あまりにも長いオプションとしてだけでなく、短いオプションがあります。リストには、リスト名と提供し、データを整理しますまた、基礎となるビューの両方を指定するURLを使用して起動。次のコマンドは、仮想ホストをリストするために使用される。

.. code-block:: bash
   
        ptdeploy vhe list

リストかどうかをさまざまなビューを使用することができ、またはそのためのデータを整理するために特別に設計されたビューから精巧なページを生成するように調整することがあるので注意してください。設計ドキュメントのリスト欄の下に格納リスト。これは、スクリーンショットで可視化することができる。

.. code-block:: bash

 - list
          List current Virtual Hosts
          example: ptdeploy vhe list


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe list
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 You have a sites available dir, so also listing available sites.
 Current Installed VHosts:
 --- Enabled Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf
 --- All Available Virtual Hosts: ---
 (2) 000-default.conf
 (3) default-ssl.conf
 ******************************


 1Apache VHost Editor Finished
 ******************************

有効にする
-------------


セキュアブートは、ブートプロセス中にロードするから悪意のあるソフトウェアや無許可のメディアを防ぐように設計機能です。この有効オプションは、サーバのブロックを可能にした。仮想ホストで使用する場合は、次のコマンドを入力した、

.. code-block:: bash
   
        ptdeploy vhe enable

このオプションはデフォルトで有効になっています。このオプションは、仮想ホストサーバがイネーブル可能にする。

アシストモジュールは、人、プロセス、テクノロジー間の相互依存性の理解を通じて高性能環境にサービスを提供するために必要な有効な機能の多くを開発しています。次のスクリーンショットは、同じことを説明しています。

.. code-block:: bash

 - enable
          enable a Server Block
          example: ptdeploy vhe enable



.. code-block:: bash

 kevell@corp:/# ptdeploy vhe enable
 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf
 
 0
 ERROR: Site default-ssl.conf does not exist!
 a2ensite default-ssl.conf.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************

無効にする
-------------

この無効化は、サーバーを無効にするために使用。非アクティブまたはアイドル仮想ホストエディタ接続は、通常、一定時間が経過すると、サーバーによって切断されます。以下のコマンドは、仮想ホストエディタを無効にするために使用されている。

.. code-block:: bash
   
        ptdeploy vhe disable

このコマンドを入力した後、サーバーを無効にするには、ユーザーに確認することができます。それは許可されません。つまり、ユーザの入力としてはい、それがサーバーを無効にした場合はすべてのボディは、そのサーバで動作する。

次のスクリーンショットは明らかにそれを視覚化する。

.. code-block:: bash


 - disable

          disable a Server Block
          example: ptdeploy vhe disable


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe disable
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf

 0
 Site default-ssl already disabled
 a2dissite default-ssl.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************


メリット
---------------

* マルチユーザーが一度にアクセスすることができます。
* ユーザーは、仮想ホストを追加または削除することができます。
* 仮想ホストエディタは、ユーザーの希望に応じて仮想ホストを有効または無効にすることができます。
* 非大文字と小文字の区別。
