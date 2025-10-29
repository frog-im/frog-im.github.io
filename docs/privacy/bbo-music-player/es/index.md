---
title: Política de Privacidad | Lyrics Overlay & Tag Editorr
description: Política de Privacidad de Lyrics Overlay & Tag Editorr (Español)
lang: es
last_updated: 2025-10-30
---

# Política de Privacidad (Lyrics Overlay & Tag Editorr)

- **Nombre de la app:** Lyrics Overlay & Tag Editorr  
- **Desarrollador:** frog-im  
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Fecha de entrada en vigor:** 2025-10-30

> Esta Política se ha elaborado con referencia a las leyes aplicables, incluidas la Ley de Protección de la Información Personal de Corea (PIPA), el RGPD/UK GDPR, la LPD suiza y las leyes estatales de privacidad de EE. UU. Cuando existan requisitos específicos por jurisdicción, estos tendrán prioridad.

---

## 1. Finalidad y alcance del tratamiento

Esta app ofrece **edición de metadatos** (título, artista, etc.) de archivos de audio **almacenados en el dispositivo**, y una **superposición de letras**.  
La app **no** crea cuentas de usuario ni **sube** contenidos del usuario a servidores propios. El tratamiento se realiza **por defecto en el dispositivo del usuario**.

No obstante, para **publicidad** y **cumplimiento legal**, socios de terceros (p. ej., Google Mobile Ads SDK (AdMob), UMP) pueden recopilar y tratar información como **identificadores publicitarios**. La obtención del consentimiento y las opciones de privacidad siguen las especificaciones de la **Plataforma de Mensajes al Usuario de Google (UMP)**.

---

## 2. Categorías de información tratada

### 2-1) Archivos seleccionados explícitamente por el usuario
- **Rutas y contenido de audio/imagen de portada:** se tratan **localmente** en el dispositivo únicamente para editar/guardar.  
- **FFmpegKit** se usa localmente para codificación, edición de metadatos y extracción de miniaturas.  
- La app **no sube** los archivos seleccionados por el usuario a nuestros servidores.

### 2-2) Ajustes locales y valores almacenados

Para el funcionamiento y la comodidad del usuario, la app guarda los siguientes valores **localmente en el dispositivo**.  
Estos valores no se envían a nuestros servidores y **se eliminan al borrar los datos de la app o al desinstalarla**.

#### (1) Preferencias (`shared_preferences`)
| Tipo | Clave/Contenido | Finalidad | Almacenamiento | Eliminación |
|---|---|---|---|---|
| Posición/fuente del overlay | `overlay_box_x`, `overlay_box_y`, `overlay_text_font` | Restaurar la posición del overlay y el tamaño de fuente | SharedPreferences del dispositivo | Se elimina al borrar datos o desinstalar |
| Publicidad/Privacidad | `pref_npa_always`, `pref_us_rdp`, `pref_child_directed`, `pref_under_age`, `pref_max_ad_rating` | Anuncios no personalizados, RDP en EE. UU., etiqueta COPPA, etiqueta de edad, límite de calificación de contenido publicitario | SharedPreferences del dispositivo | Igual que a la izquierda |

#### (2) Archivos temporales (directorio temporal del sistema)
- **Ejemplos:** `cover_*.jpg`, `tmp_*.flac`  
- **Uso:** extracción de portada, etiquetado FLAC, codificación temporal  
- **Ubicación:** carpeta temporal del sistema operativo (`systemTemp`)  
- **Retención:** se eliminan tras completar el proceso cuando es posible; además, el SO puede depurarlos periódicamente

#### (3) Guardado elegido por el usuario (SAF)
- Con “Guardar como”, los archivos finales pueden escribirse en rutas elegidas por el usuario (p. ej., Descargas, nube).  
- Estos archivos residen en **almacenamiento externo** y **permanecen tras la desinstalación**. El usuario puede eliminarlos manualmente.

#### (4) Estado de consentimiento (caché del SDK UMP)
- En EEE/Reino Unido/Suiza, el SDK UMP **cacha localmente el estado de consentimiento publicitario**.  
- Puede restablecerse borrando los datos de la app o desde **Opciones de privacidad** en la app, cuando esté disponible.

---

