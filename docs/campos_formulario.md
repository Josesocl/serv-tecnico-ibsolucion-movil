# Campos del formulario

## 1. Identificación del servicio

| Campo | Tipo | Obligatorio | Observación |
|---|---|---:|---|
| Folio servicio | Texto / automático | Sí | Idealmente generado por Jotform |
| Fecha | Fecha | Sí | Fecha del servicio |
| Hora inicio | Hora | Sí | Inicio trabajo en terreno |
| Hora término | Hora | No | Término trabajo en terreno |
| Cliente | Lista desplegable | Sí | Cliente atendido |
| Obra / planta / ubicación | Texto | Sí | Lugar físico del servicio |
| Dirección | Texto | No | Puede usarse si aplica |
| Contacto cliente | Texto | Sí | Persona de contacto |
| Teléfono contacto | Teléfono | No | Contacto terreno |
| Email contacto | Email | No | Para copia al cliente si corresponde |
| Técnico responsable | Lista desplegable | Sí | Técnico o proveedor técnico |

## 2. Equipo intervenido

| Campo | Tipo | Obligatorio | Observación |
|---|---|---:|---|
| Tipo de equipo | Lista desplegable | Sí | Máquina, herramienta, sistema o instalación |
| Marca | Texto | No | Marca equipo |
| Modelo | Texto | No | Modelo equipo |
| Número de serie | Texto | No | Serie si existe |
| Ubicación del equipo | Texto | No | Área, línea, nave, sector |
| Condición inicial | Texto largo | Sí | Estado observado al inicio |

## 3. Tipo de servicio

Opciones sugeridas:

- Preventivo
- Correctivo
- Instalación
- Puesta en marcha
- Inspección técnica
- Garantía
- Capacitación
- Emergencia
- Otro

## 4. Diagnóstico

| Campo | Tipo | Obligatorio | Observación |
|---|---|---:|---|
| Falla reportada | Texto largo | Sí | Lo informado por cliente |
| Diagnóstico técnico | Texto largo | Sí | Evaluación del técnico |
| Riesgos detectados | Texto largo | No | Seguridad, operación, daño potencial |
| Fotos antes | Carga de archivos / cámara | Sí | Evidencia inicial |

## 5. Trabajo realizado

| Campo | Tipo | Obligatorio | Observación |
|---|---|---:|---|
| Actividades realizadas | Texto largo | Sí | Descripción del trabajo |
| Repuestos utilizados | Texto largo / tabla | No | Repuestos o materiales |
| Lubricación aplicada | Sí/No + texto | No | Importante para maquinaria |
| Ajustes realizados | Texto largo | No | Ajustes, calibración, alineación |
| Pruebas realizadas | Texto largo | No | Pruebas de funcionamiento |
| Fotos durante | Carga de archivos / cámara | No | Evidencia intermedia |
| Fotos después | Carga de archivos / cámara | Sí | Evidencia final |

## 6. Estado final

Opciones sugeridas:

- Operativo
- Operativo con observaciones
- No operativo
- Pendiente de repuesto
- Pendiente de cotización
- Pendiente de nueva visita
- Servicio rechazado por cliente

## 7. Recomendaciones

| Campo | Tipo | Obligatorio | Observación |
|---|---|---:|---|
| Requiere nueva visita | Sí/No | Sí | Seguimiento técnico |
| Requiere repuestos | Sí/No | Sí | Compra posterior |
| Requiere cotización adicional | Sí/No | Sí | Venta o servicio futuro |
| Recomendaciones al cliente | Texto largo | No | Uso, mantención, seguridad |
| Observaciones del técnico | Texto largo | No | Comentarios internos |

## 8. Recepción conforme

| Campo | Tipo | Obligatorio | Observación |
|---|---|---:|---|
| Recepción conforme | Lista desplegable | Sí | Conforme / con observaciones / no conforme |
| Nombre receptor cliente | Texto | Sí | Persona que recibe |
| Cargo receptor | Texto | No | Cargo |
| RUT receptor | Texto | No | Identificación Chile |
| Email receptor | Email | No | Copia de respaldo |
| Comentarios del cliente | Texto largo | No | Observaciones de recepción |
| Firma cliente | Firma | Sí | Firma en pantalla |
| Firma técnico | Firma | Sí | Firma del responsable |
