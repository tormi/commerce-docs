Keeping a Drupal Commerce site up to date
=========================================

    Note: Drupal Commerce 2 includes an upgrade path stretching back to beta1.

To update to the newest version of Drupal Commerce, you will need to
update with Composer.

.. code-block:: terminal

    composer update drupal/commerce --with-dependencies

Please note the ``--with-dependencies`` option. Without this option
specified any needed, contributed projects and libraries will not
update. Only the Drupal Commerce module will be updated.

Run your Drupal updates once all of the dependencies are updated. We
recommend running them on the command line rather than the
``update.php`` script. See the example below.

.. code-block:: terminal

    drupal update:debug
    drupal update:execute
