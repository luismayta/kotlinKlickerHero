KotlinKlickerHero
#############################

|build_status| |code_climate| |github_tag| |issues_count| |github_issues| |test_coverage| |license|

:Version: 0.0.0
:Web: https://github.com/luismayta/KotlinKlickerHero
:Download: http://github.com/luismayta/KotlinKlickerHero
:Source: http://github.com/luismayta/KotlinKlickerHero
:Keywords: KotlinKlickerHero

Python Chalice Duplicated Soat

.. contents:: Table of Contents:
    :local:

Requirements
============

.. code-block::

   $ make install

Developing
==========

KotlinKlickerHero depends a chalice - Python serverless.

Setup
-----

Create `.chalice/config.json` :

.. code-block:: bash

  $ cat .chalice/config.json
    {
      "stages": {
        "dev": {
          "api_gateway_stage": "dev"
        }
      },
      "version": "2.0",
      "app_name": "duplicated-soat"
    }


Environment
-----------

.. code-block:: bash

  export AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxxxx
  export AWS_SECRET_ACCESS_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export AWS_DEFAULT_REGION=us-west-2
  export FLASK_DEBUG=1


Deploy to AWS Lambda and API Gateway
------------------------------------

Deploying by chalice cli:

.. code-block:: bash

  $ make deploy

Environment variables on your AWS Console
-----------------------------------------

Set environment variables on your AWS console.

.. code-block:: bash

  export POSITIVA_COD_SERVICIO=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export POSITIVA_APP_CONSUMIDORA=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export POSITIVA_USER=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export POSITIVA_PASSWORD=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

  export FACEBOOK_APP_ID=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export FACEBOOK_APP_VERSION=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export FACEBOOK_APP_SECRET=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export FACEBOOK_PAGE_TOKEN=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
  export FACEBOOK_VERIFY_TOKEN=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx


Others
------

Other commands for developing are written in Makefile:

.. code-block:: bash

  λ make help
    Commands:
        build                Build docker container
        clean                clean Files compiled
        up                   Up application
        deploy               Deploy Application
        environment          Make environment for developer
        documentation        Make Documentation
        install              Install Dependences
        lint                 Clean files unnecesary
        test                 make test
        help                 Show help text

Changelog
=========

Please see `changelog`_ for more information what has changed recently.

Contributing
============

Please see `contributing`_ for details.

Credits
=======

Made with :heart: :coffee:️and :pizza: by `company`_.

- `All Contributors`_

.. |code_climate| image:: https://codeclimate.com/github/luismayta/KotlinKlickerHero/badges/gpa.svg
  :target: https://codeclimate.com/github/luismayta/KotlinKlickerHero
  :alt: Code Climate

.. |github_tag| image:: https://img.shields.io/github/tag/luismayta/KotlinKlickerHero.svg?maxAge=2592000
  :target: https://github.com/luismayta/KotlinKlickerHero
  :alt: Github Tag

.. |build_status| image:: https://travis-ci.org/luismayta/KotlinKlickerHero.svg
  :target: https://travis-ci.org/luismayta/KotlinKlickerHero
  :alt: Build Status Tag

.. |github_issues| image:: https://img.shields.io/github/issues/luismayta/KotlinKlickerHero.svg
  :target: https://github.com/luismayta/KotlinKlickerHero/issues
  :alt: Github Issues

.. |issues_count| image:: https://codeclimate.com/github/luismayta/KotlinKlickerHero/badges/issue_count.svg
  :target: https://codeclimate.com/github/luismayta/KotlinKlickerHero
  :alt: Issue Count

.. |license| image:: https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square
  :target: LICENSE
  :alt: License

.. |test_coverage| image:: https://codeclimate.com/github/luismayta/KotlinKlickerHero/badges/coverage.svg
  :target: https://codeclimate.com/github/luismayta/KotlinKlickerHero/coverage
  :alt: Test Coverage

..
   Links

.. _`changelog`: CHANGELOG.rst
.. _`contributors`: AUTHORS
.. _`contributing`: CONTRIBUTING.rst
.. _`company`: https://github.com/hadenlabs
.. _`author`: https://github.com/luismayta