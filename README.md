# PAYONE replacement if module is not used

This package removes the unused OXID PAYONE module package from the shop and prevents conflicts in later updates.

## Install

if the PAYONE module is not used and should be removed from the shop installation

* Deactivate the PAYONE module in the shop backend.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer require d3/oxid-payone-replacement --update-no-dev`
    
* Manually remove the files from source/modules/fc/fcpayone.

## Uninstall

if the PAYONE module is to be used again

* Manually clean up the replacement module entry (d3/oxid-payone-replacement) from the vendor/composer/installed.json and composer.lock files.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    `composer remove d3/oxid-payone-replacement --update-no-dev`
