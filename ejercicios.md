---
layout: ejercicios
---

# Ejercicios

## Tema 1: Arquitecturas software para la nube

### Ejercicio 1

**Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?**

La aplicación [G-Tech](http://www.lourigeek.com/gtech/) realizada por mi y otros dos compañeros durante las prácticas de Diseño de Interfaces de usuario. Está disponible en un [repositorio público en GitHub](https://github.com/fblupi/grado_informatica-DIU).

Esta aplicación usa el patrón Modelo Vista Controlador (MVC). Usando SQL en el modelo; HTML, CSS y JavaScript en la vista y PHP en el controlador.

Para evolucionar a un patrón tipo microservicios debería convertir distintos componentes de la aplicación en microservicios:

- Uno para la vista
- Otro por cada uno de los módulos de la aplicación (usuarios, empresas, salas y eventos).
- Para comunicar estos componentes habría que utilizar una API REST.

### Ejercicio 2

**En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?**

Como he explicado en el ejercicio anterior he utilizado SQL en el modelo; HTML, CSS y JavaScript en la vista y PHP en el controlador. Pero si quisiese utilizar distintos lenguajes en el controlador no podría porque está todo muy acoplado.

En cambio si cambiase a una arquitectura tipo microservicios podría usar distintos lenguajes en cada microservicio.

Sería más conveniente utilizar una base de datos de tipo NO-SQL para la transferencia de datos por medio de la API REST mediante el uso de JSON.

---

## Tema 2: Gestión de infraestructuras virtuales

### Ejercicio 1

**Instalar chef en la máquina virtual que vayamos a usar**

```
curl -L https://www.opscode.com/chef/install.sh | sudo bash
```

![Chef Installation](images/chef-installation.png "chef-installation")

---

Volver a [home](index).
