---
layout: default
title: Registro de cambios
navegacion:
  contenido:
    - nombre: "Pendiente de liberación"
      link: "registro-cambios#pendiente-de-liberación"
  versiones:
    - nombre: "2021.04.21"
      link: "registro-cambios#20210421"
    - nombre: "2021.03.04"
      link: "registro-cambios#20210304"
    - nombre: "2021.02.12"
      link: "registro-cambios#20210212"
    - nombre: "2021.01.11"
      link: "registro-cambios#20210111"
    - nombre: "2020.12.22"
      link: "registro-cambios#20201222"
    - nombre: "2020.12.04"
      link: "registro-cambios#20201204"
    - nombre: "2020.11.20"
      link: "registro-cambios#20201120"
    - nombre: "2020.10.26"
      link: "registro-cambios#20201026"
    - nombre: "2020.09.30"
      link: "registro-cambios#20200930"
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

## 2021.04.21
---
### Agregado
- Creación de cartas de devolución a partir de comprobantes almacenados.
- Anulación de cartas de devolución liberando comprobantes asociados.
- Reporte impreso de cartas de devolución.
- Reporte impreso de cartas de devolución resumido.
- Reporte impreso de cartas de devolución detallado.
- Reporte Excel de cartas de devolución.
- Validación de anulación de comprobantes que salieron en al menos un viaje.
- **`[Calico]`** Registro de remito y cantidad procesada en tabla de líneas recibidas en interfaz de Bianchi.
- **`[Calico]`** Actualización de estado de línea recibida según proceso en SAAD en interfaz de Bianchi.
- **`[Calico]`** Proceso de creación de paradas en OptimoCamino con informe de series asociadas a vale de recepción para Telecentro.

### Modificado
- Mejora en importación de archivos Excel de gran tamaño.
- **`[Calico]`** Modificación de proceso de informe de líneas procesadas para que guarde solicitudes enviadas en base de datos en interfaz de Bianchi.
- **`[Calico]`** Modificación de proceso de informe de líneas entregadas para que guarde solicitudes enviadas en base de datos en interfaz de Bianchi.

### Quitado
- **`[Calico]`** Procedimiento almacenado de generación de informes de pedidos procesados en interfaz de Bianchi.

## 2021.03.04
---
### Agregado
- Control de paletas rendidas.
- Control de paletas debitadas a transportistas.
- Control de paletas con vales de recupero.
- Pantalla de rendición de paletas en viajes iniciados o finalizados.
- Manejo de vales de proveedor.
- Nuevo tipo de retiro "Recupero de paletas" para manejo de retiros de recupero de paletas.
- Reporte Excel de paletas a recuperar para retiros del tipo "Recupero de paletas".
- **`[Calico]`** Proceso de cambio de estado de comprobantes como recibidos para Telecentro.

### Modificado
- Carga de remitentes con razón social repetida.
- Carga de clientes sin método de aforo.
- Carga de comprobantes ingresando kilogramos y metros cúbicos si el cliente no tiene asignado un método de aforo.
- Carga de solicitudes de retiro ingresando kilogramos y metros cúbicos si el cliente no tiene asignado un método de aforo.
- **`[Calico]`** Deshabilitación de asignación de datos de transporte inactivos a viajes.
- **`[Calico]`** Marca de agua en reporte impreso estándar de viajes con datos de transporte inactivos.
- **`[Calico]`** Marca de agua en reporte impreso estándar de hojas de ruta con datos de transporte inactivos.
- **`[Calico]`** Logo de cliente en reporte de ordenes de trabajo de Telecentro.
- **`[Calico]`** Piso, departamento y teléfono de destino en reporte de ordenes de trabajo de Telecentro.
- **`[Calico]`** Refactor de proceso de informe de líneas procesadas para Bianchi.

### Corregido
- Ingresos de vales de recepción con productos seriados desde importador Excel.

## 2021.02.12
---
### Agregado
- Columna con cliente y remitente en pantalla de ingreso de turnos.
- Columna con cliente y remitente en pantalla de seguimiento de turnos.
- **`[Plb]`** Tablero de seguimiento de turnos de carga.
- **`[Plb]`** Tablero de seguimiento de turnos de descarga.

### Modificado
- Filtro por defecto con turnos activos en pantalla de ingreso de turnos.
- Filtro por defecto con turnos activos en pantalla de seguimiento de turnos.
- Estados de pedidos visualizados en pantalla de seguimiento turnos de carga.
- Estados de vales de recepción visualizados en pantalla de seguimiento turnos de descarga.
- **`[Calico]`** Asignación de fecha de conforme en tabla TMS_DetalleComprobante al conformar un comprobante pendiente de resolución.
- **`[Calico]`** Asignación de fecha de entrega en tabla TMS_DetalleComprobante al almacenar un comprobante.
- **`[Calico]`** Observación por defecto "Retira cliente" al conformar comprobantes recibidos.

### Corregido
- Inicio de hojas de ruta no emitidas al iniciar viaje.

## 2021.01.11
---
### Agregado
- **`[Calico]`** Pantalla para emisión de reportes impresos de notas de devolución a partir de vales de recepción para cliente Telecentro.
- **`[Calico]`** Interfaz de ingreso de novedades para comprobantes de Telecentro.
- **`[Calico]`** Interfaz de informe de correo electrónico para Raizen.

