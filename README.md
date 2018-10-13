# Settler
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
  * vagrant@192.168.10.10
2. env_devmng
  * development management tool operation
  * vagrant@192.168.10.100
3. env_deploy
  * deploy and testing 
  * vagrant@192.168.10.200

## Usage

1. start

```
$ git clone https://github.com/dandan611/Settler.git
$ cd <Vagrantfile directory:env_prodev>
$ mkdir data/
$ vagrant up
$ ssh vagrant@192.168.10.10
```

2. stop

```
vagrant halt
```

3. destroy

```
$ vagrant destroy -f
```
