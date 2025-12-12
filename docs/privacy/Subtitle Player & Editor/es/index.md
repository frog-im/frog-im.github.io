---
title: Política de Privacidad | Subtitle Tool
description: Política de privacidad de Subtitle Player & Editor (Subtitle Tool)
lang: es
last_updated: 2025-12-12
---

# Política de Privacidad (Subtitle Player & Editor / «Subtitle Tool»)

- **Nombre de la app:** Subtitle Player & Editor (en esta Política, «Subtitle Tool»)  
- **Desarrollador:** frog-im  
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)  
- **Fecha de entrada en vigor:** 2025-12-12  

> Esta Política se redacta tomando como referencia leyes aplicables como la Ley de Protección de Información Personal de Corea (PIPA), el RGPD/UK RGPD, la ley suiza FADP y diversas leyes de privacidad de estados de EE. UU.  
> Si existieran requisitos específicos por jurisdicción, dichos requisitos prevalecerán sobre lo aquí establecido.

---

## 1. Finalidad y Alcance

Esta app ofrece funciones de **edición de metadatos de archivos de audio** (título, artista, etc.) almacenados en el dispositivo y una función de **superposición de letras/subtítulos**.  
La app **no crea una cuenta de usuario** y **no sube el contenido del usuario a ningún servidor**. El tratamiento se realiza **en el propio dispositivo** por defecto.

Sin embargo, para fines de **publicidad** y **cumplimiento legal**, socios terceros (por ejemplo, Google Mobile Ads SDK (AdMob) y UMP) pueden recopilar y tratar información como **identificadores publicitarios**.  
La recogida de consentimientos y la gestión de opciones de privacidad siguen las especificaciones de **Google UMP (User Messaging Platform)**.

---

## 2. Categorías de Información que Tratamos

### 2-1) Archivos seleccionados explícitamente por el usuario

- **Rutas y contenido de audio/portadas:** se tratan **localmente** en el dispositivo, exclusivamente para editar y guardar.  
- Se utiliza **FFmpegKit** localmente para codificación, edición de metadatos y extracción de miniaturas.  
- La app **no sube** estos archivos seleccionados por el usuario a nuestros servidores.

### 2-2) Ajustes locales y valores almacenados

Para la funcionalidad básica y la comodidad del usuario, la app guarda los siguientes valores **localmente en el dispositivo**.  
Estos datos no se envían a nuestros servidores y se **eliminan cuando se borra la app o sus datos**.

#### (1) Preferencias (`shared_preferences`)

| Tipo | Clave/Contenido | Finalidad | Almacenamiento | Eliminación |
|---|---|---|---|---|
| Posición/tamaño de superposición y fuente | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar posición de la superposición y tamaño de fuente | SharedPreferences del dispositivo | Se elimina al borrar los datos de la app o desinstalarla |
| Configuración de anuncios/privacidad | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Anuncios no personalizados, señal U.S. RDP, etiqueta COPPA, etiqueta de edad, límite de clasificación de contenido publicitario | SharedPreferences del dispositivo | Igual que a la izquierda |

#### (2) Archivos temporales (directorio temporal del sistema)

- **Ejemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Uso:** extracción de portadas, etiquetado FLAC, codificación temporal  
- **Ubicación:** carpeta temporal del sistema operativo (`systemTemp`)  
- **Retención:** la app intenta borrarlos tras finalizar el procesamiento; también pueden eliminarse mediante tareas de limpieza del sistema operativo.

#### (3) Guardado elegido por el usuario (SAF)

- Cuando el usuario utiliza «Guardar como», los archivos de audio finales pueden escribirse en ubicaciones que el usuario elija (por ejemplo, Descargas, almacenamiento en la nube).  
- Estos archivos se almacenan en **almacenamiento externo** y **pueden permanecer tras desinstalar la app**. El usuario puede eliminarlos manualmente.

#### (4) Estado de consentimiento (caché de UMP)

- En las regiones EEE/Reino Unido/Suiza, el SDK UMP **almacena en caché el estado de consentimiento de anuncios del usuario de forma local**.  
- Se puede restablecer borrando los datos de la app o desde la pantalla de **Opciones de privacidad** dentro de la app (cuando esté disponible).

---

### 2-3) Datos relacionados con anuncios y consentimiento (SDK de terceros)

