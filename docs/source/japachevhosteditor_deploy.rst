===========================
ApacheVHostEditor
===========================

概要
------------------

Apacheバーチャルホストは単一のIPアドレスのオフ複数のドメインを実行するために使用されている。これは、Apacheのバーチャルホスト機能を処理する必要がある人に特に便利です。サイトでは、ユーザーがサイトにアクセスしたとに応じて、訪問者に異なる情報を表示する。仮想プライベートサーバに追加することができる仮想ホストの数に制限はありません（VPS）。このはUbuntuとCentOSのに適していることができます。

Helpコマンド
-----------------------

helpコマンドは、とだけでなく、Apacheのバーチャルホストエディタモジュールに含まれているオプションについての目的について、ユーザーをリードしています。 apacheのバーチャルホストエディタの代わりのパラメータからhelpコマンドリスト
ptdeployモジュールの下に。また、ユーザーのupdationをインストールするための構文について説明します。 Apacheのバーチャルホストのエディタのhelpコマンドを以下に示します。

.. code-block:: bash

	ptdeploy Apache virtualhost editor help

次のスクリーンショットは、ApacheのVirtualHostエディタの完全な努力を示している。

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
----------

このコマンドは、仮想ホストを作成するために使用される。オーバーライドが可能です。次のコマンドは、仮想ホストエディタを作成するために採用することができる。

.. code-block:: bash

	sudo ptdeploy vhe add

上記のコマンドを入力した後、以下求めることができる、

VHEのドキュメントルート、VHEのファイル拡張子、VHEのApacheのコマンド、VHE IPポート、VHEバーチャルホストディレクトリ、VHEテンプレート、VHEデフォルトのテンプレート名。

ユーザは、入力するすべての詳細を他の方法で、コマンドライン自体に入力一つずつ有する。以下のスクリーンショットは、それについて説明します

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add 
 
 Do you want to add a VHost? (Y/N) 
 y 
 What's the document root? Enter nothing for /home/karunakaran 

 What URL do you want to add as server name? 
 kumar 
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
	ServerName kumar 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Is this Okay? (Y/N) 
 y 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Enabling site kumar. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite kumar.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.murali.com --vhe-file-ext=".conf" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*" 

 *template data* 

 Assuming Okay due to yes parameter 
 Enabling site www.murali.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.murali.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --guess --vhe-url=www.kkkkkkkkk.com 

 What is your VHost Template directory? Enter nothing for default templates 

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: --- 
 (0) docroot-no-suffix 
 (1) docroot-src-suffix 
 (2) docroot-web-suffix 
 (3) docroot-www-suffix 
 (4) docroot-docroot-suffix 
 
 0 
 NameVirtualHost 127.0.0.1:80 
 <VirtualHost 127.0.0.1:80> 
 	ServerAdmin webmaster@localhost 
	ServerName www.kkkkkkkkk.com 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Assuming Okay due to yes parameter 
 Enabling site www.kkkkkkkkk.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.kkkkkkkkk.com done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************






追加 - バランサ
---------------------

このコマンドは、仮想ホストを作成するために使用される。オーバーライドが可能です。入力を入力するには二つの方法があります。簡単なようにして、ユーザは、VHE ADDを与えることができます。コマンドホストパス名とともに第二の方法を挙げることができる。次のコマンドは、仮想ホストエディタを作成するために採用することができる。

.. code-block:: bash

	sudo ptdeploy vhe add

上記のコマンドを入力した後、以下求めることができる、

VHEのドキュメントルート、VHEのファイル拡張子、VHEのApacheのコマンド、VHE IPポート、VHEバーチャルホストディレクトリ、VHEテンプレート、VHEデフォルトのテンプレート名。

ユーザーは、1つずつが、そうでなければ、コマンドライン自体のすべてを入力するすべての詳細を入力する必要があります。次のスクリーンショットは説明する

それについて

.. code-block:: bash

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

削除する
-------------

このコマンドは、特定のバーチャルホストを削除するために使用。入力を入力するには二つの方法があります。簡単な方法では、ユーザはVHE削除（rmは）を与えることができる。コマンドホストパス名とともに第二の方法を挙げることができる。次のコマンドは、ホスト名を削除するために使用される。

.. code-block:: bash

        ptdeploy vhe rm

