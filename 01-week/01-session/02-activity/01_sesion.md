# Documentación Sesión 1 - Week 01

## 1. Objetivo
Documentar el flujo de trabajo de ramas, commits y Merge Requests (MR) entre ambientes.

---

## 2. Estructura de la rama
Se trabajo acerca de como estructurar las ramas en nuestro repositorio.
La plantilla para estructurar las ramas es la siguiente:
<tipo-trabajo>/<stack>/HU-<id>-<ambiente>[-breve-descripcion]

Tambien se hablo de los diferentes tipos de campos que se pueden usar en el nombre de la rama:
-data-base
-doc
-HU
-feature

## 3. Flujo de trabajo
### 3.1. Conventional Commits
Es un formato  convencional el cual nos dice como crear un comentario para que sea entendido mejor para el grupo de trabajo.

Formato general:

```
<tipo> (<alcance>): <descripcion corta(HU-<id>) <descripcion detallada>
```
El **tipo** se puede elegir entre los siguientes:

- feat:
- fix
- docs
- refactor ...
 El **alcance** se puede elegir entre los siguientes:
 - app-mobile
 - backend
 - database
 - docs
### 3.2.Ejemplo
git commit -m "feat(frontend): add new feature"

## 4. MR
### 4.1. Concepto
Un merge request es una solicitud para integrar cambios de una rama  a otra permitiendo revision antes de fusionar.

### 4.2.Tipos de ambientes
#### 4.2.1. Dev
Es el ambiente de desarrollo donde se realizan los cambios y se integran nuevas funcionalidades.

#### 4.2.2. QA
Es el ambiente donde se revisan y  validan que la funcionalidad  cumpla con los requesistos.

#### 4.2.3. Testing
Es el ambiente de pruebas donde se corrigen  y detectan  problemas que no se vieron en QA.Es la parte donde se realizan pruebas mas profundas

#### 4.2.4.Main
Es la versión estable de còdigo-versión confiable que luego pasará a producción.

#### 4.2.5. Project
Es un ambiente donde se integran todas las funcionalidades del proyecto completo.Su objetivo e shacer que todo el proyecto funcione bien antes de  pre-producción.

### 4.2.5 Staging
Es ultimo ambiente de prueba antes de producción.Su objetivo es validar que la versión final que llegará a producción funcione bien.

### 4.2.6 Production
Los cambios llegan  a los usuarios finales.Se entrega la funcionalidad de manera segura  y estable a los usuarios.

## 5. Tipos de MR (Merge Request)
Feature: Añadir una nueva funcionalidad o característica.

Bugfix: Corregir un error o fallo en el código existente.

Hotfix: Corrección urgente de un error en producción.

Refactor: Cambios internos en el código sin afectar su funcionamiento.

Chore: Tareas de mantenimiento, configuración o limpieza de código.

Spike: Investigación o experimento corto para explorar soluciones.

 ## 6.Roles / Seguridad
Gestión de permisos: Controla quién puede leer, escribir o aprobar cambios en el repositorio.

Revisiones: Otros miembros revisan los cambios antes de hacer merge (evita errores).

Control de cambios: Registro de qué se cambió, quién lo hizo y cuándo, para mantener trazabilidad y orden.