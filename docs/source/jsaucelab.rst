================
SauceLabs
================


概要
----------------

醤油Labsのクラウド·テスト·プラットフォームを使用すると、自動またはインタラクティブに300+のブラウザでモバイルとウェブアプリケーションをテストすることができますし、
手動および自動テストのためのプラットフォーム。 SauceLabsは有名なセレンのWebドライバの上に構築されたクロスブラウザの自動化ツールです。しょうゆLabsの上の自動テストは、セレン及びJSのテストフレームワークと互換性があります。ソースは、デバッグを実行している、とあなたの時間とお金を節約、簡単にこれまで以上にテスト·スイートをスケーリングできます。


helpコマンド
----------------

helpコマンドは、とだけでなく、 saucelabモジュールに含まれているオプションについての目的について、ユーザーをガイドします。それはsaucelabモジュールの別のパラメータを示しています。また、 saucelabモジュールをインストールするための構文について説明します。 saucelabisためのhelpコマンドは以下の通り。


.. code-block:: bash

	ptconfigure SauceLabs help

上記のコマンドの絵画表現は、以下に記載されている


.. code-block:: bash

 kevell@corp:/# ptconfigure SauceLabs help
 ******************************


  This command allows you to update SauceLabs.

  SauceLabs, saucelabs

        - install
        Installs the latest version of saucelabs
        example: ptconfigure saucelabs install

 ------------------------------
 End Help
 ******************************


インストール
-----------------

The command used for installing the sauccelab module on the terminal is listed below,

.. code-block:: bash

	ptconfigure saucelabs install

端末上sauccelabモジュールをインストールするために使用されるコマンドは、以下に記載されている

.. code-block:: bash


 kevell@corp:/# ptconfigure saucelabs install 

 Install SauceLabs? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         SauceLabs!        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-31739300837.sh 
 chmod 755 /tmp/ptconfigure-temp-script-31739300837.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-31739300837.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-31739300837.sh 
 PHP Warning:  Module 'mcrypt' already loaded in Unknown on line 0 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 curl is already the newest version. 
 libcurl3 is already the newest version. 
 libcurl4-openssl-dev is already the newest version. 
 php5-curl is already the newest version. 
 0 upgraded, 0 newly installed, 0 to remove and 79 not upgraded. 

 Welcome to the Sausage installer! 
 --------------------------------- 

    ( \                 / ) 
     \ \.-------------./ / 
      \(    hot dog!   )/ 
        `.___________.' 

 --------------------------------- 
 - Checking for PHP...done 
 - Checking initial system requirements...done 
 - Downloading Composer install script...done 
 - Installing Composer...done 
 - Making sure Composer is up to date...done 
 - Downloading and unpacking Sausage and dependencies (this may take a while)...done 
 (You might also want Sauce Connect: add sauce/connect to your composer.json) 
 - Updating packages...done 
 - Configuring Sauce...done 
 - Downloading demo test files...done 
 - You're all set! 
 Try running 'vendor/bin/paratest -p 8 -f --phpunit=vendor/bin/phpunit WebDriverDemo.php' 
 (change to: SeleniumRCDemo.php for Selenium 1) 
 Then load https://saucelabs.com/account to see your tests running in parallel 
 Get the most out of Sausage: https://github.com/jlipps/sausage/blob/master/README.md 

 Temp File /tmp/ptconfigure-temp-script-31739300837.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 SauceLabs: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


代替パラメータ
-------------------------

端末上saucelabモジュールをアンインストールするために使用されるコマンドは、以下に記載されている

SauceLabs, saucelabs

メリット
----------

* 安全＆安心
* あなたの開発をスピードアップ
* 完全なテストプラットフォーム
* 環境の信頼性の向上








