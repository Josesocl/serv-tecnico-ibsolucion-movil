# Flujo operativo

## Flujo principal

1. El técnico recibe el link del formulario Jotform en su celular.
2. Abre el formulario **Serv Técnico IBSolucion Móvil**.
3. Registra datos del servicio, cliente, contacto y equipo.
4. Toma fotografías iniciales desde la cámara del celular.
5. Registra diagnóstico técnico.
6. Ejecuta el servicio.
7. Registra trabajo realizado, repuestos, ajustes, lubricación y pruebas.
8. Toma fotografías finales.
9. Informa recomendaciones o pendientes.
10. Cliente revisa y firma recepción conforme en pantalla.
11. Técnico firma.
12. Técnico envía el formulario.
13. Jotform guarda el registro.
14. Se envía email automático a `jrjottar@ibsolucion.com`.
15. La respuesta se sincroniza con Google Sheets.
16. Los respaldos quedan disponibles para consulta posterior.

## Flujo con servicio pendiente

Cuando el equipo queda pendiente de repuesto, cotización o nueva visita:

1. El técnico selecciona el estado final correspondiente.
2. Registra qué repuesto, cotización o acción se requiere.
3. Adjunta fotos que justifiquen el pendiente.
4. Cliente firma recepción conforme con observaciones.
5. Se genera respaldo para preparar cotización o nueva visita.

## Flujo de cierre conforme

1. Equipo queda operativo.
2. Técnico registra pruebas realizadas.
3. Cliente recibe el trabajo.
4. Cliente firma conforme.
5. Registro queda cerrado en Sheets con estado `Operativo` o `Operativo con observaciones`.

## Flujo de respaldo

- Jotform: registro original del envío.
- Email: aviso automático y copia operativa.
- Google Sheets: base de datos consolidada.
- Google Drive: respaldo de archivos, fotos y PDFs si se configura.
- GitHub: documentación funcional, estructura de campos y control de versiones.
