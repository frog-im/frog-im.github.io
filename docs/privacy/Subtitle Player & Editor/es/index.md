---
title: Política de privacidad | Subtitle Tool
description: Política de privacidad de Subtitle Tool (Subtitle Player & Editor) - Español
lang: es
last_updated: 2026-03-11
---

# Política de privacidad (Subtitle Tool / Subtitle Player & Editor)

- **Nombre de la app:** Subtitle Player & Editor (también denominado **Subtitle Tool** en esta Política)
- **Desarrollador:** frog-im
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Fecha de entrada en vigor:** 2026-03-11

> Esta Política se ha elaborado con referencia a las leyes aplicables, incluidas la Ley de Protección de la Información Personal de Corea (PIPA), el GDPR / UK GDPR, la FADP suiza y las leyes estatales de privacidad pertinentes de EE. UU. Si se aplican normas locales obligatorias, dichas normas prevalecerán.

---

## 1. Finalidad y alcance

Esta app ofrece:

- Reproducción y edición de subtítulos
- Reproducción de video + subtítulos a partir de archivos seleccionados por el usuario
- Superposición flotante de subtítulos / letras mostrada sobre otras apps en Android

La gestión de subtítulos compatible puede incluir formatos como:

- `srt`
- `vtt`
- `ass`
- `ssa`
- `lrc`
- `txt`

La app **no** crea una cuenta de usuario y **no** sube los archivos de subtítulos o multimedia del usuario a los servidores propios del desarrollador. El análisis, la edición, la vista previa de subtítulos y la mayor parte del procesamiento relacionado con la reproducción se realizan **localmente en el dispositivo**.

Sin embargo, para publicidad, gestión del consentimiento y cumplimiento legal, SDK de terceros como **Google Mobile Ads SDK (AdMob)** y **Google UMP** pueden procesar cierta información, como identificadores publicitarios, señales del dispositivo y opciones de consentimiento.

---

## 2. Categorías de información que procesamos

### 2-1) Archivos seleccionados explícitamente por el usuario

La app interactúa con archivos que el usuario selecciona explícitamente, incluidos:

- **Archivos de subtítulos**
  - Ejemplos: `.srt`, `.vtt`, `.ass`, `.ssa`, `.lrc`, `.txt`
  - Usos:
    - Reproducción de subtítulos dentro de la app
    - Edición de subtítulos
    - Visualización de subtítulos en superposición
    - Conversión y exportación de subtítulos

- **Archivos multimedia**
  - Ejemplos: archivos locales de video o audio elegidos por el usuario
  - Usos:
    - Reproducción de video + subtítulos
    - Alineación de tiempo de la superposición con el contenido multimedia que se está reproduciendo

Puntos importantes:

- Los archivos seleccionados por el usuario se procesan localmente en el dispositivo.
- La app no sube esos archivos a los servidores propios del desarrollador.
- Las rutas y los contenidos de los archivos se utilizan únicamente para reproducción, superposición, edición, guardado y acciones solicitadas por el usuario.

### 2-2) Configuración local y valores almacenados

Para proporcionar ajustes persistentes y restaurar el estado anterior, la app almacena algunos valores localmente en el dispositivo mediante `SharedPreferences` o almacenamiento local similar proporcionado por el sistema operativo.

Estos valores no se envían a los servidores propios del desarrollador y normalmente se eliminan si se borran los datos de la app o si la app se desinstala.

#### (1) Ajustes de superposición

Los ejemplos incluyen:

- `overlay_box_x`
- `overlay_box_y`
- `overlay_text_font`
- `overlay_text_color`
- `overlay_outline_enabled`
- `overlay_outline_color`
- `overlay_outline_width`
- `overlay_force_landscape`
- `overlay_interstitial_count`

Finalidad:

- Restaurar la posición de la superposición
- Restaurar el estilo de subtítulos para la superposición y la reproducción de subtítulos dentro de la app
- Mantener preferencias de contorno / fuente / orientación
- Controlar la lógica de frecuencia de visualización de anuncios en algunos flujos relacionados con la superposición

