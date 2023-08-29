# Overview
This project is vagrant script for terraform playground. It is developed on the Mac M1/M2 and uses QEMU as Provider.

**Prerequisite**
* Enable File Sharing([doc](https://developer.hashicorp.com/vagrant/docs/synced-folders/smb))
* Installing QEMU
# How to run?
1. Run vagrant
    ```shell
    vagrant plugin install vagrant-qemu
    vagrant up
    ```
    * `smb_username`, `smb_password` : [doc](https://developer.hashicorp.com/vagrant/docs/synced-folders/smb)
