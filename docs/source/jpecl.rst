=====
PECL
=====

あらすじ
----------------

PECL 正エミッタ結合論理」の略です。Pecl は差動ロジック出力高速クロック分配回路でよく使用されます。このコマンドは、作成、削除、setpassward、ユーザーが存在します。グループの活動はこのコマンドを使っても可能。このコマンドの主な機能は、システムに基づいています。Ubuntu や CentOS を適しています。

ヘルプ コマンド
----------------------

Pecl パッケージの開発は非常に簡単になります: それはで動作が存在する、修正、作成、システム pecl の設定パスワードをサポートします。Pecl、パッケージの変更されるユーザーの既定のレイアウトするたびに、ユーザーが大量のコードを書いたはそう簡単になります。

.. code-block:: bash

	ptconfigure pecl help


次のスクリーン ショットでは、その機能について説明します。


.. code-block:: bash

 kevell@corp:/# ptconfigure pecl help
 ************************************
  This command allows you to modify create or modify pecls

  PECL, pecl

        - install
        Install
        example: ptconfigure pecl pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure pecl pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure pecl pkg-ensure --package="somename"

        - update
        Update
        example: ptconfigure pecl update
 ------------------------------
 ******************************

Install
---------

ユーザーはPECLをインストールする必要がある場合には、以下のコマンドは、プロセスを実行します。

.. code-block:: bash

	ptconfigure pecl pkg-install