#### (2) Posiciones recientes de reproducción o superposición

Los ejemplos incluyen:

- `overlay_recent_positions`
- `video_subtitle_recent_position`

Finalidad:

- Restaurar o sugerir posiciones recientes de inicio de subtítulos/superposición
- Reanudar la reproducción de video + subtítulos de forma más cómoda

#### (3) Valores de preferencias de publicidad y privacidad

Los ejemplos pueden incluir:

- `pref_npa_always`
- `pref_us_rdp`
- `pref_child_directed`
- `pref_under_age`
- `pref_max_ad_rating`

Finalidad:

- Almacenar opciones de privacidad publicitaria
- Aplicar la configuración de privacidad y anuncios de UMP / AdMob

#### (4) Salida de subtítulos creada por el usuario

Cuando el usuario guarda o exporta archivos de subtítulos, la app puede escribir nuevos archivos de subtítulos en una ubicación seleccionada por el usuario, como por ejemplo:

- Descargas
- Otra carpeta seleccionada mediante el selector del sistema
- Una ubicación de almacenamiento gestionada por el usuario

Estos archivos guardados por el usuario pueden permanecer en el dispositivo después de eliminar la app, a menos que el usuario los elimine manualmente.

#### (5) Archivos temporales y cachés

La app y las bibliotecas de terceros pueden crear archivos temporales o de caché para el funcionamiento normal, como:

- datos de caché del selector de archivos
- datos temporales de conversión de subtítulos
- datos de caché relacionados con la reproducción

Están destinados únicamente al funcionamiento local y no se suben a los servidores propios del desarrollador.

#### (6) Caché del estado de consentimiento de UMP

En las regiones donde se aplica Google UMP, el SDK puede almacenar en caché localmente en el dispositivo el estado de consentimiento.

Por lo general, esto puede restablecerse mediante:

- la eliminación de los datos de la app, o
- el cambio de las opciones de consentimiento dentro de la app cuando haya una entrada disponible de opciones de privacidad

### 2-3) Procesamiento relacionado con la superposición de Android y los permisos

En Android, la superposición flotante de subtítulos puede utilizar:

- permiso `SYSTEM_ALERT_WINDOW` / mostrar sobre otras apps
- permiso `POST_NOTIFICATIONS`
- una notificación de servicio en primer plano requerida para el servicio de superposición

Finalidad:

- mostrar la superposición de subtítulos sobre otras apps
- mantener el servicio de superposición en funcionamiento
- permitir que Android muestre las notificaciones necesarias de superposición / servicio
- leer información de notificaciones multimedia cuando sea necesario para el soporte del avance de subtítulos

Estos permisos se utilizan únicamente para funciones de la app que el usuario elige usar.

### 2-4) Anuncios, consentimiento y datos relacionados (SDK de terceros)

La app utiliza SDK de anuncios / consentimiento de Google, incluidos:

- **Google Mobile Ads SDK (AdMob)**
- **Google UMP**

La app puede mostrar:

- anuncios de banner
- anuncios intersticiales
- anuncios recompensados o intersticiales recompensados

Estos SDK pueden procesar datos como:

- identificadores publicitarios (por ejemplo, AAID / IDFA cuando corresponda)
- información basada en IP y relacionada con la red
- metadatos del dispositivo y de la app
- señales de interacción con anuncios
- opciones de consentimiento

Las finalidades pueden incluir:

- entrega de anuncios
- medición y elaboración de informes publicitarios
- limitación de frecuencia
- prevención del fraude
- cumplimiento legal

El desarrollador procura configurar estos SDK de forma coherente con las opciones de consentimiento del usuario y la ley aplicable.

---

## 3. Cómo procesamos y conservamos los datos

- **Configuraciones locales y datos de posiciones recientes**
  - se conservan en el dispositivo hasta que se borran los datos de la app o se elimina la app

- **Archivos temporales / caché**
  - se conservan solo mientras sea necesario para el funcionamiento y luego la app los elimina cuando es práctico, o el sistema operativo los limpia más adelante

