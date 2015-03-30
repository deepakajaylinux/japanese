================
Storyplayer 
================

概要
-------------

Storyplayer は機能と非機能的なソフトウェアとサービス、firehose スケールでテストをビルドのテストのための DataSift のテスト ツールです。それは素敵な PHPUnit 用の単体テストの開発者、および Behat の受け入れのプロダクト マネージャーによってテストの間座っています。

Storyplayer は、新しいオープン ソースのテスト ツールです。Storyplayer 当初設計され DataSift のリアルタイム ファイアホース フィルタ リング製品をテストします。これはサービス指向のアーキテクチャで構成されます。


* データの piplines （ZeroMQ と HTTP を使用して) 
* サービス (HTTP および時々 ZeroMQ を使用) のサポート 
* 内部および一般向け Api (JSON over HTTP を使用) 
* (HTML を使用して) フロント エンド インターフェイス


Storyplayer は、Storyplayer ユーザーのようにあなたのソフトウェアと対話する設計されているため、任意の言語で書かれたソフトウェアをテストできます。


Helpコマンド
----------------------

このコマンドは、Storyplayer の使用状況を判断するのに役立ちます。ユーザーはこのモジュールを実行する別の方法/形式について知っているに来る。このコマンドをこのコマンドの目的を知っているエンド ・ ユーザーをガイドします。以下に、コマンドと同じのスクリーン ショット。

.. code-block:: bash

	ptconfigure Storyplayer help

.. code-block:: bash


 kevell@corp:/# ptconfigure storyplayer help
 ******************************


  This command allows you to install Storyplayer from a GC Repo.

  Storyplayer

        - install
        Install Storyplayer
        example: cleopatra storyplayer install
 
        - remove
        Remove Storyplayer
        example: cleopatra storyplayer uninstall

 ------------------------------
 End Help
 ******************************




インストール
----------------

ユーザーのマシンで storyplayer モジュールをインストールする必要がある場合、特定のコマンドの下のインストール プロセスが実行されます。


.. code-block:: bash
        
        ptconfigure storyplayer install

