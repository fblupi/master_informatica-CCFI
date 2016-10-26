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

Respuesta

---

Volver a [home](index).
