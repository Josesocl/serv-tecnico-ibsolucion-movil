# Serv Técnico IBSolucion Móvil

Proyecto piloto para implementar un formulario móvil de servicio técnico en terreno para IBSolucion.

La solución está pensada para técnicos que realizan visitas a clientes, registran diagnóstico, trabajo realizado, evidencias fotográficas, repuestos, estado final del equipo y recepción conforme del cliente.

## Objetivo

Construir una solución operativa simple, sin costos adicionales iniciales, usando:

- Jotform como formulario móvil.
- Google Sheets como base de datos operativa.
- Google Drive como respaldo de evidencias, PDFs y documentos.
- GitHub como respaldo técnico y control de versiones del diseño funcional.

## Nombre del formulario

**Serv Técnico IBSolucion Móvil**

## Alcance inicial

El piloto debe permitir:

1. Registrar servicios técnicos desde celular.
2. Tomar fotografías antes, durante y después del servicio.
3. Registrar diagnóstico técnico y trabajo realizado.
4. Registrar repuestos, materiales y recomendaciones.
5. Capturar firma del cliente y del técnico.
6. Generar respaldo automático en Jotform.
7. Enviar notificación por email a `jrjottar@ibsolucion.com`.
8. Sincronizar respuestas con Google Sheets.
9. Mantener respaldo documental del proyecto en GitHub.

## Cliente

El formulario es genérico para IBSolucion. No debe quedar asociado a un cliente específico como ALUDOM, aunque ALUDOM puede ser uno de los clientes seleccionables en el formulario.

## Estructura del repositorio

```text
README.md
docs/
  alcance_funcional.md
  campos_formulario.md
  flujo_operativo.md
  modelo_datos.md
  checklist_piloto.md
  configuracion_jotform.md
  configuracion_google_sheets.md
templates/
  email_servicio_tecnico.md
  recepcion_conforme.md
  estructura_pdf_servicio.md
exports/
  google_sheets_headers.csv
  jotform_campos_base.json
assets/
  logo_ibsolucion.jpg
changelog.md
```

## Estado del proyecto

Versión inicial documental para configurar el piloto operativo en Jotform y Google Sheets.
