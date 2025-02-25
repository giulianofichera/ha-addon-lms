## [0.0.53] 2023-01-02
### Warning
 - For 8.x series realted to baby(Radio) firmware see http://github.com/pssc/ha-addon-lms

### Changes
 - lms and CPAN support bumped to 8.3
 - lms panel available to non admin users
 - low container OS updates without package installs

### Added
 - change perms on restore logic
 - change perms on configuration option

### Fixes
 - Documenation spelling and clarifiaction
 - Remove broken heathcheck and hass-cli
 - Notification of updates users can't do anthing about
 - Fix docs example to use better smb dialect
 - Backup exlusions updated


## [0.0.52] 2021-07-13

### Fixes
 - User older base for i386 build

### Changes
 - use ghcr


## [0.0.51] 2021-06-29

### Changes
 - Sensors update evey 10 mins.

### Fixes
 - ingress imageporxy mapping (issues with favorites and radio station art in material skin)

### Changes
 - Sensors update evey 10 mins.
 - Use lint and builder workflows for build
 - Use 8.2 CPAN build repo

## [0.0.50] 2021-12-11

### Fixes
 - pemissions on /config/lms/cache
 - Fix ownership of key paths


## [0.0.49] 2021-10-24

### Fixes
 - pemissions on /config/lms/cache/tmp
 - url(X mapping in ingress
 - Fix arch of debian package pulled

### Added
 - Examples for NAS mounts cifs/nfs.

## [0.0.48] 2021-09-17

### Added
 - Support for CIFS mounts

## [0.0.47] 2021-09-12


### Added
 - Support for skins add "skin: material" to default to that skin for ingress
 - sshfs
 - Discussion forum
 - Supprot for home assistant container as a LMS "Custom OS" for updates and inital wizard

### Changes
 - Update base to debian-addon 4.2.3
 - Update LMS to version 8.2.0
 - Fix typos in readme.

### Fixes
 - Change from snapshot to backup to remove depriation warnings

## [0.0.46] 2021-07-26

### Changes
 - Multi part Docker build to reduce image size for perl modules build
 - remove support of squeezelite/localplayer to its own addon https://github.com/pssc/ha-addon-squeezelite
 - Refactor udev support.
 - Update base to debian-addon 4.2.2
 - LMS fixed to version 8.1.1
 - Disable appamour causes issues with vairous plugins
 - Pruing of installed binaries
 - limit debug output (8 hours ago) <pssc>

### Fixes
 - Fixes for aarch64 multipart build inc wget for confiure scripts to update (3 weeks ago)
 - Fixes module copy afer build, Fix add addional perl modules per lms community docker 

## [0.0.45] 2021-06-05

### Fixes
 - Fix image build issues
 - Fix memory based run mount
 - Fix /proc/asound after enabling audio
 - Fix for pulse audio permission issues with squeezebox running as an alternate user

### Changes
 - Change to pre built images
 - Change /config to allow exec for plugins to work better
 - Chnage output from lms to be line buffered for better logging 

### Added
 - Audio support in container
 - Packages for sqeezelite decoding possibly via localPlayer addon

## [0.0.44] 2020-03-07

### Fixes
 - tmpfs chnages
 - random volume creation
 - Minor information message correction

## [0.0.41] 2020-01-14

### Fixes
 - build

### Changes
 - tidy debug build package install

### Added
 - use init to mount tmpfs for /var/run, if started with right perms

## [0.0.40] 2020-01-14

### Changes
 - Build CPAN modules from source
 - Reduce image size
 - Reduce layers
 - turn of debug by default.

## [0.0.40] 2020-01-05

### Fixes
 - adm64 build
 - squeezy config for sensors

### Changes
 - Tidy Dockerfile whitespace

## [0.0.38] 2020-12-29

### Added
 - Sensors
 - Add extfat support
 - Support for media dir

### Fixes
 - Setup reqirements

## [0.0.37] 2020-08-05

### Added
 - Documentation, split and updated
 - udev supoort for direct mounting

### Changes
 - Better logging of mounts
 - Auto set name from container name.
 - Generic dir creation

### Fixes
 - package installation

## [0.0.36] 2020-06-07
### Added
 - Allow for custom init scripts and packages

### Changes
 - Increase shutdown timeout to allow cleanup and run from ram
 - Use better logos and icons 
 - Make build image versions consistant
 - Be more descriptive and indicate self build repo
 - Better description to Docker image labels 
 - Better logging of mounts
 - Auto set name from container name.

### Fixes
 - Ajax requests for ingress for trackstat
 - Change log formatting 

## [0.0.34] 2020-06-18
### Added
 - README.md for addon interface desribing basic addional functions

### Changes

### Fixes
 - Change log formatting

## [0.0.33] 2020-05-17
### Added
- Support for multiple links
- Support for multiple mounts
- Support for multiple directories
- Change log ;-)

### Changes
- Expire single mount support

### Fixes
- Container startup ordering