- **Archivos de subtítulos guardados por el usuario**
  - permanecen en la ubicación de guardado elegida por el usuario hasta que este los elimine

- **Datos de anuncios / consentimiento gestionados por terceros**
  - se conservan de acuerdo con las políticas de Google y la ley aplicable

---

## 4. Tratamiento por terceros y transferencias transfronterizas

Para anuncios y gestión del consentimiento, cierta información puede ser procesada por Google y socios relacionados.

| Elemento | Detalles |
|---|---|
| Destinatario | Google LLC y filiales / encargados del tratamiento relacionados |
| Finalidad | Entrega de anuncios, medición, prevención del fraude, gestión del consentimiento y cumplimiento legal |
| Posibles datos | Identificadores publicitarios, información del dispositivo/app, información basada en IP, datos de interacción con anuncios, estado de consentimiento |
| Destino | Estados Unidos y otras regiones donde opera la infraestructura de Google |
| Conservación | De acuerdo con las políticas de Google y la ley aplicable |

El desarrollador procura mantener las divulgaciones de privacidad de la tienda de apps coherentes con el comportamiento real de los SDK.

---

## 5. Sus derechos y opciones

Dependiendo de su jurisdicción, puede tener derechos como:

- acceso
- rectificación
- supresión
- limitación
- portabilidad
- oposición
- retirada del consentimiento cuando el consentimiento sea la base legal

Los controles prácticos incluyen:

- cambiar las opciones de anuncios / privacidad dentro de la app cuando estén disponibles
- borrar los datos de la app para eliminar configuraciones locales y preferencias en caché
- desinstalar la app
- eliminar manualmente los archivos de subtítulos exportados del almacenamiento del usuario
- utilizar controles del sistema operativo, como ajustes de notificaciones, restablecimiento del ID publicitario o ajustes de personalización de anuncios

Para los datos procesados por Google, los usuarios también deben consultar, cuando corresponda, las propias herramientas de privacidad y cuenta de Google.

---

## 6. Privacidad infantil

Esta app no está destinada principalmente a niños.

Su finalidad principal es la reproducción y edición de subtítulos, la visualización en superposición y funciones utilitarias relacionadas. Cuando corresponda, la configuración de los SDK publicitarios puede aplicar indicadores relacionados con la edad o dirigidos a menores, de conformidad con los requisitos de la plataforma y la configuración del desarrollador.

---

## 7. Medidas de seguridad

Dentro de los límites de la arquitectura de la app, el desarrollador procura:

- minimizar la recopilación manteniendo la mayor parte del procesamiento de subtítulos y multimedia en el dispositivo
- utilizar selectores de archivos del sistema y acceso a archivos iniciado por el usuario
- utilizar los permisos del sistema de forma transparente
- apoyarse en el transporte de red cifrado utilizado por los SDK de terceros, cuando corresponda

Ningún método de almacenamiento o transmisión es completamente seguro, pero la app está diseñada para evitar una recopilación innecesaria por parte del desarrollador.

---

## 8. Software de código abierto

La app utiliza software de código abierto, incluidas bibliotecas relacionadas con:

- análisis y serialización de subtítulos
- selección de archivos
- preferencias locales
- ventanas de superposición
- reproducción de video
- WebView

Los avisos de código abierto están disponibles dentro de la app. Para algunos componentes, la app puede utilizar una copia modificada localmente de un paquete de código abierto, conservando el aviso de licencia original.

---

## 9. Contacto

Si tiene preguntas o solicitudes relacionadas con la privacidad:

- **Correo electrónico:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Incluya el nombre de la app **Subtitle Player & Editor** en su mensaje.

---

## 10. Cambios en esta Política

Esta Política puede actualizarse si:

- cambian las funciones de la app
- cambian los permisos o el uso de SDK
- cambian los requisitos legales o de la plataforma

Los cambios materiales se reflejarán en la página actualizada de la política y, cuando corresponda, en la app.
