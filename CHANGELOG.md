# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [2.0.0] - 2020-11-04
### Added
- MariaDB Instance is included in to the template
- Downloading and building locally your MariaDB Docker Image.
- AWS S3 and Cloudian HyperStore S3 Bucket can be configured part of the installation
- Added Support for specify StorageClass where you PVC will be created.
- Added section comments to easier understand what's going on.

### Changed
- Moved nginx.conf in to the template file for easier changing the configuration with PR
- Moved all configuration in to a ConfigMap files.
- You can now change the Username, Database for MariaDB and the password and root password get automated generated.
- We are now creating two Persistent Volumes, one for NextCloud and one for MariaDB.
- Forward all support to NextCloud because this is nothing that Cristie Supporting.

### Removed
- Removed BuildConfig because of nginx.conf is part of the template.
- Removed the mariadb-backup.yaml, because Cristie Recommending real backup software for Openshift Container.

## [1.0.0] - 2017-08-29
### Added
- Initial release from [tobru](https://github.com/tobru/nextcloud-openshift)
