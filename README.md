# gVim Cookbook
## Description
The gVim cookbook installs the platform specific gvim (or equivalent) package.

## Cookbooks
* homebrew # TODO: Should package manager cookbooks be here?
* vim

## Supported Platforms
* Debian/Ubuntu
* Mac OS X
* RHEL/CentOS

## Usage
### gvim::default
Installs the "gvim" package for the platform. On Mac OS X this is
MacVim, on Centos/Debian/RHEL/Ubuntu this is `vim-gtk`.

## License and Author
### Authors
* Erran Carey (erran_carey@rapid7.com)
