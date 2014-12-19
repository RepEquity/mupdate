mupdate
=======

Shell script to update drupal modules and create git commit that optionally includes url to release notes.

## Installation Notes

Make sure to add the script to your $PATH so you can run the 'mupdate' command from anywhere. There are a number of ways to accomplish this. The simplest is to add the script to the folder `/usr/local/bin`. A more correct way would be to have a bin in your user space as described [here](http://apple.stackexchange.com/questions/99788/os-x-create-a-personal-bin-directory-bin-and-run-scripts-without-specifyin).

## Requirements

Drush and Git are required to use this script. The `mupdate` command should be run insite a drupal folder and valid git repo.

## Usage Instructions

The script takes two arguments. The first is the machine name of the module, the second is the url to the update release notes. This script should be run within your Drupal site directory (just like any other drush command) which should also be a git repo.

For example:
`mupdate ctools https://www.drupal.org/node/2378333` Will download the latest version of ctools using drush and create a git commit with log message "upgrading ctools module => https://www.drupal.org/node/2378333"

The second argument is optional but highly suggested.

Let me know if you have any issues.

Thank you!

