---
layout: default
title: Registro de cambios
navegacion:
  contenido:
    - nombre: "Pendiente de liberación"
      link: "registro-cambios#pendiente-de-liberación"
  versiones:
    - nombre: "2020.09.11"
      link: "registro-cambios#20200911"
    - nombre: "2020.08.31"
      link: "registro-cambios#20200831"
    - nombre: "2020.08.04"
      link: "registro-cambios#20200804"     
---
{% include navegacion.html %}
{% include navegacion-contenido.html %}
# Registro de cambios
---
En este archivo se documentaran todo los cambios notables liberados en cada versión.

El formato esta basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/), y para el nombre de versión se utiliza la fecha de lazamiento de la misma en el formato **AAAA.MM.DD**.

## Pendiente de liberación
---
### Agregado
- Modulo de seguimiento de paletas.
- Seguimiento de interfaces con [OptimoCamino](https://www.optimocamino.com/) desde monitor
- **`[Calico Argentina]`** Seguimiento de interfaces con [Wirsolut](https://www.wirsolut.com/) desde monitor.

## 2020.09.11
---
### Agregado
- Carga de paletas utilizadas por viajes.

### Modificado
- Optimización de performance de pantalla de viajes.

## 2020.08.31
---
### Agregado
- Proceso de conforme de ordenes de retiro.
- Maestro de tipos de paleta.
- Carga de paletas utilizadas por muelles.

### Modificado
- Optimización de performance de pantalla de muelles.
- Los datos de vehículo y chofer en el ingreso de turnos son de carga libre y no se validan contra los maestros del modulo de flota.

## 2020.08.04
---
### Modificado
- El proceso de valorización de viajes muestra un mensaje con el motivo por el cual no se pudo valorizar en caso de error.
- El tipo de viaje permite indicar si el viaje tiene retorno.
- La carga de viajes completa el origen y destino del viaje con la sucursal en la que esta logueado el usuario si el tipo de viaje seleccionado tiene retorno.
- La empresa de transporte permite configurar si se mostrara el valor del viaje en los reportes.
- El reporte impreso estándar de viajes muestra el valor del viaje dependiendo de la parametrización de la empresa de transporte.
- **`[Calyco Uruguay]`** El reporte impreso particular de viajes muestra fecha y hora estimada de carga del viaje.
- **`[Calyco Uruguay]`** El reporte impreso particular de viajes muestra la observación del viaje.
- **`[Calyco Uruguay]`** El reporte impreso particular de liquidación de transportistas muestra el rango de fechas de emisión utilizadas en el filtro de la consulta de viajes.

### Correcciones
- Selección de roles en pantalla de carga de usuario.
- Mejoras de performance en inicio masivo de viajes.
- Mejoras de performance en valorización masiva de viajes. 