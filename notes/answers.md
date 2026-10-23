apt update and apt upgrade are two different steps. apt update only
refreshes the list of available packages from the repositories, it does
not install or change anything on the server. apt upgrade is the step
that actually installs the newer versions of the packages that are
already installed. That is why update must be run first, because
upgrade needs the fresh list to know which packages have new versions.
In short: update = check for updates, upgrade = install them.
