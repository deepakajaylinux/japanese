=========
RubyBDD
=========

あらすじ
------------------

Ruby 振る舞い駆動開発 (BDD) ユーザーは、ユーザーと一緒に、Php 言語の開発者をもたらす実行可能な自己文書化テストでより良いソフトウェアの Ruby BDD をインストールできるようにあなたにテスト駆動開発、ドメイン駆動設計、受け入れテストを計画駆動技術の最高を与えます。Ubuntu やセント OS で快適します。

ヘルプ コマンド
------------------------

ヘルプ コマンド同様目的に関してユーザーを導くようにルビー Bdd モジュールに含まれているオプションについて。Help コマンドは、ptconfigure モジュールの下に Ruby Bdd の代替パラメーターを一覧表示されます。また、ユーザーの更新をインストールするための構文について説明します。Ruby Bdd のヘルプ コマンドを以下に示します。


.. code-block:: bash

		ptconfigure Ruby Bdd help

次のスクリーン ショットは Ruby Bdd の完全な努力を示しています。


.. code-block:: bash

 kevell@corp:/# ptconfigure RubyBDD help

 ******************************


  This command allows you to install Ruby RVM.

  RubyBDD, rubybdd, ruby-bdd

        - install
        Installs Ruby BDD Gems
        example: ptconfigure ruby-bdd install

 ------------------------------
 End Help
 ******************************


インストール
-------------------

更新されたバージョンで、インストールを行うために必要な Ruby Bdd のインストールも含まれます。それはモジュールをインストールする Ruby Bdd ptconfigure の下でちょうど、下記のコマンドを使用してマニフェスト プロセスです。

.. code-block:: bash

	ptconfigure Ruby Bdd Install

それは質問攻めにコマンド入力活性化後。

ユーザーが [はい] を入力するときに自動的にシステムからのチェックとルビー Bdd がインストールされます。ない場合、インストールを終了します。次のスクリーン ショットは、それを示しています。



.. code-block:: bash

 kevell@corp:/# ptconfigure ruby-bdd install

 Install Ruby BDD? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          !Ruby BDD!!        *
 *******************************
 ERROR:  Error installing cucumber:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:1:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/gherkin-2.12.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/gherkin-2.12.2/ext/gherkin_lexer_ar/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package cucumber from the Packager Gem did not execute correctly
 ERROR:  Error installing capybara:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:4:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2/ext/nokogiri/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package capybara from the Packager Gem did not execute correctly
 ERROR:  While executing gem ... (Gem::DependencyError)
     Unable to resolve dependencies: calabash-android requires rubyzip (~> 0.9.9); xamarin-test-cloud requires rubyzip (~> 1.1)
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 [Pharaoh Logging] Adding Package calabash from the Packager Gem did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 RubyBDD: Success
 ------------------------------
 Installer Finished
 ******************************

オプション
---------------


.. cssclass:: table-bordered


 +---------------------------+--------------------------------------------------+-------------+----------------------------------------+
 | パラメーター              | パラメーターの代替                               | オプション  | コメント                               |
 +===========================+==================================================+=============+========================================+
 |Install RubyBdd? (Y/N)     | 代わりにRubyBddを使用するのでは、我々は使用する  | Y           | それはファラオのツールでptconfigure    |
 |                           | ことができますruby-bdd, rubybdd.                 |             | 下RubyBddをインストールします          |
 +---------------------------+--------------------------------------------------+-------------+----------------------------------------+
 |Install RubyBdd?(Y/N)      | 代わりにRubyBddを使用するのでは、我々は使用する  | N           | システム出口インストール               |
 |                           | ことができますruby-bdd, rubybdd.|                |             |                                        |
 +---------------------------+--------------------------------------------------+-------------+----------------------------------------+


利点
----------------


* Rubybdd は Ubuntu や CentOS で裕福です
* Rubybdd 非大文字小文字の区別をサポートしています
* Rubybdd は柔軟です
* BDD を持つもう一つの大きな利点は、駆動開発-最新バージョンの rubybdd、およびパッチ ・ レベル、に応じて、ユーザーを更新できます。
  ルビー。
* インストールに使用する Rubybdd
 

