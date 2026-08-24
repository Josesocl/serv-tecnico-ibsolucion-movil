# Modelo de datos

## Entidad principal: Servicio técnico

Cada envío del formulario representa un servicio técnico realizado o intentado en terreno.

## Campos clave

| Campo | Descripción | Uso |
|---|---|---|
| folio_servicio | Identificador único del servicio | Búsqueda, control y trazabilidad |
| fecha | Fecha de atención | Reportes y filtros |
| cliente | Cliente atendido | Segmentación |
| tecnico_responsable | Técnico a cargo | Control de ejecución |
| tipo_servicio | Tipo de atención | Análisis operacional |
| equipo_tipo | Tipo de equipo | Historial técnico |
| equipo_marca | Marca | Historial técnico |
| equipo_modelo | Modelo | Historial técnico |
| equipo_serie | Número de serie | Trazabilidad por equipo |
| diagnostico | Diagnóstico técnico | Base técnica |
| trabajo_realizado | Actividades ejecutadas | Evidencia del servicio |
| estado_final | Resultado final | Gestión posterior |
| requiere_cotizacion | Sí/No | Oportunidad comercial |
| requiere_nueva_visita | Sí/No | Seguimiento |
| recepcion_conforme | Estado de recepción | Respaldo cliente |

## Tablas sugeridas en Google Sheets

### Respuestas_Jotform

Tabla principal sincronizada desde Jotform. No modificar manualmente salvo necesidad controlada.

### Clientes

Campos sugeridos:

- cliente_id
- nombre_cliente
- rut_cliente
- contacto_principal
- email
- telefono
- direccion
- estado

### Técnicos

Campos sugeridos:

- tecnico_id
- nombre
- email
- telefono
- empresa
- especialidad
- activo

### Equipos

Campos sugeridos:

- equipo_id
- cliente
- tipo_equipo
- marca
- modelo
- numero_serie
- ubicacion
- observaciones

### Repuestos

Campos sugeridos:

- repuesto_id
- descripcion
- unidad
- costo_referencial
- proveedor
- observaciones

### Dashboard

Vista resumida para reportes:

- Servicios por mes.
- Servicios por cliente.
- Servicios por técnico.
- Estados finales.
- Servicios pendientes.
- Cotizaciones requeridas.
- Repuestos requeridos.
