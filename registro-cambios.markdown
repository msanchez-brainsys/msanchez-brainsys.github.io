---
layout: default
title: Registro de cambios
---
# Registro de cambios
---
En este archivo se documentaran todo los cambios notables liberados en cada versión.

El formato esta basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/), y para el nombre de versión se utiliza la fecha de lazamiento de la misma en el formato **AAAA.MM.DD**.

## Pendiente de liberación
---
### Agregado
- Proceso de conforme de ordenes de retiro.
- Modulo de seguimiento de paletas.
- **`[Calico Chile]`** Interfaz particular que envia informe Excel por correo electronico de stock y kardex no seriado de DirecTv.

### Modificado
- Los datos de vehiculo y chofer en el ingreso de turnos son de carga libre y no se validan contra los maestros del modulo de flota.

## 2020.08.04
---
### Modificado
- El proceso de valorización de viajes muestra un mensaje con el motivo por el cual no se pudo valorizar en caso de error.
- El tipo de viaje permite indicar si el viaje tiene retorno.
- La carga de viajes completa el origen y destino del viaje con la sucursal en la que esta logueado el usuario si el tipo de viaje seleccionado tiene retorno.
- La empresa de transporte permite configurar si se mostrara el valor del viaje en los reportes.
- El reporte impreso estándar de viajes muestra el valor del viaje dependiendo de la parametrización de la empresa de transporte.
- **`[Calyco Uruguay]`** El reporte impreso particual de viajes muestra fecha y hora estimada de carga del viaje.
- **`[Calyco Uruguay]`** El reporte impreso particual de viajes muestra la observación del viaje.
- **`[Calyco Uruguay]`** El reporte impreso particual de liquidación de transportistas muestra el rango de fechas de emisión utilizadas en el filtro de la consulta de viajes.