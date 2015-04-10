===============
NginxSBEditor
===============

概要
----------

このモジュールの既定のモジュールの罰金の一部であり、Nginx ServerBlocks 機能を処理します。これを使用するための方法論と今後のトピックでこの nginx エディターの下で機能についても見てみましょう。


Helpコマンド
---------------------

ヘルプ コマンドはその主な用途は、NginxSBEditor の主な機能は、宣言で使用することができます代替のパラメーターの一覧など NginxSBEditor に関する必要な情報のすべてを包み込む (Ex: 追加、削除、一覧表示、有効にすると、無効にする)、およびそれらの興味深い関数を宣言するために使用する構文も。NginxSBEditor の下のヘルプ オプションを宣言するため、次のコマンドを使用します。


.. code-block:: bash

		ptdeploy NginxSBEditor help


次のスクリーン ショットは、help コマンドの働きについて絵を示しています。


.. code-block:: bash

 kevell@corp:/# ptdeploy NginxSBEditor help
 ******************************


  This command is part of Default Modules and handles Nginx ServerBlocks Functions.

  NginxSBEditor, nginx-sb-editor, nginxsbe

          - add
          create a Server Block
          example: ptdeploy nginxsbe add
          sb-docroot
          sb-url
          sb-ip-port

          - rm
          remove a Server Block
          example: ptdeploy nginxsbe rm

          - list
          List current Server Blocks
          example: ptdeploy nginxsbe list

          - enable
          enable a Server Block
          example: ptdeploy nginxsbe enable

          - disable
          disable a Server Block
          example: ptdeploy nginxsbe disable

 ------------------------------
 End Help
 ******************************

使用方法
---------------

として描かれていると、上記で説明した、NginxSBEditor ヘルプ コマンドは次の関数


* Add
* Remove
* List
* Enable
* Disable


NginxSBEditor の下のこれらの興味深い関数を使用する方法を見てみましょう。


Add
------

この関数の役割を作成する/ブロックを追加する、新しいサーバーです。コマンドと追加機能の働きは下図します。


.. code-block:: bash

		ptdeploy NginxSBEditor add

上記コマンドを入力し、この追加機能の働きは以下します。

.. cssclass:: table-bordered

 +-------------------------------+-----------------------------------------+------------+---------------------------------------+
 | パラメータ                    | 代替パラメータ                          | オプション | 注釈                                  |
 +===============================+=========================================+============+=======================================+
 |Do you want to add a 		 | の代わりに NginxSBEditor,               | Y(Yes)     | ユーザーは、 Yとして入力することが    |
 |ServerBlock? (Y/N)             | 我々は使用することができます            |            | できる新しいサーバーブロックを追加    |
 |                               | nginx-sb-editor, nginxsbe また          |            | する必要がある場合                    |
 +-------------------------------+-----------------------------------------+------------------+---------------------------------+	
 |Do you want to add a           | の代わりに NginxSBEditor,               | N(No)      | ユーザーは、Nとして彼らができる新しい |
 |ServerBlock? (Y/N)             | 我々は使用することができます            |            | サーバーブロック入力を追加する必要    |
 |                               | nginx-sb-editor, nginxsbe また          |            | にない場合|                           |
 +-------------------------------+-----------------------------------------+------------+---------------------------------------+


ユーザーが進む場合、追加の処理中にサーバー ブロックを追加する、次の手順関与しています。


Step 1:

What is document root?

ユーザーが彼らがないデフォルトを続行したい場合、ルートを指定します。

Step 2:

What URL do you want to add as server name?

ユーザーを追加することになっている url を指定しなければなりません。

Step 3:

What IP? Port should be set?

ユーザーがいないデフォルトを続行する場合、ip アドレスを指定します。

Step 4:

What is your ServerBlock Template directory?

ない既定値を続行する場合、ユーザーが、ディレクトリを指定します。

Step 5:

Please check the ServerBlock

ユーザーがサーバー ブロックが追加されますを確保するための出力表示を確認してください。

Step 6:

Is this Okay? (Y/N)

他の N を Y として入力することができる場合は、ユーザーに満足している生成結果