### 2-3) Datos de publicidad y consentimiento (SDKs de terceros)
- **Google Mobile Ads SDK (AdMob) y UMP** pueden recopilar/tratar, por ejemplo: **identificadores publicitarios (AAID/IDFA)**, **rangos de IP**, **información de dispositivo/app**, **señales de interacción con anuncios**, **estado de consentimiento**, etc.  
- **Finalidades:** entrega de anuncios, control de frecuencia, prevención de fraude, medición de rendimiento, cumplimiento legal  
- **Regiones con consentimiento obligatorio (EEE/Reino Unido/Suiza):** el consentimiento se recoge mediante UMP y se ofrece una pantalla de **Opciones de privacidad** cuando proceda.  
  En regiones sin dicha obligación (p. ej., KR), la opción **puede no mostrarse**.

---

## 3. Tratamiento y plazos de conservación

- **Ajustes locales:** permanecen en el dispositivo hasta que el usuario borre los datos de la app o la desinstale  
- **Archivos temporales:** se crean durante la codificación/extracción; se eliminan tras el proceso o pueden permanecer temporalmente en cachés del SO  
- **Datos de anuncios/consentimiento (terceros):** conforme a las **políticas de Google**

---

## 4. Transferencias a terceros y flujos transfronterizos

Para publicidad y gestión del consentimiento, la información del usuario puede transmitirse a la infraestructura de Google y tratarse allí.

| Ítem | Detalles |
|---|---|
| **Destinatario** | Google LLC y sus filiales/subencargados |
| **Destino** | Estados Unidos (y otras regiones donde se aloje la infraestructura de Google) |
| **Finalidad** | Entrega de anuncios, medición/rendimiento, cumplimiento legal, gestión del consentimiento |
| **Datos** | Identificadores publicitarios, rangos de IP, info de dispositivo/app, interacciones con anuncios, estado de consentimiento, etc. |
| **Conservación** | Según las políticas de Google |
| **Efecto de la negativa** | Si se rechaza, puede limitarse la personalización; podrían mostrarse anuncios no personalizados |

Cumplimos los requisitos de divulgación de **“Seguridad de datos” de Google Play** y mantenemos dichas divulgaciones alineadas con el tratamiento real.

---

## 5. Derechos del usuario y cómo ejercerlos

- **Desactivar anuncios personalizados / cambiar el consentimiento**  
  - En regiones admitidas (EEE/Reino Unido/Suiza): ajustar en **Ajustes → Opciones de privacidad**.  
  - Otras regiones: usar los ajustes del SO para **restablecer el ID de anuncios / limitar el seguimiento**.
- **Restablecer información local:** al borrar los datos o desinstalar la app se restablecen coordenadas del overlay, tamaño de fuente y otros ajustes locales.
- Los derechos bajo **RGPD/UK GDPR/LPD suiza/leyes estatales de privacidad de EE. UU.** (acceso, rectificación, supresión, portabilidad, limitación, retirada del consentimiento, etc.) pueden ejercerse según lo previsto en esas leyes.  
  Para los datos publicitarios tratados por Google, utilice los **procedimientos de Google**.

---

## 6. Privacidad de menores

Esta app **no está dirigida a menores**. Si una persona menor de la edad mínima legal usa la app, debe dejar de usarla y emplear, junto con su tutor, las funciones del SO para limitar anuncios. Cuando proceda, podemos aplicar **TFUA (etiqueta dirigida a menores)** u opciones equivalentes de protección infantil.

---

## 7. Medidas de seguridad

- **Minimización de datos** en la recogida y almacenamiento  
- **Uso limitado** de archivos temporales y eliminación tras el procesamiento cuando sea posible  
- Tratamiento **dentro del ámbito de permisos del SO**  
- **Cifrado en tránsito** (TLS o equivalente) para transferencias a terceros según las normas de los SDK

---

## 8. Seguridad de datos (Google Play)

Mantenemos exacto el apartado de **“Seguridad de datos”** en Play Console y lo actualizamos con prontitud cuando haya cambios.

---

## 9. Avisos de código abierto

La app utiliza software de código abierto como **FFmpeg**. Un archivo informativo (p. ej., `open-source/ffmpeg/WHERE-TO-GET-SOURCE.txt`) dentro de la app explica cómo obtener el código fuente. A petición, lo proporcionaremos conforme a dicha guía.

---

## 10. Contacto

- Correo: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 11. Cambios en esta Política

Podemos revisar esta Política debido a cambios legales o del servicio. Publicaremos las actualizaciones **en la app** y en esta **página de la política**.  
Para cambios materiales, avisaremos **al menos 7 días antes** de la fecha efectiva.

---

## Apéndice: Guía para el usuario

- **Enlace dentro de la app:** abra esta página desde **Ajustes → Privacidad**.  
- **Comportamiento regional:** en EEE/Reino Unido/Suiza se muestran Opciones de privacidad. **En KR y otras regiones, es posible que el botón no muestre opciones adicionales** si la ley no lo exige.