以下のスクリーンショットは、RMの機能を示しています。

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm 

 Do you want to delete VHost/s? (Y/N) 
 y 
 Deleting vhost 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 
 14 
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Site www.siva.com disabled. 
 To activate the new configuration, you need to run: 
   service apache2 reload 
 a2dissite www.siva.com.conf done 
 VHost www.siva.com.conf Deleted  if existed 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --

 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) ddddddd.conf
 (2) default-ssl.conf
 (3) default-ssl.dpkg-remove
 (4) default.dpkg-remove
 (5) karuna
 (6) kumar.conf
 (7) llllllllllllll.conf
 (8) mmmmmm.conf
 (9) ptbuild.conf
 (10) testrepo.conf
 (11) www.dae.com.conf
 (12) www.dave.com
 (13) www.google.com
 (14) www.kkkkkkkkk.com.conf
 (15) www.murali.com.conf

 14
 Site www.kkkkkkkkk.com already disabled
 a2dissite www.kkkkkkkkk.com.conf done
 VHost www.kkkkkkkkk.com.conf Deleted  if existed
 ******************************

 1Apache VHost Editor Finished
 ******************************

.. code-block:: bash



 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.da.com.conf

 Deleting vhost
 Site www.da.com disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite www.da.com.conf done
 VHost www.da.com.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.dae.com.conf

 Deleting vhost
 Site www.dae.com disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite www.dae.com.conf done
 VHost www.dae.com.conf Deleted  if existed
 ******************************

 1Apache VHost Editor Finished
 ******************************





リスト
--------

このコマンドは、現在の仮想ホストをリストするために使用。次のコマンドは、仮想ホストをリストするために使用。

.. code-block:: bash

	ptdeploy vhe list

スクリーンショットは、リスト機能を示しています。

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe list 

 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 You have a sites available dir, so also listing available sites. 
 Current Installed VHosts: 
 --- Enabled Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 --- All Available Virtual Hosts: --- 
 (16) 000-default.conf 
 (17) ddddddd.conf 
 (18) default-ssl.conf 
 (19) default-ssl.dpkg-remove 
 (20) default.dpkg-remove 
 (21) karuna 
 (22) kumar.conf 
 (23) llllllllllllll.conf 
 (24) mmmmmm.conf 
 (25) ptbuild.conf 
 (26) www.dave.com 
 (27) www.google.com 
 (28) www.kkkkkkkkk.com.conf 
 (29) www.murali.com.conf 
 (30) www.siva.com.conf 
 (31) www.siva1.com 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 





有効にする
----------------

セキュアブートは、ブートプロセス中にロードするから悪意のあるソフトウェアや無許可のメディアを防ぐように設計機能です。この有効オプションは、サーバのブロックを可能にした。仮想ホストで使用する場合は、次のコマンドを入力した、

.. code-block:: bash
   
        ptdeploy vhe enable

このオプションはデフォルトで有効になっています。このオプションは、仮想ホストサーバがイネーブル可能にする。

アシストモジュールは、人、プロセス、テクノロジー間の相互依存性の理解を通じて高性能環境にサービスを提供するために必要な有効な機能の多くを開発しています。次のスクリーンショットは、同じことを説明しています。

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe enable 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 

 7 
 Enabling site llllllllllllll. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite llllllllllllll.conf done 
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

 kevell@corp:/# ptdeploy vhe disable 

 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) default-ssl.conf 
 (2) default-ssl.dpkg-remove 
 (3) default.dpkg-remove 
 (4) karuna 
 (5) kumar.conf 
 (6) ptbuild.conf 
 (7) www.dave.com 
 (8) www.google.com 
 (9) www.kkkkkkkkk.com.conf 
 (10) www.murali.com.conf 
 (11) www.siva.com.conf 
 (12) www.siva1.com 

 9 
 Site www.kkkkkkkkk.com disabled. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2dissite www.kkkkkkkkk.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 






メリット
---------------

* マルチユーザーが一度にアクセスすることができます。
* ユーザーは、仮想ホストを追加または削除することができます。
* 仮想ホストエディタは、ユーザーの希望に応じて仮想ホストを有効または無効にすることができます。
* 非大文字と小文字の区別。
* 裕福なUbuntuとCentOSの中で。