Step 7:

What is your ServerBlock directory?

ユーザーがディレクトリを指定している。

Step 8:

Do you want to enable a server block? (Y/N)

ユーザー Y または N 自分のニーズに応じてとして入力する必要があります。


Step 9:

What is your Enabled Symlink ServerBlock directory.

サーバー ブロックが有効な場合ユーザーのディレクトリを指定しなければなりません。

次のスクリーンショットは、視覚的に前述したプロセスを示している。


.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe add
 Do you want to add a ServerBlock? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 /root/Nginx
 What URL do you want to add as server name?
 www.ngx.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What is your ServerBlock Template directory? Enter nothing for default templates
 /root/Nginxdir
 Please Choose ServerBlock Template: 
 --- Default Server Block Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-sfx
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 3
 Please check ServerBlock: server {
        listen   127.0.0.1:80 ; ## listen for ipv4; this line is default and implied
        #listen   [::]:80 default ipv6only=on; ## listen for ipv6

        root /root/Nginx/www ;
        index index.html index.htm index.php;

        # Make site accessible from http://localhost/
        server_name www.ngx.com ;

        # pass the PHP scripts to FastCGI server listening on 127.0.0.1:9000
        #
        location ~ \.php$ {
                try_files $uri =404;
                fastcgi_split_path_info ^(.+\.php)(/.+)$;
                fastcgi_pass 127.0.0.1:9000;
                fastcgi_index index.php;
                include fastcgi_params;
        }

 }

 Is this Okay? (Y/N) 
 Y
 What is your ServerBlock directory?
 /root/Nginxdir
 Do you want to enable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /home/Nginxsymlink
 Server Block Enabled Symlink Created
 ******************************
 

 1ServerBlock Creator Finished
 ******************************




Remove
----------

削除機能は、不要なサーバー ブロックを削除するに使用されます。これを行うことができます、以下コマンドを使用して


.. code-block:: bash

	ptdeploy NginxSBEditor rm

表に示すように、次のプロセスを削除に関与する上記のコマンドを入力した後


.. cssclass:: table-bordered

 +-------------------------------+-----------------------------------------+------------------+----------------------------------------+
 | パラメータ                    | 代替パラメータ                          | オプション       | 注釈                                   |
 +===============================+=========================================+==================+========================================+
 |Do you want to delete          | の代わりに NginxSBEditor,               | Y(Yes)           | ユーザーは、 Yとして入力することがで   |
 |ServerBlock/s? (Y/N)           | 我々は使用することができます            |                  | きるサーバ·ブロックを削除する必要      |
 |                               | nginx-sb-editor, nginxsbe また          |                  | がある場合                             |
 +-------------------------------+-----------------------------------------+------------------+----------------------------------------+
 |Do you want to add a           | の代わりに NginxSBEditor,               | N(No)            | ユーザは、 Nとして入力することができ   |
 |ServerBlock/s? (Y/N)           | 我々は使用することができます            |                  | るサーバ·ブロックを削除するため        |
 |                               | nginx-sb-editor, nginxsbe また          |                  | に必要とされていない場合|              |
 +-------------------------------+-----------------------------------------+------------------+----------------------------------------+



ユーザーが進む場合このプロセス中にサーバーのブロックを削除する、次の手順関与しています。

Step 1:

Deleting ServerBlock

What is your ServerBlock directory?

ユーザーがディレクトリを指定する必要があります。

Step 2:

ServerBlockを選択して下さい

--All Server Blocks: ---

(0) www.ngn.com

(1) www.ngx.com

(2) www.nx.com

ユーザーは、自分のニーズに応じて 2 ～ 0 の値を指定する必要。

Step 3:

!! Sure? Definitely delete ServerBlock? (Y/N) !!

ユーザー Y または N 自分のニーズに応じてを指定しなければなりません。

Step 4:

Do you want to disable a ServerBlock? (Y/N)

ユーザー Y または N 自分のニーズに応じてを指定しなければなりません。

Step 5:

What is your Enabled Symlink ServerBlock directory?

ユーザーがディレクトリを指定する必要があります。

