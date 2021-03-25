# Vagrant で CentOS 8

- box list

~~~
(base) rinsaka@Macmini2020 Cent8 % vagrant box list
centos/7  (virtualbox, 2004.01)
centos7.2 (virtualbox, 0)
(base) rinsaka@Macmini2020 Cent8 % 
~~~

- box add

~~~
(base) rinsaka@Macmini2020 Cent8 % vagrant box add generic/centos8
==> box: Loading metadata for box 'generic/centos8'
    box: URL: https://vagrantcloud.com/generic/centos8
This box can work with multiple providers! The providers that it
can work with are listed below. Please review the list and choose
the provider you will be working with.

1) docker
2) hyperv
3) libvirt
4) parallels
5) virtualbox
6) vmware_desktop

Enter your choice: 5
==> box: Adding box 'generic/centos8' (v3.2.10) for provider: virtualbox
    box: Downloading: https://vagrantcloud.com/generic/boxes/centos8/versions/3.2.10/providers/virtualbox.box
Download redirected to host: vagrantcloud-files-production.s3-accelerate.amazonaws.com
    box: Calculating and comparing box checksum...
==> box: Successfully added box 'generic/centos8' (v3.2.10) for 'virtualbox'!
(base) rinsaka@Macmini2020 Cent8 %                  
~~~


- box list

~~~
(base) rinsaka@Macmini2020 Cent8 % vagrant box list
centos/7        (virtualbox, 2004.01)
centos7.2       (virtualbox, 0)
generic/centos8 (virtualbox, 3.2.10)
(base) rinsaka@Macmini2020 Cent8 % 
~~~

- init Vagrantfile

~~~~
(base) rinsaka@Macmini2020 Cent8 % vagrant init generic/centos8
A `Vagrantfile` has been placed in this directory. You are now
ready to `vagrant up` your first virtual environment! Please read
the comments in the Vagrantfile as well as documentation on
`vagrantup.com` for more information on using Vagrant.
(base) rinsaka@Macmini2020 Cent8 % ls
Vagrantfile
(base) rinsaka@Macmini2020 Cent8 % 
~~~~


