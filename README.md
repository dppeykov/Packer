# Packer

## Finding the base image id with oci-cli:

- oci compute image list --compartment-id $TF_VAR_compartment_ocid | grep -A 3 "Oracle-Linux-7.7-2020"

## Useful links for the partitioning:

https://medium.com/@mattia.rossi/building-oci-custom-images-with-packer-and-the-oracle-ocisurrogate-builder-5eef4bf7d6ae

## Packer Labs on GitHub:

https://github.com/richardwark/packer-oci/tree/master/workshops/packer-oci

## Installing pluggins
Install go first and add it to the PATH - see instructions on the site
In order to install the plugin, simply clone the repo and run the following commands:

go mod init main
go build
mkdir ~/.packer.d/plugins
mv main ~/.packer.d/plugins/packer-plugin-name
