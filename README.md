[![Build Status](https://travis-ci.org/paul-m/drupal_dependency_bounds_test.svg?branch=master)](https://travis-ci.org/paul-m/drupal_dependency_bounds_test)


Drupal Dependency Bounds Test
=============================

This test asks the following question:

What happens when we don't use Drupal 8.4.x's composer.lock file?
-----------------------------------------------------------------

We essentially follow this pattern:

    $ composer update
    $ ./vendor/bin/phpunit -c core/ --testsuite unit

We do this with both `--prefer-lowest` and without.