次のスクリーンショットは、削除のプロセスについて視覚的に示している。


.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe rm
 Do you want to delete ServerBlock/s? (Y/N) 
 Y
 Deleting ServerBlock
 What is your ServerBlock directory?
 /root/Nginxdir
 Please Choose ServerBlock:
 ---All Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 (2) www.nx.com

 2
 !! Sure? Definitely delete ServerBlock? (Y/N) !!
 Y
 Do you want to disable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /root/home/Nginxsymlink
 Server Block www.nx.com Disabled if existed
 Server Block www.nx.com Deleted if existed
 *******************************


 1ServerBlock Creator Finished
 ******************************


List
------

リスト オプションの機能は現在インストールされているサーバー ブロックをリストします。以下に、リストに使用するコマンドが指定されました。


.. code-block:: bash

		ptdeploy NginxSBEditor list

リストのオプションに関与する次のプロセス上のコマンドを入力した後


Step 1:

What is your ServerBlock directory?

ユーザーがディレクトリを指定する必要があります。

Step 2:

What is your Enabled Symlink ServerBlock directory?

ユーザーがディレクトリを指定する必要があります。

これらの手順は、現在インストールされている ServerBlocks の彼のリストが表示されます。次のスクリーン ショットはリスト オプションの作業を視覚的に示しています。


.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe list
 What is your ServerBlock directory?
 /root/Nginxdir
 What is your Enabled Symlink ServerBlock directory?

 Current Installed ServerBlocks:
 --- Enabled Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 --- All Available Server Blocks: ---
 (2) www.ngn.com
 (3) www.ngx.com
 ******************************


 1ServerBlock Creator Finished
 ******************************


Enable
----------

イネーブル機能はserverblockを有効にするために使用されます。有効に使用するコマンドは、以下の通りです

.. code-block:: bash

	ptdeploy nginxsbe enable

.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe enable

 Do you want to enable a ServerBlock? (Y/N) 
 y
 What is your Enabled Symlink ServerBlock directory? Found "/etc/nginx/sites-enabled" - Enter nothing to use this

 Please Choose ServerBlock:
 --- All Server Blocks: ---
 (0) ServerBlocktemp
 (1) aaaaaa
 (2) as
 (3) ddd
 (4) default
 (5) default.dpkg-old
 (6) dfdkdfsd.com
 (7) dfsdfssfdfdfdf.com
 (8) google
 (9) karuna
 (10) kkkkkkk
 (11) kumark
 (12) sites-available
 (13) vijay
 (14) www.amazon.com
 (15) www.deepak.com
 (16) www.google.com
 (17) www.kkk.com

 1
 Server Block Enabled Symlink Created
 ******************************
 ServerBlock Creator Finished
 ******************************


Disable
---------

禁止機能は、サーバーのブロックを無効にするために使用される。無効にするためのコマンドは、以下に記載されている

.. code-block:: bash

	ptdeploy nginxsbe disable


.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe disable

 Do you want to disable a ServerBlock? (Y/N) 
 y
 What is your Enabled Symlink ServerBlock directory? Found "/etc/nginx/sites-enabled" - Enter nothing to use this

 Please Choose ServerBlock:
 --- All Server Blocks: ---
 (0) ServerBlocktemp
 (1) aaaaaa
 (2) as
 (3) ddd
 (4) default
 (5) default.dpkg-old
 (6) dfdkdfsd.com
 (7) dfsdfssfdfdfdf.com
 (8) google
 (9) karuna
 (10) kkkkkkk
 (11) kumark
 (12) sites-available
 (13) vijay
 (14) www.amazon.com
 (15) www.deepak.com
 (16) www.google.com
 (17) www.kkk.com

 1
 Server Block aaaaaa Disabled  if exist
 ******************************
 ServerBlock Creator Finished
 ******************************




メリット
----------

* それは裕福な両方の ubuntu と同様セント OS のように。
* 宣言で使用されるパラメーターの大文字と小文字は区別されません。
* ユーザーの追加や削除、サーバー ブロックの前であってもに、利用でき、現在インストールさ
  れているサーバー ブロックのリストを表示できます。