.. code-block:: bash


 kevell@corp:/# ptconfigure pecl pkg-install

 Enter Package Name:
 timezonedb
 yes: standard output: Broken pipe
 yes: write error
 downloading timezonedb-2015.2.tgz ...
 Starting to download timezonedb-2015.2.tgz (198,675 bytes)
 .........................................done: 198,675 bytes
 5 source files, building
 running: phpize
 Configuring for:
 PHP Api Version:         20121113
 Zend Module Api No:      20121212
 Zend Extension Api No:   220121212
 building in /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2
 running: /tmp/pear/temp/timezonedb/configure
 checking for grep that handles long lines and -e... /bin/grep
 checking for egrep... /bin/grep -E
 checking for a sed that does not truncate output... /bin/sed
 checking for cc... cc
 checking whether the C compiler works... yes
 checking for C compiler default output file name... a.out
 checking for suffix of executables...
 checking whether we are cross compiling... no
 checking for suffix of object files... o
 checking whether we are using the GNU C compiler... yes
 checking whether cc accepts -g... yes
 checking for cc option to accept ISO C89... none needed
 checking how to run the C preprocessor... cc -E
 checking for icc... no
 checking for suncc... no
 checking whether cc understands -c and -o together... yes
 checking for system library directory... lib
 checking if compiler supports -R... no
 checking if compiler supports -Wl,-rpath,... yes
 checking build system type... x86_64-unknown-linux-gnu
 checking host system type... x86_64-unknown-linux-gnu
 checking target system type... x86_64-unknown-linux-gnu
 checking for PHP prefix... /usr
 checking for PHP includes... -I/usr/include/php5 -I/usr/include/php5/main -I/usr/include/php5/TSRM -I/usr/include/php5/Zend -I/usr/include/  
 php5/ext -I/usr/include/php5/ext/date/lib
 checking for PHP extension directory... /usr/lib/php5/20121212
 checking for PHP installed headers prefix... /usr/include/php5
 checking if debug is enabled... no
 checking if zts is enabled... no
 checking for re2c... no
 configure: WARNING: You will need re2c 0.13.4 or later if you want to regenerate PHP parsers.
 checking for gawk... no
 checking for nawk... nawk
 checking if nawk is broken... no
 checking whether to enable timezonedb support... yes, shared
 checking how to print strings... printf
 checking for a sed that does not truncate output... (cached) /bin/sed
 checking for fgrep... /bin/grep -F
 checking for ld used by cc... /usr/bin/ld
 checking if the linker (/usr/bin/ld) is GNU ld... yes
 checking for BSD- or MS-compatible name lister (nm)... /usr/bin/nm -B
 checking the name lister (/usr/bin/nm -B) interface... BSD nm
 checking whether ln -s works... yes
 checking the maximum length of command line arguments... 1572864
 checking whether the shell understands some XSI constructs... yes
 checking whether the shell understands "+="... yes
 checking how to convert x86_64-unknown-linux-gnu file names to x86_64-unknown-linux-gnu format... func_convert_file_noop
 checking how to convert x86_64-unknown-linux-gnu file names to toolchain format... func_convert_file_noop
 checking for /usr/bin/ld option to reload object files... -r
 checking for objdump... objdump
 checking how to recognize dependent libraries... pass_all
 checking for dlltool... no
 checking how to associate runtime and link libraries... printf %s\n
 checking for ar... ar
 checking for archiver @FILE support... @
 checking for strip... strip
 checking for ranlib... ranlib
 checking for gawk... (cached) nawk
 checking command to parse /usr/bin/nm -B output from cc object... ok
 checking for sysroot... no
 checking for mt... mt
 checking if mt is a manifest tool... no
 checking for ANSI C header files... yes
 checking for sys/types.h... yes
 checking for sys/stat.h... yes
 checking for stdlib.h... yes
 checking for string.h... yes
 checking for memory.h... yes
 checking for strings.h... yes
 checking for inttypes.h... yes
 checking for stdint.h... yes
 checking for unistd.h... yes
 checking for dlfcn.h... yes
 checking for objdir... .libs
 checking if cc supports -fno-rtti -fno-exceptions... no
 checking for cc option to produce PIC... -fPIC -DPIC
 checking if cc PIC flag -fPIC -DPIC works... yes
 checking if cc static flag -static works... yes
 checking if cc supports -c -o file.o... yes
 checking if cc supports -c -o file.o... (cached) yes
 checking whether the cc linker (/usr/bin/ld -m elf_x86_64) supports shared libraries... yes
 checking whether -lc should be explicitly linked in... no
 checking dynamic linker characteristics... GNU/Linux ld.so
 checking how to hardcode library paths into programs... immediate
 checking whether stripping libraries is possible... yes
 checking if libtool supports shared libraries... yes
 checking whether to build shared libraries... yes
 checking whether to build static libraries... no
 configure: creating ./config.status
 config.status: creating config.h
 config.status: executing libtool commands
 running: make
 /bin/bash /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/libtool --mode=compile cc  -I. -I/tmp/pear/temp/timezonedb -DPHP_ATOM_INC -
 I/ tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/include -I/tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/main -I/tmp/pear/
 te  mp/timezonedb -I/usr/include/php5 -I/usr/include/php5/main -I/usr/include/php5/TSRM -I/usr/include/php5/Zend -I/usr/include/php5/ext -I/ 
 usr/include/php5/ext/date/lib -I/usr/include/php/ext/date/lib  -Wall -DHAVE_CONFIG_H  -g -O2   -c /tmp/pear/temp/timezonedb/timezonedb.c -o  
 timezonedb.lo
 libtool: compile:  cc -I. -I/tmp/pear/temp/timezonedb -DPHP_ATOM_INC -I/tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/include -I/tmp/ 
 pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/main -I/tmp/pear/temp/timezonedb -I/usr/include/php5 -I/usr/include/php5/main -I/usr/
 include/php5/TSRM -I/usr/include/php5/Zend -I/usr/include/php5/ext -I/usr/include/php5/ext/date/lib -I/usr/include/php/ext/date/lib -Wall -
 DHAVE_CONFIG_H -g -O2 -c /tmp/pear/temp/timezonedb/timezonedb.c  -fPIC -DPIC -o .libs/timezonedb.o
 /tmp/pear/temp/timezonedb/timezonedb.c: In function 'zm_startup_timezonedb':
 /tmp/pear/temp/timezonedb/timezonedb.c:83:2: warning: passing argument 1 of 'php_date_set_tzdb' discards 'const' qualifier from pointer  
 target type [enabled by default]
  php_date_set_tzdb(&timezonedb_external);
  ^
 In file included from /tmp/pear/temp/timezonedb/timezonedb.c:30:0:
 /usr/include/php5/ext/date/php_date.h:196:13: note: expected 'struct timelib_tzdb *' but argument is of type 'const struct timelib_tzdb *'
 PHPAPI void php_date_set_tzdb(timelib_tzdb *tzdb);
             ^
 /tmp/pear/temp/timezonedb/timezonedb.c: In function 'zm_info_timezonedb':
 /tmp/pear/temp/timezonedb/timezonedb.c:100:23: warning: initialization discards 'const' qualifier from pointer target type [enabled by  
 default] 
  timelib_tzdb *tzdb = &timezonedb_external;
                       ^
 /bin/bash /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/libtool --mode=link cc -DPHP_ATOM_INC -I/tmp/pear/temp/pear-build-
 rootalLvFn/ timezonedb-2015.2/include -I/tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/main -I/tmp/pear/temp/timezonedb -I/usr/ 
 include/php5 -I/usr/include/php5/main -I/usr/include/php5/TSRM -I/usr/include/php5/Zend -I/usr/include/php5/ext -I/usr/include/php5/ext/date/ 
 lib -I/usr/include/php/ext/date/lib  -Wall -DHAVE_CONFIG_H  -g -O2   -o timezonedb.la -export-dynamic -avoid-version -prefer-pic -module - 
 rpath /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/modules  timezonedb.lo
 libtool: link: cc -shared  -fPIC -DPIC  .libs/timezonedb.o    -O2   -Wl,-soname -Wl,timezonedb.so -o .libs/timezonedb.so
 libtool: link: ( cd ".libs" && rm -f "timezonedb.la" && ln -s "../timezonedb.la" "timezonedb.la" )
 /bin/bash /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/libtool --mode=install cp ./timezonedb.la /tmp/pear/temp/pear-build- 
 rootalLvFn/timezonedb-2015.2/modules
 libtool: install: cp ./.libs/timezonedb.so /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/modules/timezonedb.so
 libtool: install: cp ./.libs/timezonedb.lai /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/modules/timezonedb.la
 libtool: finish: PATH="/usr/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/home/karunakaran/bin:/home/karunakaran/karunak/ 
 bin:/sbin" ldconfig -n /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/modules
 ----------------------------------------------------------------------
 Libraries have been installed in:
   /tmp/pear/temp/pear-build-rootalLvFn/timezonedb-2015.2/modules

 If you ever happen to want to link against installed libraries
 in a given directory, LIBDIR, you must either use libtool, and
 specify the full pathname of the library, or use the `-LLIBDIR'
 flag during linking and do at least one of the following:
   - add LIBDIR to the `LD_LIBRARY_PATH' environment variable
     during execution
   - add LIBDIR to the `LD_RUN_PATH' environment variable
     during linking
   - use the `-Wl,-rpath -Wl,LIBDIR' linker flag
   - have your system administrator add LIBDIR to `/etc/ld.so.conf'

 See any operating system documentation about shared libraries for
 more information, such as the ld(1) and ld.so(8) manual pages.
 ----------------------------------------------------------------------

 Build complete.
 Don't forget to run 'make test'.

 running: make INSTALL_ROOT="/tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2" install
 Installing shared extensions:     /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2/usr/lib/php5/20121212/
 running: find "/tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2" | xargs ls -dils
 524332   4 drwxr-xr-x 3 root root   4096 Apr  9 18:11 /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2
 524354   4 drwxr-xr-x 3 root root   4096 Apr  9 18:11 /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2/usr
 524355   4 drwxr-xr-x 3 root root   4096 Apr  9 18:11 /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2/usr/lib
 524356   4 drwxr-xr-x 3 root root   4096 Apr  9 18:11 /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2/usr/lib/php5
 524357   4 drwxr-xr-x 2 root root   4096 Apr  9 18:11 /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2/usr/lib/php5/20121212
 524353 320 -rwxr-xr-x 1 root root 326764 Apr  9 18:11 /tmp/pear/temp/pear-build-rootalLvFn/install-timezonedb-2015.2/usr/lib/php5/20121212/ 
 timezonedb.so

 Build process completed successfully
 Installing '/usr/lib/php5/20121212/timezonedb.so'
 install ok: channel://pecl.php.net/timezonedb-2015.2
 configuration option "php_ini" is not set to php.ini location
 You should add "extension=timezonedb.so" to php.ini
 [Pharaoh Logging] Adding Package timezonedb from the Packager PECL executed correctly
 ******************************
 PECL Modifications:
 --------------------------------------------
 PECL: Success
 ------------------------------
 PECL Mods Finished
 ******************************


Ensure
----------

ユーザーはPECLを確保する必要がある場合、下記のコマンドは、プロセスを実行します。

.. code-block:: bash

	ptconfigure pecl pkg-ensure

.. code-block:: bash

 kevell@corp:/# ptconfigure pecl pkg-ensure

 Enter Package:
 timezonedb
 ABOUT PECL.PHP.NET/TIMEZONEDB-2015.2
 ====================================
 Release Type          PECL-style PHP extension (source code)
 Name                  timezonedb
 Channel               pecl.php.net
 Summary               Timezone Database to be used with PHP's date and
                      time functions
 Description           This extension is a drop-in replacement for the
                      builtin timezone database that
                      comes with PHP. You should only install this
                      extension in case you need to get
                      a later version of the timezone database than
                      the one that ships with PHP.

                      The data that this extension uses comes from the
                      "Olson" database, which is
                      located at http://www.iana.org/time-zones.
 Maintainers           Derick Rethans <derick@php.net> (lead)
 Release Date          2015-03-21 13:51:19
 Release Version       2015.2 (stable)
 API Version           2015.2 (stable)
 License               PHP (http://www.php.net/license)
 Release Notes         Updated to version 2015.2 (2015b)
 Required Dependencies PHP version 4.0.0
                      PEAR installer version 1.4.0b1 or newer
 package.xml version   2.0
 Last Modified         2015-04-09 12:41
 Previous Installed    - None -
 Version
 [Pharaoh Logging] Package timezonedb from the Packager PECL is Installed
 ******************************

 PECL Modifications:
 --------------------------------------------
 PECL: Success
 ------------------------------
 PECL Mods Finished
 ******************************



Remove
------------

このコマンドを使用すると、pecl を削除することができます。リムーバブル pecl 名前は単一コマンドライン自体に言及することができます。
作成するために使用されるコマンドのとおりです。


.. code-block:: bash

	ptconfigure pecl remove 



開始後の上記のコマンドとして入力、pecl の取り外し。ファイル、pecl から既に削除した場合を示すメッセージが表示されます。スクリーン ショットは、コマンドとその機能について説明します。


.. code-block:: bash


 kevell@corp:/# ptconfigure pecl pkg-remove

 Enter Package Name:
 timezonedb
 Unable to remove "extension=timezonedb.so" from php.ini
 uninstall ok: channel://pecl.php.net/timezonedb-2015.2
 ****************************** 

 PECL Modifications:
 --------------------------------------------
 PECL: Success
 ------------------------------
 PECL Mods Finished
 ******************************


Update
-------------

PECLパッケージを更新するために使用されるコマンドは、以下の通りです

.. code-block:: bash

	ptconfigure pecl update

.. code-block:: bash


 kevell@corp:/# ptconfigure pecl update
 Updating channel "doc.php.net"
 Channel "doc.php.net" is up to date
 Updating channel "pear.pdepend.org"
 Channel "pear.pdepend.org" is up to date
 Updating channel "pear.php.net"
 Channel "pear.php.net" is up to date
 Updating channel "pear.phpmd.org"
 Channel "pear.phpmd.org" is up to date
 Updating channel "pecl.php.net"
 Update of Channel "pecl.php.net" succeeded
 ******************************
 PECL Modifications:
 --------------------------------------------
 PECL: Success
 ------------------------------
 PECL Mods Finished
 ****************************** 






利点
----------------

* 非大文字小文字を区別します。
* Ubuntu や CentOS で裕福な。
* 低消費電力。
* 新しいシステム pecl を作成します。
* 削除、pecl
* 追加のグループ化が可能です。
* 削除グループが可能です。
* ショー グループが可能です。

 
