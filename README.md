# WebGoat Workshop

## Requirements

To run WebGoat in a VM you'll need to install the following tools:

* Vagrant - https://www.vagrantup.com/docs/installation/
* VirtualBox - https://www.virtualbox.org/ (or your preferred Vagrant provider)
* Ansible - http://docs.ansible.com/

        # Easiest way to install ansible is via pip
        pip install ansible

## Build WebGoat Virtual Machine

It's very important that you build the VM before you come to the workshop.
The ``vagrant up`` command will download a CentOS image to use for the VM.
If you wait until the meeting to download it, you may be waiting on the
download the whole time.

    git clone https://github.com/cyberdefdojo/web-goat-ansible
    cd web-goat-ansible
    vagrant up

## Run WebGoat

    vagrant ssh
    java -jar webgoat-container-7.0.1-war-exec.jar 
    
You should be able to see WebGoat running on [http://localhost:8080/WebGoat](http://localhost:8080/WebGoat)