.. code-block:: bash 


 kevell@corp:/# ptconfigure storyplayer install

 Install Storyplayer ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          Storyplayer         *
 *******************************
 What is the program data directory? Found "/opt/storyplayer" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 Program Data Folder /opt/storyplayer Deleted if existed
 Creating /tmp/ptconfigure-temp-script-30388926365.sh
 chmod 755 /tmp/ptconfigure-temp-script-30388926365.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-30388926365.sh Permissions
 Executing /tmp/ptconfigure-temp-script-30388926365.sh
 --2015-03-13 09:28:16--  https://getcomposer.org/installer
 Resolving getcomposer.org (getcomposer.org)... 87.98.253.108
 Connecting to getcomposer.org (getcomposer.org)|87.98.253.108|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [text/plain]
 Saving to: â€˜installerâ€™

    [                <=>                                                                                       ] 2,74,634    38.3KB/s   in 7.0s   
 Installing symfony/yaml (v2.6.4)
 Downloading https://api.github.com/repos/symfony/Yaml/zipball/60ed7751671113cf1ee7d7778e691642c2e9acd8
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/symfony/yaml/60ed7751671113cf1ee7d7778e691642c2e9acd8.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/symfony/yaml/Symfony/Component/Yaml/608f7b6f8cc4abc17da0dac15662c7c4' -d '/opt/storyplayer/storyplayer/vendor/composer/0d5e9897' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/0d5e9897'

    REASON: datasift/storyplayer 1.5.8 requires symfony/yaml 2.* -> satisfiable by symfony/yaml[2.0.4, 2.0.5, 2.0.6, 2.0.7, v2.0.10, v2.0.12, v2.0.13, v2.0.14, v2.0.15, v2.0.16, v2.0.17, v2.0.18, v2.0.19, v2.0.20, v2.0.21, v2.0.22, v2.0.23, v2.0.24, v2.0.25, v2.0.9, v2.1.0, v2.1.1, v2.1.10, v2.1.11, v2.1.12, v2.1.13, v2.1.2, v2.1.3, v2.1.4, v2.1.5, v2.1.6, v2.1.7, v2.1.8, v2.1.9, v2.2.0, v2.2.1, v2.2.10, v2.2.11, v2.2.2, v2.2.3, v2.2.4, v2.2.5, v2.2.6, v2.2.7, v2.2.8, v2.2.9, v2.3.0, v2.3.1, v2.3.10, v2.3.11, v2.3.12, v2.3.13, v2.3.14, v2.3.15, v2.3.16, v2.3.17, v2.3.18, v2.3.19, v2.3.2, v2.3.20, v2.3.21, v2.3.22, v2.3.23, v2.3.24, v2.3.25, v2.3.3, v2.3.4, v2.3.5, v2.3.6, v2.3.7, v2.3.8, v2.3.9, v2.4.0, v2.4.1, v2.4.10, v2.4.2, v2.4.3, v2.4.4, v2.4.5, v2.4.6, v2.4.7, v2.4.8, v2.4.9, v2.5.0, v2.5.1, v2.5.10, v2.5.2, v2.5.3, v2.5.4, v2.5.5, v2.5.6, v2.5.7, v2.5.8, v2.5.9, v2.6.0, v2.6.1, v2.6.2, v2.6.3, v2.6.4].

  - Installing datasift/ifconfig-parser (0.1.1)
 Downloading https://api.github.com/repos/datasift/ifconfig-parser-php/zipball/7a47ed1aa85e6742555724ae969c115bb637f849
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/datasift/ifconfig-parser/7a47ed1aa85e6742555724ae969c115bb637f849.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/datasift/ifconfig-parser/7a60b9e6dd74a292d2e0206419acad01' -d '/opt/storyplayer/storyplayer/vendor/composer/eadbda9d' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/eadbda9d'

    REASON: datasift/netifaces 0.1.0 requires datasift/ifconfig-parser * -> satisfiable by datasift/ifconfig-parser[0.1.0, 0.1.1].

  - Installing datasift/os (0.1.2)
 Downloading https://api.github.com/repos/datasift/os-php/zipball/e21c7483663a9407668b819416c5f7e80eded31f
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/datasift/os/e21c7483663a9407668b819416c5f7e80eded31f.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/datasift/os/7e5bf2fa027859f511091d6f1c5e8943' -d '/opt/storyplayer/storyplayer/vendor/composer/9b169e68' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/9b169e68'

    REASON: datasift/netifaces 0.1.0 requires datasift/os * -> satisfiable by datasift/os[0.1.0, 0.1.1, 0.1.2].

  - Installing datasift/netifaces (0.1.0)
 Downloading https://api.github.com/repos/datasift/netifaces/zipball/c01728273b0718bff86817e62a26fd358eb39996
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/datasift/netifaces/c01728273b0718bff86817e62a26fd358eb39996.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/datasift/netifaces/77390360a5b5ceb6a0f0bdde18368c14' -d '/opt/storyplayer/storyplayer/vendor/composer/7435e2a0' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/7435e2a0'

    REASON: datasift/storyplayer 1.5.8 requires datasift/netifaces * -> satisfiable by datasift/netifaces[0.1.0].

  - Installing symfony/event-dispatcher (v2.6.4)
 Downloading https://api.github.com/repos/symfony/EventDispatcher/zipball/f75989f3ab2743a82fe0b03ded2598a2b1546813
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/symfony/event-dispatcher/f75989f3ab2743a82fe0b03ded2598a2b1546813.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/symfony/event-dispatcher/Symfony/Component/EventDispatcher/f023f688e5c023b05e0833ab4e2e83f3' -d '/opt/storyplayer/storyplayer/vendor/composer/ba821eaa' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/ba821eaa'

    REASON: guzzle/guzzle v3.9.2 requires symfony/event-dispatcher ~2.1 -> satisfiable by symfony/event-dispatcher[v2.1.0, v2.1.1, v2.1.10, v2.1.11, v2.1.12, v2.1.13, v2.1.2, v2.1.3, v2.1.4, v2.1.5, v2.1.6, v2.1.7, v2.1.8, v2.1.9, v2.2.0, v2.2.1, v2.2.10, v2.2.11, v2.2.2, v2.2.3, v2.2.4, v2.2.5, v2.2.6, v2.2.7, v2.2.8, v2.2.9, v2.3.0, v2.3.1, v2.3.10, v2.3.11, v2.3.12, v2.3.13, v2.3.14, v2.3.15, v2.3.16, v2.3.17, v2.3.18, v2.3.19, v2.3.2, v2.3.20, v2.3.21, v2.3.22, v2.3.23, v2.3.24, v2.3.25, v2.3.3, v2.3.4, v2.3.5, v2.3.6, v2.3.7, v2.3.8, v2.3.9, v2.4.0, v2.4.1, v2.4.10, v2.4.2, v2.4.3, v2.4.4, v2.4.5, v2.4.6, v2.4.7, v2.4.8, v2.4.9, v2.5.0, v2.5.1, v2.5.10, v2.5.2, v2.5.3, v2.5.4, v2.5.5, v2.5.6, v2.5.7, v2.5.8, v2.5.9, v2.6.0, v2.6.1, v2.6.2, v2.6.3, v2.6.4].

  - Installing guzzle/guzzle (v3.9.2)
 Downloading https://api.github.com/repos/guzzle/guzzle3/zipball/54991459675c1a2924122afbb0e5609ade581155
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/guzzle/guzzle/54991459675c1a2924122afbb0e5609ade581155.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/guzzle/guzzle/c0af4c3a7828a121b4fec3476e285c9e' -d '/opt/storyplayer/storyplayer/vendor/composer/b04adeaa' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/b04adeaa'

    REASON: aws/aws-sdk-php 2.7.22 requires guzzle/guzzle ~3.7 -> satisfiable by guzzle/guzzle[v3.7.0, v3.7.1, v3.7.2, v3.7.3, v3.7.4, v3.8.0, v3.8.1, v3.9.0, v3.9.1, v3.9.2].

  - Installing aws/aws-sdk-php (2.7.22)
 Downloading https://api.github.com/repos/aws/aws-sdk-php/zipball/7c97f11ca46c47209e597ebab6e74e164cdf6216
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/aws/aws-sdk-php/7c97f11ca46c47209e597ebab6e74e164cdf6216.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/aws/aws-sdk-php/ff3c26d9e20b7d54678b52c9b5f87191' -d '/opt/storyplayer/storyplayer/vendor/composer/62e7677e' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/62e7677e'

    REASON: datasift/storyplayer 1.5.8 requires aws/aws-sdk-php 2.* -> satisfiable by aws/aws-sdk-php[2.0.0, 2.0.1, 2.0.2, 2.0.3, 2.1.0, 2.1.1, 2.1.2, 2.2.0, 2.2.1, 2.3.0, 2.3.1, 2.3.2, 2.3.3, 2.3.4, 2.4.0, 2.4.1, 2.4.10, 2.4.11, 2.4.12, 2.4.2, 2.4.3, 2.4.4, 2.4.5, 2.4.6, 2.4.7, 2.4.8, 2.4.9, 2.5.0, 2.5.1, 2.5.2, 2.5.3, 2.5.4, 2.6.0, 2.6.1, 2.6.10, 2.6.11, 2.6.12, 2.6.13, 2.6.14, 2.6.15, 2.6.16, 2.6.2, 2.6.3, 2.6.4, 2.6.5, 2.6.6, 2.6.7, 2.6.8, 2.6.9, 2.7.0, 2.7.1, 2.7.10, 2.7.11, 2.7.12, 2.7.13, 2.7.14, 2.7.15, 2.7.16, 2.7.17, 2.7.18, 2.7.19, 2.7.2, 2.7.20, 2.7.21, 2.7.22, 2.7.3, 2.7.4, 2.7.5, 2.7.6, 2.7.7, 2.7.8, 2.7.9].

  - Installing mockery/mockery (0.9.3)
 Downloading https://api.github.com/repos/padraic/mockery/zipball/686f85fa5b3b079cc0157d7cd3e9adb97f0b41e1
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/mockery/mockery/686f85fa5b3b079cc0157d7cd3e9adb97f0b41e1.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/mockery/mockery/785f0a3edd73b0bdb7d7966c21c5d2bb' -d '/opt/storyplayer/storyplayer/vendor/composer/7f28b98b' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/7f28b98b'

    REASON: datasift/stone 1.9.13 requires mockery/mockery 0.9.* -> satisfiable by mockery/mockery[0.9.0, 0.9.1, 0.9.2, 0.9.3].

  - Installing sebastian/version (1.0.4)
 Downloading https://api.github.com/repos/sebastianbergmann/version/zipball/a77d9123f8e809db3fbdea15038c27a95da4058b
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/version/a77d9123f8e809db3fbdea15038c27a95da4058b.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/version/3754e43c48c06a19f73793bf8f82531a' -d '/opt/storyplayer/storyplayer/vendor/composer/6889492f' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/6889492f'

    REASON: phpunit/phpunit 4.5.0 requires sebastian/version ~1.0 -> satisfiable by sebastian/version[1.0.0, 1.0.1, 1.0.2, 1.0.3, 1.0.4].

  - Installing sebastian/global-state (1.0.0)
 Downloading https://api.github.com/repos/sebastianbergmann/global-state/zipball/c7428acdb62ece0a45e6306f1ae85e1c05b09c01
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/global-state/c7428acdb62ece0a45e6306f1ae85e1c05b09c01.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/global-state/2ba6b95e4ab3760fbdc0a5070386e9ec' -d '/opt/storyplayer/storyplayer/vendor/composer/483de02a' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/483de02a'

    REASON: phpunit/phpunit 4.5.0 requires sebastian/global-state ~1.0 -> satisfiable by sebastian/global-state[1.0.0].

  - Installing sebastian/recursion-context (1.0.0)
 Downloading https://api.github.com/repos/sebastianbergmann/recursion-context/zipball/3989662bbb30a29d20d9faa04a846af79b276252
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/recursion-context/3989662bbb30a29d20d9faa04a846af79b276252.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/recursion-context/b3c72f22bd17f683490b6a5282d7f3a5' -d '/opt/storyplayer/storyplayer/vendor/composer/1d071769' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/1d071769'

    REASON: sebastian/exporter 1.2.0 requires sebastian/recursion-context ~1.0 -> satisfiable by sebastian/recursion-context[1.0.0].

  - Installing sebastian/exporter (1.2.0)
 Downloading https://api.github.com/repos/sebastianbergmann/exporter/zipball/84839970d05254c73cde183a721c7af13aede943
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/exporter/84839970d05254c73cde183a721c7af13aede943.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/exporter/2533514510f26c88718fcf7941effeba' -d '/opt/storyplayer/storyplayer/vendor/composer/7ce7bae3' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/7ce7bae3'

    REASON: phpunit/phpunit 4.5.0 requires sebastian/exporter ~1.2 -> satisfiable by sebastian/exporter[1.2.0].

  - Installing sebastian/environment (1.2.1)
 Downloading https://api.github.com/repos/sebastianbergmann/environment/zipball/6e6c71d918088c251b181ba8b3088af4ac336dd7
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/environment/6e6c71d918088c251b181ba8b3088af4ac336dd7.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/environment/b030989406fc2d810fd209cbc370c97b' -d '/opt/storyplayer/storyplayer/vendor/composer/b869a17e' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/b869a17e'

    REASON: phpunit/phpunit 4.5.0 requires sebastian/environment ~1.2 -> satisfiable by sebastian/environment[1.2.0, 1.2.1].

  - Installing sebastian/diff (1.2.0)
 Downloading https://api.github.com/repos/sebastianbergmann/diff/zipball/5843509fed39dee4b356a306401e9dd1a931fec7
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/diff/5843509fed39dee4b356a306401e9dd1a931fec7.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/diff/0275b11a00ddec6770ddcf80f45f5045' -d '/opt/storyplayer/storyplayer/vendor/composer/1796ba86' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/1796ba86'

    REASON: sebastian/comparator 1.1.1 requires sebastian/diff ~1.2 -> satisfiable by sebastian/diff[1.2.0].

  - Installing sebastian/comparator (1.1.1)
 Downloading https://api.github.com/repos/sebastianbergmann/comparator/zipball/1dd8869519a225f7f2b9eb663e225298fade819e
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/sebastian/comparator/1dd8869519a225f7f2b9eb663e225298fade819e.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/sebastian/comparator/ce196c53a14ada40f3f0e52125deca9f' -d '/opt/storyplayer/storyplayer/vendor/composer/8a1fe81e' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/8a1fe81e'

    REASON: phpunit/phpunit 4.5.0 requires sebastian/comparator ~1.1 -> satisfiable by sebastian/comparator[1.1.0, 1.1.1].

  - Installing doctrine/instantiator (1.0.4)
 Downloading https://api.github.com/repos/doctrine/instantiator/zipball/f976e5de371104877ebc89bd8fecb0019ed9c119
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/doctrine/instantiator/f976e5de371104877ebc89bd8fecb0019ed9c119.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/doctrine/instantiator/485434fe08559549c945cc95091ce33c' -d '/opt/storyplayer/storyplayer/vendor/composer/42852e57' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/42852e57'

    REASON: phpunit/phpunit-mock-objects 2.3.0 requires doctrine/instantiator ~1.0,>=1.0.1 -> satisfiable by doctrine/instantiator[1.0.1, 1.0.2, 1.0.3, 1.0.4].

  - Installing phpdocumentor/reflection-docblock (2.0.4)
 Downloading https://api.github.com/repos/phpDocumentor/ReflectionDocBlock/zipball/d68dbdc53dc358a816f00b300704702b2eaff7b8
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpdocumentor/reflection-docblock/d68dbdc53dc358a816f00b300704702b2eaff7b8.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpdocumentor/reflection-docblock/d1a0972308473be16bda65bdaa2cf8af' -d '/opt/storyplayer/storyplayer/vendor/composer/72e855c2' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/72e855c2'

    REASON: phpspec/prophecy v1.3.1 requires phpdocumentor/reflection-docblock ~2.0 -> satisfiable by phpdocumentor/reflection-docblock[2.0.0, 2.0.1, 2.0.2, 2.0.3, 2.0.4].

  - Installing phpspec/prophecy (v1.3.1)
 Downloading https://api.github.com/repos/phpspec/prophecy/zipball/9ca52329bcdd1500de24427542577ebf3fc2f1c9
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpspec/prophecy/9ca52329bcdd1500de24427542577ebf3fc2f1c9.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpspec/prophecy/78dda2d75504c0751056397b7bc0ae20' -d '/opt/storyplayer/storyplayer/vendor/composer/a8b9b8b0' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/a8b9b8b0'

    REASON: phpunit/phpunit 4.5.0 requires phpspec/prophecy ~1.3.1 -> satisfiable by phpspec/prophecy[v1.3.1].

  - Installing phpunit/php-text-template (1.2.0)
 Downloading https://api.github.com/repos/sebastianbergmann/php-text-template/zipball/206dfefc0ffe9cebf65c413e3d0e809c82fbf00a
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/php-text-template/206dfefc0ffe9cebf65c413e3d0e809c82fbf00a.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/php-text-template/3e1b52545afad3b107af424940d7fbf1' -d '/opt/storyplayer/storyplayer/vendor/composer/1f635d33' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/1f635d33'

    REASON: phpunit/phpunit 4.5.0 requires phpunit/php-text-template ~1.2 -> satisfiable by phpunit/php-text-template[1.2.0].

  - Installing phpunit/phpunit-mock-objects (2.3.0)
 Downloading https://api.github.com/repos/sebastianbergmann/phpunit-mock-objects/zipball/c63d2367247365f688544f0d500af90a11a44c65
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/phpunit-mock-objects/c63d2367247365f688544f0d500af90a11a44c65.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/phpunit-mock-objects/80d5d7c80920ce66d3db4a290b0d7003' -d '/opt/storyplayer/storyplayer/vendor/composer/06696499' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/06696499'

    REASON: phpunit/phpunit 4.5.0 requires phpunit/phpunit-mock-objects ~2.3 -> satisfiable by phpunit/phpunit-mock-objects[2.3.0].

  - Installing phpunit/php-timer (1.0.5)
 Downloading https://api.github.com/repos/sebastianbergmann/php-timer/zipball/19689d4354b295ee3d8c54b4f42c3efb69cbc17c
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/php-timer/19689d4354b295ee3d8c54b4f42c3efb69cbc17c.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/php-timer/6af874a6494f793d2b2f16397503d95f' -d '/opt/storyplayer/storyplayer/vendor/composer/82395102' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/82395102'

    REASON: phpunit/phpunit 4.5.0 requires phpunit/php-timer ~1.0.2 -> satisfiable by phpunit/php-timer[1.0.3, 1.0.4, 1.0.5].

  - Installing phpunit/php-file-iterator (1.3.4)
 Downloading https://api.github.com/repos/sebastianbergmann/php-file-iterator/zipball/acd690379117b042d1c8af1fafd61bde001bf6bb
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/php-file-iterator/acd690379117b042d1c8af1fafd61bde001bf6bb.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/php-file-iterator/29860041713566d1f8eab5bbde1c27ed' -d '/opt/storyplayer/storyplayer/vendor/composer/c1800bc8' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/c1800bc8'

    REASON: phpunit/phpunit 4.5.0 requires phpunit/php-file-iterator ~1.3.2 -> satisfiable by phpunit/php-file-iterator[1.3.2, 1.3.3, 1.3.4].

  - Installing phpunit/php-token-stream (1.4.0)
 Downloading https://api.github.com/repos/sebastianbergmann/php-token-stream/zipball/db32c18eba00b121c145575fcbcd4d4d24e6db74
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/php-token-stream/db32c18eba00b121c145575fcbcd4d4d24e6db74.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/php-token-stream/d8f7babec98475553410c41ce40cebf8' -d '/opt/storyplayer/storyplayer/vendor/composer/c8215ab0' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/c8215ab0'

    REASON: phpunit/php-code-coverage 2.0.15 requires phpunit/php-token-stream ~1.3 -> satisfiable by phpunit/php-token-stream[1.3.0, 1.4.0].

  - Installing phpunit/php-code-coverage (2.0.15)
 Downloading https://api.github.com/repos/sebastianbergmann/php-code-coverage/zipball/34cc484af1ca149188d0d9e91412191e398e0b67
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/php-code-coverage/34cc484af1ca149188d0d9e91412191e398e0b67.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/php-code-coverage/070381e4e7d02391a7267ca3286dc116' -d '/opt/storyplayer/storyplayer/vendor/composer/b9bd1f43' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/b9bd1f43'

    REASON: phpunit/phpunit 4.5.0 requires phpunit/php-code-coverage ~2.0 -> satisfiable by phpunit/php-code-coverage[2.0.0, 2.0.1, 2.0.10, 2.0.11, 2.0.12, 2.0.13, 2.0.14, 2.0.15, 2.0.2, 2.0.3, 2.0.4, 2.0.5, 2.0.6, 2.0.7, 2.0.8, 2.0.9].

  - Installing phpunit/phpunit (4.5.0)
 Downloading https://api.github.com/repos/sebastianbergmann/phpunit/zipball/5b578d3865a9128b9c209b011fda6539ec06e7a5
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phpunit/phpunit/5b578d3865a9128b9c209b011fda6539ec06e7a5.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phpunit/phpunit/c4fb13d2d024ebe94df766398785564e' -d '/opt/storyplayer/storyplayer/vendor/composer/0aa0e7f3' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/0aa0e7f3'

    REASON: datasift/stone 1.9.13 requires phpunit/phpunit ~4.5 -> satisfiable by phpunit/phpunit[4.5.0].

  - Installing datasift/stone (1.9.13)
 Downloading https://api.github.com/repos/datasift/ms-lib-stone/zipball/07ac2c438fb2fd783ed60b443805aa91062c39d0
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/datasift/stone/07ac2c438fb2fd783ed60b443805aa91062c39d0.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/datasift/stone/51d992cf8e39cf7d041bc51408514788' -d '/opt/storyplayer/storyplayer/vendor/composer/ae4de42c' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/ae4de42c'

    REASON: datasift/storyplayer 1.5.8 requires datasift/stone >=1.5.0 -> satisfiable by datasift/stone[1.5.0, 1.5.1, 1.5.2, 1.5.3, 1.5.4, 1.5.5, 1.6.0, 1.6.1, 1.6.2, 1.6.3, 1.6.4, 1.6.5, 1.6.6, 1.6.7, 1.6.8, 1.6.9, 1.7.0, 1.7.1, 1.7.2, 1.8.0, 1.8.1, 1.9.0, 1.9.1, 1.9.10, 1.9.11, 1.9.12, 1.9.13, 1.9.2, 1.9.3, 1.9.4, 1.9.5, 1.9.6, 1.9.7, 1.9.8, 1.9.9].

  - Installing datasift/webdriver (1.5.2)
 Downloading https://api.github.com/repos/datasift/php_webdriver/zipball/3274a66007382a25fec3a5da2deb5fb55eab5927
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/datasift/webdriver/3274a66007382a25fec3a5da2deb5fb55eab5927.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/datasift/webdriver/e942c5be451d58c532a3277af5465426' -d '/opt/storyplayer/storyplayer/vendor/composer/ded7c928' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/ded7c928'

    REASON: datasift/storyplayer 1.5.8 requires datasift/webdriver >=1.5.0 -> satisfiable by datasift/webdriver[1.5.0, 1.5.1, 1.5.2].

  - Installing phix/exceptionslib (1.1.6)
 Downloading https://api.github.com/repos/stuartherbert/ExceptionsLib/zipball/b27d393a178ad664dec4a0d49263608b9ad9806c
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/exceptionslib/b27d393a178ad664dec4a0d49263608b9ad9806c.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/exceptionslib/d37a7542ee710c1d8c2ced57afafd14c' -d '/opt/storyplayer/storyplayer/vendor/composer/42ed2734' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/42ed2734'

    REASON: phix/validationlib 4.2.0 requires phix/exceptionslib 1.* -> satisfiable by phix/exceptionslib[1.1.5, 1.1.6].

  - Installing phix/validationlib (4.2.0)
 Downloading https://api.github.com/repos/stuartherbert/ValidationLib/zipball/70bc0f9f37ca2893cb55fa5d53f6a211ed22578d
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/validationlib/70bc0f9f37ca2893cb55fa5d53f6a211ed22578d.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/validationlib/dcac5c90f670780d971f2ddddd8981d1' -d '/opt/storyplayer/storyplayer/vendor/composer/0f0782b2' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/0f0782b2'

    REASON: phix/cliengine 1.3.2 requires phix/validationlib 4.* -> satisfiable by phix/validationlib[4.0.1, 4.0.2, 4.1.0, 4.2.0].

  - Installing phix/consoledisplaylib (4.0.2)
 Downloading https://api.github.com/repos/stuartherbert/ConsoleDisplayLib/zipball/d5860841db19a444266a92cc2e9420fce7a97e21
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/consoledisplaylib/d5860841db19a444266a92cc2e9420fce7a97e21.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/consoledisplaylib/c57b0aee824e9176631789e8539f3353' -d '/opt/storyplayer/storyplayer/vendor/composer/200d8b4a' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/200d8b4a'

    REASON: phix/cliengine 1.3.2 requires phix/consoledisplaylib 4.* -> satisfiable by phix/consoledisplaylib[4.0.1, 4.0.2].

  - Installing phix/contractlib (2.1.4)
 Downloading https://api.github.com/repos/stuartherbert/ContractLib/zipball/93f7a623426063f3a13f17a3a940cb80cc9a05b4
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/contractlib/93f7a623426063f3a13f17a3a940cb80cc9a05b4.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/contractlib/88dbd4c59b5d71c35ed7bb3f68702542' -d '/opt/storyplayer/storyplayer/vendor/composer/06337270' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/06337270'

    REASON: phix/commandlinelib 4.2.0 requires phix/contractlib 2.* -> satisfiable by phix/contractlib[2.1.3, 2.1.4].

  - Installing phix/commandlinelib (4.2.0)
 Downloading https://api.github.com/repos/stuartherbert/CommandLineLib/zipball/447c1608d8bfd4ffd390ae61183e023495881a21
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/commandlinelib/447c1608d8bfd4ffd390ae61183e023495881a21.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/commandlinelib/d962f3a1671e6c8b413f082df120527f' -d '/opt/storyplayer/storyplayer/vendor/composer/9db26cbf' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/9db26cbf'

    REASON: phix/cliengine 1.3.2 requires phix/commandlinelib 4.* -> satisfiable by phix/commandlinelib[4.0.0, 4.0.1, 4.1.0, 4.2.0].

  - Installing phix/autoloader (4.3.3)
 Downloading https://api.github.com/repos/stuartherbert/Autoloader/zipball/bcb15eaadc74e9debd309831b2cb47b540f8a861
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/autoloader/bcb15eaadc74e9debd309831b2cb47b540f8a861.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/autoloader/e44990011ae95de29d7711a172e7d08e' -d '/opt/storyplayer/storyplayer/vendor/composer/43adb134' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/43adb134'

    REASON: datasift/storyplayer 1.5.8 requires phix/autoloader 4.* -> satisfiable by phix/autoloader[4.3.1, 4.3.2, 4.3.3].

  - Installing phix/cliengine (1.3.2)
 Downloading https://api.github.com/repos/stuartherbert/CliEngine/zipball/ad5a66a84ec3d717ef558375442bd0becee4d992
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/phix/cliengine/ad5a66a84ec3d717ef558375442bd0becee4d992.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/phix/cliengine/a6ec29317943b4c7a36b332efe2a6477' -d '/opt/storyplayer/storyplayer/vendor/composer/73af218c' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/73af218c'

    REASON: datasift/storyplayer 1.5.8 requires phix/cliengine @dev -> satisfiable by phix/cliengine[1.0.0, 1.1.0, 1.1.1, 1.2.0, 1.2.1, 1.3.0, 1.3.1, 1.3.2].

  - Installing datasift/storyplayer (1.5.8)
 Downloading https://api.github.com/repos/datasift/storyplayer/zipball/711caccdec0dc253ca6ab08273d757a7b983f8c4
    Downloading: 100%         
 Writing /home/deepak/.composer/cache/files/datasift/storyplayer/711caccdec0dc253ca6ab08273d757a7b983f8c4.zip into cache
    Extracting archive
 Executing command (CWD): unzip '/opt/storyplayer/storyplayer/vendor/datasift/storyplayer/13b06a3ef0d79cec7fc314767c604d3f' -d '/opt/storyplayer/storyplayer/vendor/composer/18616df3' && chmod -R u+w '/opt/storyplayer/storyplayer/vendor/composer/18616df3'

    REASON: Required by root: Install command rule (install datasift/storyplayer 1.5.5|install datasift/storyplayer 1.5.6|install datasift/storyplayer 1.5.7|install datasift/storyplayer 1.5.8|install datasift/storyplayer 2.0.0|install datasift/storyplayer 2.0.1|install datasift/storyplayer 2.0.2|install datasift/storyplayer 2.1.0|install datasift/storyplayer 2.1.1|install datasift/storyplayer 2.1.2)

 symfony/event-dispatcher suggests installing symfony/dependency-injection ()
 symfony/event-dispatcher suggests installing symfony/http-kernel ()
 aws/aws-sdk-php suggests installing doctrine/cache (Adds support for caching of credentials and responses)
 aws/aws-sdk-php suggests installing monolog/monolog (Adds support for logging HTTP requests and responses)
 sebastian/global-state suggests installing ext-uopz (*)
 phpdocumentor/reflection-docblock suggests installing dflydev/markdown (~1.0)
 phpdocumentor/reflection-docblock suggests installing erusev/parsedown (~1.0)
 phpunit/php-code-coverage suggests installing ext-xdebug (>=2.2.1)
 phpunit/phpunit suggests installing phpunit/php-invoker (~1.1)
 Writing lock file
 Generating autoload files
 All settings correct for using Composer
 Downloading...

 Composer successfully installed to: /opt/storyplayer/storyplayer/composer.phar
 Use it: php composer.phar
 Temp File /tmp/ptconfigure-temp-script-90378632638.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Storyplayer: Success
 ------------------------------
 Installer Finished



