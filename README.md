```
➜  /tmp symfony new tester 3.4

 Downloading Symfony...

    6.1 MiB/6.1 MiB ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓  100%

 Preparing project...

 ✔  Symfony 3.4.0 was successfully installed. Now you can:

    * Change your current directory to /tmp/tester

    * Configure your application in app/config/parameters.yml file.

    * Run your application:
        1. Execute the php bin/console server:start command.
        2. Browse to the http://localhost:8000 URL.

    * Read the documentation at http://symfony.com/doc

➜  /tmp cd tester 
➜  tester ls -la
total 168
drwxr-xr-x  9 chris chris  4096 Dec  4 21:02 .
drwxrwxrwt 17 root  root  36864 Dec  4 21:02 ..
drwxr-xr-x  4 chris chris  4096 Dec  4 21:02 app
drwxr-xr-x  2 chris chris  4096 Dec  4 21:02 bin
-rw-rw-rw-  1 chris chris  2258 Dec  4 21:02 composer.json
-rw-rw-rw-  1 chris chris 85455 Dec  4 21:02 composer.lock
-rw-r--r--  1 chris chris   265 Nov 30 17:32 .gitignore
-rw-r--r--  1 chris chris   988 Nov 30 17:32 phpunit.xml.dist
-rw-rw-rw-  1 chris chris    71 Dec  4 21:02 README.md
drwxr-xr-x  3 chris chris  4096 Nov 30 17:32 src
drwxr-xr-x  3 chris chris  4096 Dec  4 21:02 tests
drwxr-xr-x  5 chris chris  4096 Dec  4 21:02 var
drwxr-xr-x 16 chris chris  4096 Dec  4 21:02 vendor
drwxr-xr-x  2 chris chris  4096 Dec  4 21:02 web
➜  tester composer install
Loading composer repositories with package information
Installing dependencies (including require-dev) from lock file
Nothing to install or update
Generating autoload files
> Incenteev\ParameterHandler\ScriptHandler::buildParameters
Updating the "app/config/parameters.yml" file
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::buildBootstrap
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::clearCache

 // Clearing the cache for the dev environment with debug                       
 // true                                                                        

                                                                                
 [OK] Cache for the "dev" environment (debug=true) was successfully cleared.    
                                                                                

> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::installAssets

 Trying to install assets as relative symbolic links.

                                                                                
 [OK] No assets were provided by any bundle.                                    
                                                                                

> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::installRequirementsFile
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::prepareDeploymentTarget
➜  tester rm -rf vendor 
➜  tester composer install
Loading composer repositories with package information
Installing dependencies (including require-dev) from lock file
Package operations: 38 installs, 0 updates, 0 removals
  - Installing doctrine/lexer (v1.0.1) Loading from cache
  - Installing doctrine/annotations (v1.2.7) Loading from cache
  - Installing twig/twig (v1.35.0) Loading from cache
  - Installing symfony/polyfill-util (v1.6.0) Loading from cache
  - Installing paragonie/random_compat (v2.0.11) Loading from cache
  - Installing symfony/polyfill-php70 (v1.6.0) Loading from cache
  - Installing symfony/polyfill-php56 (v1.6.0) Loading from cache
  - Installing symfony/polyfill-mbstring (v1.6.0) Loading from cache
  - Installing symfony/symfony (v3.4.0) Downloading: 100%         
  - Installing symfony/polyfill-intl-icu (v1.6.0) Loading from cache
  - Installing symfony/polyfill-apcu (v1.6.0) Loading from cache
  - Installing psr/simple-cache (1.0.0) Loading from cache
  - Installing psr/log (1.0.2) Loading from cache
  - Installing psr/link (1.0.0) Loading from cache
  - Installing psr/container (1.0.0) Loading from cache
  - Installing psr/cache (1.0.1) Loading from cache
  - Installing fig/link-util (1.0.0) Loading from cache
  - Installing doctrine/inflector (v1.1.0) Loading from cache
  - Installing doctrine/collections (v1.3.0) Loading from cache
  - Installing doctrine/cache (v1.6.2) Loading from cache
  - Installing doctrine/common (v2.6.2) Loading from cache
  - Installing jdorn/sql-formatter (v1.2.17) Loading from cache
  - Installing doctrine/doctrine-cache-bundle (1.3.2) Loading from cache
  - Installing doctrine/dbal (v2.5.13) Loading from cache
  - Installing doctrine/doctrine-bundle (1.8.1) Loading from cache
  - Installing doctrine/instantiator (1.0.5) Loading from cache
  - Installing doctrine/orm (v2.5.13) Loading from cache
  - Installing incenteev/composer-parameter-handler (v2.1.2) Loading from cache
  - Installing composer/ca-bundle (1.1.0) Loading from cache
  - Installing sensiolabs/security-checker (v4.1.6) Loading from cache
  - Installing sensio/distribution-bundle (v5.0.21) Loading from cache
  - Installing sensio/framework-extra-bundle (v5.1.1) Downloading: 100%         
  - Installing monolog/monolog (1.23.0) Loading from cache
  - Installing symfony/monolog-bundle (v3.1.2) Loading from cache
  - Installing swiftmailer/swiftmailer (v5.4.8) Loading from cache
  - Installing symfony/swiftmailer-bundle (v2.6.7) Loading from cache
  - Installing sensio/generator-bundle (v3.1.6) Loading from cache
  - Installing symfony/phpunit-bridge (v3.4.0) Loading from cache
paragonie/random_compat suggests installing ext-libsodium (Provides a modern crypto API that can be used to generate random bytes.)
symfony/polyfill-intl-icu suggests installing ext-intl (For best performance)
doctrine/doctrine-cache-bundle suggests installing symfony/security-acl (For using this bundle to cache ACLs)
sensio/framework-extra-bundle suggests installing symfony/psr-http-message-bridge (To use the PSR-7 converters)
monolog/monolog suggests installing aws/aws-sdk-php (Allow sending log messages to AWS services like DynamoDB)
monolog/monolog suggests installing doctrine/couchdb (Allow sending log messages to a CouchDB server)
monolog/monolog suggests installing ext-amqp (Allow sending log messages to an AMQP server (1.0+ required))
monolog/monolog suggests installing ext-mongo (Allow sending log messages to a MongoDB server)
monolog/monolog suggests installing graylog2/gelf-php (Allow sending log messages to a GrayLog2 server)
monolog/monolog suggests installing mongodb/mongodb (Allow sending log messages to a MongoDB server via PHP Driver)
monolog/monolog suggests installing php-amqplib/php-amqplib (Allow sending log messages to an AMQP server using php-amqplib)
monolog/monolog suggests installing php-console/php-console (Allow sending log messages to Google Chrome)
monolog/monolog suggests installing rollbar/rollbar (Allow sending log messages to Rollbar)
monolog/monolog suggests installing ruflin/elastica (Allow sending log messages to an Elastic Search server)
monolog/monolog suggests installing sentry/sentry (Allow sending log messages to a Sentry server)
symfony/phpunit-bridge suggests installing ext-zip (Zip support is required when using bin/simple-phpunit)
Generating autoload files
> Incenteev\ParameterHandler\ScriptHandler::buildParameters
Updating the "app/config/parameters.yml" file
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::buildBootstrap
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::clearCache

 // Clearing the cache for the dev environment with debug                       
 // true                                                                        

                                                                                
 [OK] Cache for the "dev" environment (debug=true) was successfully cleared.    
                                                                                

> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::installAssets

 Trying to install assets as relative symbolic links.

                                                                                
 [OK] No assets were provided by any bundle.                                    
                                                                                

> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::installRequirementsFile
> Sensio\Bundle\DistributionBundle\Composer\ScriptHandler::prepareDeploymentTarget
➜  tester php bin/console server:start

                                                                                                                        
 [OK] Server listening on http://127.0.0.1:8000                                                                         
                                                                                                                        

➜  tester git remote add origin https://github.com/codereviewvideos/member-form-example-test.git
fatal: Not a git repository (or any of the parent directories): .git
➜  tester git init
Initialised empty Git repository in /tmp/tester/.git/
➜  tester git:(master) ✗ ga .
➜  tester git:(master) ✗ gc -am "init"
[master (root-commit) 7bbb1a6] init
 42 files changed, 4806 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 .idea/encodings.xml
 create mode 100644 .idea/modules.xml
 create mode 100644 .idea/php.xml
 create mode 100644 .idea/tester.iml
 create mode 100644 .idea/workspace.xml
 create mode 100644 README.md
 create mode 100644 app/.htaccess
 create mode 100644 app/AppCache.php
 create mode 100644 app/AppKernel.php
 create mode 100644 app/Resources/views/base.html.twig
 create mode 100644 app/Resources/views/default/index.html.twig
 create mode 100644 app/Resources/views/form-example/index.html.twig
 create mode 100644 app/config/config.yml
 create mode 100644 app/config/config_dev.yml
 create mode 100644 app/config/config_prod.yml
 create mode 100644 app/config/config_test.yml
 create mode 100644 app/config/parameters.yml.dist
 create mode 100644 app/config/routing.yml
 create mode 100644 app/config/routing_dev.yml
 create mode 100644 app/config/security.yml
 create mode 100644 app/config/services.yml
 create mode 100755 bin/console
 create mode 100755 bin/symfony_requirements
 create mode 100644 composer.json
 create mode 100644 composer.lock
 create mode 100644 phpunit.xml.dist
 create mode 100644 src/.htaccess
 create mode 100644 src/AppBundle/AppBundle.php
 create mode 100644 src/AppBundle/Controller/DefaultController.php
 create mode 100644 tests/AppBundle/Controller/DefaultControllerTest.php
 create mode 100644 var/SymfonyRequirements.php
 create mode 100644 var/cache/.gitkeep
 create mode 100644 var/logs/.gitkeep
 create mode 100644 var/sessions/.gitkeep
 create mode 100644 web/.htaccess
 create mode 100644 web/app.php
 create mode 100644 web/app_dev.php
 create mode 100644 web/apple-touch-icon.png
 create mode 100644 web/config.php
 create mode 100644 web/favicon.ico
 create mode 100644 web/robots.txt

```