### Modificado
- Registro de etapa al valorizar viaje.
- Visualización de precio y extra costo en cero en reporte impreso estándar de viajes para viajes anulados.
- Visualización de precio y extra costo en cero en reporte impreso de liquidación de viajes para viajes anulados.
- Visualización de precio y extra costo en cero en reporte impreso de prorrateos de viajes para viajes anulados.
- Visualización de precio y extra costo en cero en reporte Excel estándar de viajes para viajes anulados.
- Visualización de precio y extra costo en cero en reporte Excel de liquidación de viajes para viajes anulados.
- Visualización de unidades en detalle de reporte impreso de notas de devolución.
- Visualización de unidades en detalle de reporte Excel de notas de devolución.

## 2020.12.22
---
### Agregado
- Configuración de validación de emisión de hojas de ruta en viajes iniciados según tipo de viaje.
- Configuración de validación de inicio de viaje con paletas asignadas según tipo de viaje.
- Configuración de validación de finalización de viajes con rendición de paletas según tipo de viaje.
- Configuración de topes en regla de adicionales.
- Filtro de transportes inactivos en carga de viajes

### Modificado
- Mejora de usabilidad en caga de paletas utilizadas por muelle.
- Mejora de usabilidad en caga de paletas utilizadas por viajes.
- Mejoras de performance en integraciones con [OptimoCamino](https://www.optimocamino.com/).

### Corregido
- Redondeo a dos decimales en reporte impreso de adicionales.
- Redondeo a dos decimales en reporte Excel de adicionales.

## 2020.12.04
---
### Agregado
- Consulta de retiros por número de viaje.
- Carga de tipos de adicionales repetidos.

### Modificado
- Calculo de reglas de tipos de adicional por tipo de unidad de acoplado.
- Inicio de viajes con control hojas de ruta y paletas asignadas.

## 2020.11.20
---
### Agregado
- Indicadores visuales de totales asignados a muelle.
- Indicadores visuales de totales asignados a viaje.
- Configuración de formatos en importador Excel.
- Fecha de creación en pantalla de retiros.
- Totales en pantalla de retiros.
- **`[Cic]`** Ingreso y modificación de subclientes desde servicio web.
- **`[Cic]`** Ingreso y modificación de productos desde servicio web.
- **`[Intralog]`** Ingreso de pedidos dese archivos EDI.
- **`[Intralog]`** Informe de pedidos en archivos EDI.
- **`[Klo]`** Ingreso de pedidos desde Excel con formato particular.

### Modificado
- Mejora de usabilidad en caga de paletas utilizadas por muelle.
- Mejora de usabilidad en caga de paletas utilizadas por viajes.
- Mejoras de performance en pantalla de hojas de ruta.
- Valorización de viajes solo al iniciar.
- Creación y modificación de viajes sin calculo de totales.
- Numeración de viajes no bloqueante.
- Carga de devolución con marca en vale de recepción.
- **`[Calico Argentina]`** Reporte impreso de viajes estándar sin extra costo.
- **`[Calico Argentina]`** Reporte impreso de viajes estándar sin columna de paletas.
- **`[Calico Argentina]`** Reporte impreso de viajes estándar con calculo de medidas a paritr de comprobantes asignados a hojas de ruta.
- **`[Calico Argentina]`** Reporte impreso de hojas de ruta estándar sin columna de paletas.

## 2020.10.26
---
### Agregado
- Filtro por ordenes de retiro con comprobantes asignados en consulta de ordenes de retiro.
- Visualización de ordenes de retiro con comprobantes asignados en grilla de ordenes de retiro.
- Filtro por muelles automáticos en consulta de muelles.
- Visualización de muelles automáticos en grilla de muelles.
- Visualización de comprobantes asociados a retiros en detalle de grillas de ordenes de retiro.
- Listado de comprobantes asociados a retiro en detalle de grilla.
- Reporte impreso de extra costos.
- Reporte impreso de prorrateos de viaje.
- Calculo de prorrateos de comprobantes.
- Calculo de prorrateos de retiros.
- Calculo de prorrateos de comprobantes asociados a retiros.
- Interfaz estándar de envío de informes por correo electrónico.
- Configuración de informe por correo electrónico al ejecutar interfaz de movimiento de archivos entre directorios.

### Modificado
- Leyendas de fechas mas descriptivas en reporte impreso de adicionales de viajes.

### Corregido
- Reporte impreso de planillas desfasado al mostrar comprobantes con observaciones muy extensas.
- Filtro de hojas de rutas en viaje devuelve hojas de ruta conformes.

## 2020.09.30
---
### Agregado
- Carga de paletas utilizadas por viajes.
- Seguimiento de interfaces con [OptimoCamino](https://www.optimocamino.com/) desde monitor.
- Proceso automático de movimiento de archivos entre directorios.

### Modificado
- Optimización de performance de pantalla de viajes.
- El reporte impreso estándar de viajes muestra paletas utilizadas.
- El reporte impreso estándar de hojas de ruta muestra paletas utilizadas.
- **`[Calico Argentina]`** El reporte impreso particular de viajes muestra paletas utilizadas.
- **`[Calico Argentina]`** El reporte impreso particular de hojas de ruta muestra paletas utilizadas.

### Quitado
- Finalización automática de viajes.

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