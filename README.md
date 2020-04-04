# Packer

Finding the base image id with oci-cli:
oci compute image list --compartment-id $TF_VAR_compartment_ocid | grep -A 3 "Oracle-Linux-7.7-2020"
