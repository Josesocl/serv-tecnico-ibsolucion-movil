# Configuración Jotform

## Nombre del formulario

**Serv Técnico IBSolucion Móvil**

## Configuración general

- Idioma: Español.
- Diseño: mobile first.
- Logo: IBSolucion.
- Formato recomendado: una pregunta por pantalla o secciones cortas.
- Activar barra de progreso si está disponible.
- Activar envío desde dispositivos móviles.

## Secciones recomendadas

1. Identificación del servicio.
2. Cliente y ubicación.
3. Técnico responsable.
4. Equipo intervenido.
5. Tipo de servicio.
6. Diagnóstico.
7. Evidencias iniciales.
8. Trabajo realizado.
9. Repuestos y materiales.
10. Evidencias finales.
11. Estado final y recomendaciones.
12. Recepción conforme.
13. Firmas.

## Campos críticos

- Fotos antes del servicio.
- Fotos después del servicio.
- Diagnóstico técnico.
- Trabajo realizado.
- Estado final.
- Firma cliente.
- Firma técnico.

## Configuración recomendada para maquinaria

El campo **Tipo de equipo** no debe usar categorías genéricas de soporte TI como Celular, Tablet o Laptop.

Si el formulario fue creado desde una plantilla anterior, borrar o descartar el campo anterior **Tipo de equipo** y crear nuevamente la estructura de maquinaria con tres campos:

1. **Categoría de maquinaria**.
2. **Tipo de equipo - Aluminio y PVC**.
3. **Tipo de equipo - Madera y Tableros**.

### Campo 1: Categoría de maquinaria

Tipo de campo: lista desplegable.

Opciones para pegar en Jotform:

```text
Aluminio y PVC
Madera y Tableros
```

Campo obligatorio: sí.

### Campo 2A: Tipo de equipo - Aluminio y PVC

Tipo de campo: lista desplegable.

Opciones para pegar en Jotform:

```text
Cortadora Mono Cabezal
Cortadora Doble Cabezal
CNC 3 ejes
CNC 4 ejes
CNC 5 ejes
Soldadora Mono cabezal
Soldadora 2 cabezales
Soldadora 4 cabezales
Retestadora fresas
Pantógrafo
Sierra portátil
```

Campo obligatorio: sí, pero solo cuando la categoría seleccionada sea **Aluminio y PVC**.

### Campo 2B: Tipo de equipo - Madera y Tableros

Tipo de campo: lista desplegable.

Opciones para pegar en Jotform:

```text
Seccionadora Horizontal
Seccionadora Vertical
Enchapadora de Cantos
Centro de Mecanizado Nesting
Centro de Mecanizado Barra y Corte
CNC de 2 cabezales
Centro de Perforación
Centro de Corte
Lijadora
```

Campo obligatorio: sí, pero solo cuando la categoría seleccionada sea **Madera y Tableros**.

## Reglas condicionales en Jotform

En Jotform, ir a:

`Configuración → Condiciones → Mostrar/Ocultar campo`

Configurar estas reglas:

### Regla 1

Si:

`Categoría de maquinaria` es igual a `Aluminio y PVC`

Entonces:

- Mostrar `Tipo de equipo - Aluminio y PVC`
- Ocultar `Tipo de equipo - Madera y Tableros`

### Regla 2

Si:

`Categoría de maquinaria` es igual a `Madera y Tableros`

Entonces:

- Mostrar `Tipo de equipo - Madera y Tableros`
- Ocultar `Tipo de equipo - Aluminio y PVC`

### Regla 3

Si:

`Categoría de maquinaria` está vacía

Entonces:

- Ocultar `Tipo de equipo - Aluminio y PVC`
- Ocultar `Tipo de equipo - Madera y Tableros`

## Nombre de campos recomendado para Google Sheets

Para evitar confusión en la planilla, se recomienda usar estos nombres técnicos:

- `categoria_maquinaria`
- `tipo_equipo_aluminio_pvc`
- `tipo_equipo_madera_tableros`

En reportes o dashboards posteriores se puede crear una columna calculada llamada `tipo_equipo_final`, que tome el valor del campo de Aluminio/PVC o Madera/Tableros según corresponda.

## Notificación interna

Destinatario:

`jrjottar@ibsolucion.com`

Asunto sugerido:

`Nuevo Servicio Técnico IBSolucion - {Cliente} - {Fecha}`

Contenido mínimo:

```text
Se ha registrado un nuevo servicio técnico en terreno.

Cliente: {Cliente}
Técnico: {Técnico responsable}
Fecha: {Fecha}
Tipo de servicio: {Tipo de servicio}
Estado final: {Estado final}

Revisar detalle completo en Jotform y Google Sheets.
```

## Autorespuesta al cliente

Activar solo si se captura email del cliente y si el servicio queda cerrado.

Asunto sugerido:

`Recepción Servicio Técnico IBSolucion - {Fecha}`

## Integraciones

### Google Sheets

Conectar el formulario a la planilla:

`Registro_Servicios_Tecnicos_IBSolucion`

Hoja principal:

`Respuestas_Jotform`

### Google Drive

Usar Google Drive como carpeta de respaldo de PDFs, fotos y exportaciones cuando sea posible según el plan disponible.

## Advertencia sobre plan gratuito

El plan gratuito de Jotform puede tener límites de formularios, respuestas mensuales, almacenamiento y envíos. El piloto debe monitorear esos límites durante los primeros servicios reales.
