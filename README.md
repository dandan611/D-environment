# D-environment
development environment 

## Tools

* vagrant(2.0.1)
* virtualbox(5.2.4.r119785)
* vagrant plugin
  * vagrant-cachier
  * vagrant-vbguest
  
    ```
    $ vagrant plugin install vagrant-cachier
    $ vagrant plugin install vagrant-vbguest
    ```

## OS

* CentoOS 7.4

## Environment Type

1. env_prodev
  * development product 
2. env_devmng
  * development management tool operation
3. env_deploy
  * deploy and testing 

## Usage

1. start

```
$ cd <Vagrantfile directory>
$ mkdir data/
$ vagrant up
$ ssh vagrant@192.168.10.10
$ mkvirtualenv --python python3.6 <product name>
$ deactivate
```

2. stop

```
vagrant halt
```

3. destroy

```
$ vagrant destroy -f
```
