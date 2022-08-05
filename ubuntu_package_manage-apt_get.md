# 1. ubuntu package manage: apt-get

apt-get: low level, backward compatible;

apt: high level, based on apt-get, no backward compatible;

1. update system source tree: `apt-get update`
1. upgrades all installed packages: `apt-get upgrade`
1. install a package: `apt-get install xxx`
1. remove
    1. remove a package and keep config file: `apt-get remove xxx`
    1. remove a package and it's global config file which commonly located at "/etc" directory: `apt-get purge xxx`
    1. remove some packages which is installed by other package and no longer used: `apt-get autoremove`
1. search
    1. list all packages installed in the system: `apt list --installed`
    1. search a package whose name or description contains xxx: `apt-cache search xxx`
    1. seach xxx and show dependencies and same time: `apt-cache show xxx`