アンインストール
----------------

ユーザーがマシンにstoryplayerモジュールをアンインストールする必要がある場合、下記のコマンドは、アンインストールのプロセスを実行します。

.. code-block:: bash

 kevell@corp:/# ptconfigure storyplayer uninstall

 Uninstall Storyplayer? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          Storyplayer         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-32245879129.sh
 chmod 755 /tmp/ptconfigure-temp-script-32245879129.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-32245879129.sh Permissions
 Executing /tmp/ptconfigure-temp-script-32245879129.sh
 Temp File /tmp/ptconfigure-temp-script-32245879129.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 Storyplayer: Success
 ------------------------------
 Installer Finished
 ******************************

メリット
--------------

* 各ユーザー ストーリーは、1 つの機能または製品やサービスを提供している利点の簡単な説明です。

* 彼らは平易な英語で書かれていると明確な受け入れテストと製品やサービスを提供して何かの後ろに 'なぜ' を記録する場所が含まれます。

* 彼ら製品開発チーム、プロジェクト管理、あなたの建築家、エンジニア、テスト担当者の間で共有することができます。

* サービス ストーリーはユーザー ストーリーとそっくりの内部サービスおよび Api です。


当初から設計されています Storyplayer 単体テストと製品の間でそのギャップを埋めるために - あなたのストーリーのすべてのテストを自動化する受け入れテストします。


