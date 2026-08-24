# Configuración Google Sheets

## Planilla principal

Nombre sugerido:

`Registro_Servicios_Tecnicos_IBSolucion`

## Ubicación sugerida en Drive

`IBSOLUCION / Serv Técnico IBSolucion Móvil / 02_Respuestas`

## Hojas recomendadas

1. `Respuestas_Jotform`
2. `Clientes`
3. `Técnicos`
4. `Equipos`
5. `Repuestos`
6. `Dashboard`

## Hoja Respuestas_Jotform

Debe ser alimentada automáticamente por Jotform.

Recomendación: no modificar columnas directamente si están sincronizadas desde Jotform.

## Hoja Clientes

Usar para normalizar nombres de clientes y evitar errores de digitación.

Columnas sugeridas:

- cliente_id
- nombre_cliente
- rut_cliente
- contacto_principal
- email
- telefono
- direccion
- estado

## Hoja Técnicos

Columnas sugeridas:

- tecnico_id
- nombre
- email
- telefono
- empresa
- especialidad
- activo

## Hoja Equipos

Columnas sugeridas:

- equipo_id
- cliente
- tipo_equipo
- marca
- modelo
- numero_serie
- ubicacion
- observaciones

## Hoja Repuestos

Columnas sugeridas:

- repuesto_id
- descripcion
- unidad
- costo_referencial
- proveedor
- observaciones

## Hoja Dashboard

Indicadores sugeridos:

- Total servicios.
- Servicios por mes.
- Servicios por cliente.
- Servicios por técnico.
- Servicios pendientes.
- Servicios con cotización adicional.
- Servicios con repuestos requeridos.
- Servicios no conformes.
