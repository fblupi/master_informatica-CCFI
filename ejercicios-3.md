---
layout: ejercicios
---

# Ejercicios

## Tema 3: Orquestación de máquinas virtuales

### Ejercicio 1

**Instalar una máquina virtual Debian usando Vagrant y conectar con ella**

```
vagrant box add debian-jessie https://github.com/holms/vagrant-jessie-box/releases/download/Jessie-v0.1/Debian-jessie-amd64-netboot.box
```

![Vagrant Add](images/vagrant-add.png "vagrant-add")

```
vagrant init debian-jessie
```

![Vagrant Init](images/vagrant-init.png "vagrant-init")

```
vagrant up
```

![Vagrant Up](images/vagrant-up.png "vagrant-up")


```
vagrant ssh
```

![Vagrant SSH](images/vagrant-ssh.png "vagrant-ssh")

### Ejercicio 2

**Crear un script para provisionar `nginx` o cualquier otro servidor web que pueda ser útil para alguna otra práctica**

Cambiar el archivo `Vagrantfile`:

```rb
Vagrant.configure("2") do |config|
  config.vm.box = "debian-jessie"
  config.vm.provision "shell", inline: "sudo apt-get update && sudo apt-get install -y nginx"
end
```

Ejecutar en consola:

```
vagrant provision
```

![Vagrant nginx](images/vagrant-nginx.png "vagrant-nginx")

---

Volver a [home](index).
