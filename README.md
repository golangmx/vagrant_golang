# Vagrant con go

Entorno de desarrollo de go con vagrant.

## Introducción

El proyecto tiene como objetivo facilitar el uso de `go` evitando los problemas y dependencias comunes de los sitemas operativos, de está forma nos concentramos en el desarrollo en lugar de la instalación y configuración. El proyecto está orientado al uso del entorno por desarrolladores novatos, así que no esperes nada avanzado.

**Herramientas**

* [Ubuntu 14.04.3 LTS](http://releases.ubuntu.com/14.04/)
* [Golang 1.5.1](https://golang.org/dl/)
* [Vagrant](https://www.vagrantup.com/)
* [Mi configuración personal](https://github.com/ivan-iver/config)

**Acerca de las herramientas**

> **Go**, comunmente referido como `golang`, es un lenguaje de programación desarrollado en Google en 2007 por [Robert Griesemer](https://en.wikipedia.org/wiki/Robert_Griesemer), [Rob Pike](https://en.wikipedia.org/wiki/Rob_Pike), y [Ken Thompson](https://en.wikipedia.org/wiki/Ken_Thompson). Diseñado principalmente para la programación de sistemas, es un lenguaje que usa el tipado estático, compilado, con [recolección de basura](https://es.wikipedia.org/wiki/Recolector_de_basura) [(GC)](https://en.wikipedia.org/wiki/Garbage_collection_(computer_science)), diversas características de seguridad y  [programación concurrente](https://en.wikipedia.org/wiki/Concurrent_programming) con estílos [CSP](https://en.wikipedia.org/wiki/Communicating_sequential_processes) como característica añadida.

> **Vagrant** es un software que crea y configura entornos de desarrollo virtuales. Puedes ser visto como un [wrapper](2) sobre software de virtualización como [VirtualBox](3), [VMware](4), [KVM](5), [Contenedores Linux](6) (LXC) y que ayuda a la gestión de la configuración con el uso de [Ansible](7), [Chef](8), [Salt](9), y [Puppet](10).

> Fuente: [Wikipedia](8)
    
[1]: https://en.wikipedia.org/wiki/Development_environment_(software_development_process)
[2]: https://en.wikipedia.org/wiki/Wrapper_library
[3]: https://en.wikipedia.org/wiki/VirtualBox
[4]: https://en.wikipedia.org/wiki/VMware
[5]: https://en.wikipedia.org/wiki/Kernel-based_Virtual_Machine
[6]: https://en.wikipedia.org/wiki/Linux_Containers
[7]: https://en.wikipedia.org/wiki/Ansible_(software)
[8]: https://en.wikipedia.org/wiki/Chef_(software)
[9]: https://en.wikipedia.org/wiki/Salt_(software)
[10]: https://en.wikipedia.org/wiki/Puppet_(software)
[11]: https://en.wikipedia.org/wiki/Vagrant_(software)

**Tabla de contenido**

- [Requerimientos](#require)
- [Quickstart](#quickstart)
- [Licencia](#license)


## <a name="require">Requerimientos</a>

1. Debes tener instalado [Vagrant](http://www.vagrantup.com/downloads.html)
2. Y [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## <a name="quickstart"></a>Quickstart

Primero clonamos el repositorio:

``` bash
$ git clone https://github.com/ivan-iver/vagrant_golang.git golang
```

Después podemos correr la máquina de vagrant:

```
$ cd golang/
$ vagrant up --provision
```

Y esperamos, ya que se bajará la maquina virtual y se configurará.
Si lo deseas puedes modificar el [archivo de vagrant](Vagrantfile) y sus [opciones de configuración](ConfigOptions).

## <a name="license"></a>Copyright and license

***

Copyright (c) 2015 Iván Jaimes. Ver [LICENCIA](LICENSE) para más detalles.

## Feedback

La retroalimentación siempre es bienvenida. Si encuentras algo que pueda corregir o mejorar, por favor notificame.

[Vagrant]: http://www.vagrantup.com/
[Vagrantfile]: https://github.com/ivan-iver/vagrant_golang/blob/master/Vagrantfile
[ConfigOptions]: http://docs.vagrantup.com/v2/vagrantfile/