- **Google Mobile Ads SDK (AdMob) y UMP** pueden recopilar y tratar, por ejemplo: **identificadores publicitarios (AAID/IDFA)**, **rangos de IP**, **información de dispositivo/app**, **señales de interacción con anuncios**, **estado de consentimiento**, etc.  
- **Finalidades:** entrega de anuncios, limitación de frecuencia, prevención de fraude, medición del rendimiento, cumplimiento legal.  
- **Regiones que requieren consentimiento (EEE/Reino Unido/Suiza):** el consentimiento se recoge mediante pantallas de UMP y se ofrece una pantalla de **Opciones de privacidad** cuando así se exige.  
  En regiones sin dichos requisitos (por ejemplo, Corea), esta opción **puede no mostrarse**.

---

## 3. Tratamiento y Retención

- **Ajustes locales:** se almacenan en el dispositivo hasta que el usuario borra los datos de la app o la desinstala.  
- **Archivos temporales:** se crean durante la codificación/extracción y se eliminan tras el procesamiento, o pueden permanecer de forma temporal como parte de la caché del sistema.  
- **Datos de anuncios/consentimiento (terceros):** se conservan y eliminan de acuerdo con las **políticas de Google**.

---

## 4. Transferencias a Terceros y Flujos Transfronterizos

Para publicidad y gestión del consentimiento, cierta información del usuario puede transmitirse y tratarse en infraestructuras de Google.

| Elemento | Detalles |
|---|---|
| **Destinatario** | Google LLC y sus filiales/subencargados |
| **Destino** | Estados Unidos (y otras regiones donde se aloja la infraestructura de Google) |
| **Finalidad** | Entrega de anuncios, medición y rendimiento, cumplimiento legal, gestión de consentimiento |
| **Datos** | Identificadores publicitarios, rangos de IP, info de dispositivo/app, interacciones con anuncios, estado de consentimiento, etc. |
| **Retención** | Según las políticas de Google |
| **Efecto de la negativa** | Es posible que se limiten los anuncios personalizados; se pueden mostrar anuncios no personalizados |

Cumplimos los requisitos de **“Seguridad de datos” de Google Play** y mantenemos las declaraciones alineadas con el tratamiento real.

---

## 5. Sus Derechos y Cómo Ejercerlos

- **Exclusión de anuncios personalizados / cambio de consentimiento**  
  - En regiones admitidas (EEE/Reino Unido/Suiza): puede cambiar sus preferencias en **Ajustes → Opciones de privacidad**.  
  - En otras regiones: puede utilizar los ajustes del sistema operativo para **restablecer el ID publicitario / limitar el seguimiento de anuncios**.
- **Restablecimiento de información local:** al borrar los datos de la app o desinstalarla se restablecen las coordenadas de superposición, el tamaño de la fuente y otros ajustes locales.  
- Los derechos previstos en **RGPD/UK RGPD/FADP suiza/leyes estatales de EE. UU.** (acceso, rectificación, supresión, portabilidad, limitación, retirada del consentimiento, etc.) podrán ejercerse en la medida en que dichas leyes lo establezcan.  
  Para los datos publicitarios tratados por Google, use los **procedimientos de Google**.

---

## 6. Privacidad de Menores

Esta app **no está dirigida a menores**.  
Si un menor por debajo de la edad mínima legal utiliza la app, debe dejar de utilizarla y emplear, junto con su tutor, las funciones de limitación de anuncios del sistema operativo.  
Cuando proceda, podremos aplicar etiquetas como **TFUA (child-directed tag)** u opciones similares de protección infantil.

---

## 7. Medidas de Seguridad

- **Minimización de datos** en la recopilación y el almacenamiento  
- Uso limitado de archivos temporales y eliminación tras el procesamiento cuando sea posible  
- Tratamiento exclusivamente **dentro del ámbito de permisos del sistema operativo**  
- Cifrado **TLS o equivalente** durante la transmisión a terceros (según los estándares de los SDK)

---

## 8. Seguridad de Datos (Google Play)

Preparamos y mantenemos la sección de **Seguridad de datos** en Play Console de forma precisa y la actualizamos con prontitud cuando hay cambios.

---

## 9. Avisos de Código Abierto

La app utiliza software de código abierto, como **FFmpeg**.  
Dentro de la app se incluye un archivo informativo (por ejemplo, `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) que explica cómo obtener el código fuente.  
Si lo solicita, proporcionaremos el código fuente conforme a las indicaciones de dicho archivo.

---

## 10. Contacto

- Correo electrónico: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Cambios en Esta Política

Podremos modificar esta Política debido a cambios legales o del servicio.  
Publicaremos las actualizaciones **dentro de la app** y en esta **página de política**.  
En caso de cambios materiales, proporcionaremos un aviso **al menos 7 días antes** de la fecha efectiva.
