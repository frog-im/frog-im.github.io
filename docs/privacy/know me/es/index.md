---
title: Política de Privacidad | know_me
description: know_me (PeopleNote, Memory for People) Política de Privacidad (Español)
---

# Política de Privacidad (know_me / PeopleNote, Memory for People)

- **Nombre de la aplicación:** know_me (PeopleNote, Memory for People)
- **Desarrollador:** frog-im
- **Responsable de Protección de Datos Personales / Persona de contacto:** frog-im
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Fecha de entrada en vigor:** 2026-03-04
- **Última actualización:** 2026-03-04

> Esta Política ha sido elaborada con base en la información procesada por la aplicación y sus funciones relacionadas.  
> Si existen leyes o reglamentos obligatorios aplicables en un país o región específica, dichas leyes o reglamentos podrán prevalecer.

---

## 1. Finalidad y Alcance

`know_me` es una aplicación diseñada para ayudar a los usuarios a registrar y gestionar información sobre personas y, cuando sea necesario, realizar copias de seguridad, restaurar y compartir dicha información en archivos PDF.

Sus funciones principales incluyen:

- Almacenar información específica de cada persona (como nombre, texto identificativo, notas, rasgos de personalidad, país, género, información de contacto, etc.)
- Clasificación en carpetas, búsqueda y funciones de fusión
- Adjuntar fotos y gestionar descripciones
- Exportar e importar copias de seguridad (`.knm`)
- Exportar archivos PDF
- Bloqueo de la aplicación (contraseña/patrón)
- Gestión de publicidad y consentimiento (AdMob/UMP)

La aplicación no requiere un registro de cuenta por separado, y los datos principales del usuario generalmente se almacenan de forma local en el dispositivo del usuario.  
Sin embargo, ciertos SDK de terceros incluidos para la gestión de publicidad y consentimiento pueden procesar alguna información.

---

## 2. Categorías de Información Personal Procesada

### 2-1) Información ingresada directamente por el usuario

La siguiente información se almacena únicamente cuando el usuario la introduce directamente:

- Nombre
- Texto identificativo (como apariencia/características utilizadas como texto de nota)
- Notas
- Rasgos de personalidad, país, género
- Número de teléfono
- Texto relacionado con el momento de aparición / momento del encuentro
- Información de plataforma/sitio
- Nombre/color de la carpeta
- Descripción de la imagen (caption)

### 2-2) Archivos seleccionados en el dispositivo

- Archivos de imagen seleccionados por el usuario al adjuntar fotos
- Archivos de copia de seguridad `.knm` seleccionados por el usuario al importar copias de seguridad
- Rutas de guardado y archivos guardados seleccionados por el usuario al exportar PDF/copias de seguridad

### 2-3) Datos almacenados localmente dentro de la aplicación

Los siguientes datos pueden almacenarse en el dispositivo del usuario para proporcionar las funciones de la aplicación:

- Base de datos SQLite (`people_note.db`): metadatos de personas/carpetas/plataformas/sitios/imágenes
- Archivos de imagen: cifrados y almacenados dentro de la carpeta de documentos de la aplicación (`.enc`)
- Ajustes de la aplicación (`SharedPreferences`): tema, ordenación, opciones de privacidad/publicidad, opciones de enmascaramiento de PDF, políticas de bloqueo de la aplicación, etc.
- Información de bloqueo de la aplicación: valores hash y salts para contraseñas/patrones (`SharedPreferences`)
- Claves de cifrado locales: almacenadas en `flutter_secure_storage`
- Archivos temporales: vistas previas de descifrado de imágenes, archivos de caché de importación/exportación, etc. (carpeta temporal)

### 2-4) Información que puede procesarse automáticamente durante la gestión de publicidad y consentimiento

Cuando las funciones de publicidad o gestión de consentimiento están habilitadas, los SDK de Google LLC y de socios relacionados (como AdMob y UMP) pueden procesar automáticamente la siguiente información:

- Identificadores publicitarios (AAID/IDFA, etc.)
- Dirección IP e información de red
- Información del dispositivo (versión del sistema operativo, modelo del dispositivo, versión de la aplicación, etc.)
- Información de interacción con anuncios (impresiones, clics, etc.)
- Estado de consentimiento e información sobre elecciones de privacidad
- Información relacionada con diagnóstico, rendimiento y seguridad

Los registros principales del usuario de la aplicación, por lo general, no se cargan en el servidor del desarrollador, pero parte de la información anterior puede transmitirse a servicios de terceros mientras se utilicen funciones de publicidad/consentimiento.

---

## 3. Finalidad del Tratamiento de la Información Personal

La aplicación procesa información personal o información relacionada para los siguientes fines:

- Registrar y consultar información sobre personas centrada en contactos/notas
- Proporcionar funciones de organización, como clasificación en carpetas, búsqueda y fusión
- Adjuntar y mostrar fotos
- Realizar funciones solicitadas por el usuario, como copia de seguridad/restauración y exportación a PDF
- Proporcionar funciones de seguridad de bloqueo de la aplicación
- Proporcionar publicidad, gestionar el consentimiento, prevenir actividades fraudulentas y cumplir con obligaciones legales

---

## 4. Período de Conservación y Almacenamiento de la Información Personal

- Datos internos de la aplicación (SQLite, ajustes locales, imágenes cifradas): se conservan en el dispositivo del usuario hasta que se elimine la aplicación, se borren los datos de la aplicación o el usuario elimine los datos directamente
- Archivos temporales: se eliminan después de que finaliza la tarea correspondiente o se borran conforme a la política de caché del sistema operativo
- Archivos exportados por el usuario (PDF, archivos de copia de seguridad): pueden permanecer en la ubicación de almacenamiento seleccionada por el usuario y deben ser eliminados directamente por el usuario
- Datos relacionados con publicidad/consentimiento (procesados por terceros): sujetos a las políticas de cada proveedor de servicios y a las leyes aplicables

En principio, la aplicación no almacena los registros principales del usuario en el servidor del desarrollador.  
Sin embargo, los archivos que el usuario guarde directamente en almacenamiento externo son gestionados dentro del propio entorno del usuario.

---

## 5. Procedimientos y Métodos para la Eliminación de la Información Personal

Cuando la finalidad del tratamiento se haya cumplido o cuando el usuario solicite la eliminación, la aplicación destruye la información correspondiente o la procesa para que ya no sea referenciada, de la siguiente manera.

### 5-1) Procedimientos de eliminación

- Cuando el usuario elimina directamente registros individuales de personas, carpetas, imágenes, datos de copia de seguridad, etc., dichos datos se consideran sujetos a eliminación inmediata.
- Cuando el usuario elimina la aplicación o borra los datos de la aplicación desde la configuración del dispositivo, los datos almacenados en el área interna de almacenamiento de la aplicación se eliminan de acuerdo con los procedimientos de eliminación del sistema operativo.
- Los archivos temporales quedan sujetos a limpieza una vez finalizada la tarea correspondiente, y algunos datos en caché pueden permanecer hasta cierto momento dependiendo de la política del sistema operativo.

### 5-2) Métodos de eliminación

- Datos SQLite: eliminación de los registros correspondientes
- Ajustes de la aplicación (`SharedPreferences`): eliminación de la clave correspondiente o de todos los ajustes
- Valores de `flutter_secure_storage`: eliminación de los elementos correspondientes de almacenamiento seguro
- Archivos internos de la aplicación (imágenes cifradas, archivos temporales, etc.): eliminación de los archivos correspondientes
- PDF/archivos de copia de seguridad guardados directamente por el usuario en almacenamiento externo: no son eliminados automáticamente por la aplicación y deben ser eliminados directamente por el usuario

Salvo que la legislación aplicable exija lo contrario, el desarrollador no almacena por separado los registros principales del usuario en el servidor del desarrollador.

---

## 6. Cesión a Terceros, Encargo de Tratamiento y Transferencia Internacional

La aplicación puede utilizar servicios de Google para la gestión de publicidad y consentimiento.

| Elemento | Detalles |
|---|---|
| **Destinatario / Encargado** | Google LLC y sus filiales (operadores de AdMob/UMP) |
| **País de transferencia** | Estados Unidos y regiones donde opera la infraestructura de Google |
| **Momento de la transferencia** | De forma continua durante solicitudes de anuncios, verificaciones del estado de consentimiento, inicialización del SDK y operación |
| **Método de transferencia** | Transmisión mediante comunicación de red entre la aplicación y servidores de terceros |
| **Base legal para la transferencia internacional** | Tratamiento dentro del alcance necesario para prestar el servicio conforme a bases legales aplicables o, cuando sea necesario, con base en el consentimiento del titular de los datos |
| **Finalidad** | Publicación de anuncios, medición de anuncios, gestión del consentimiento, prevención de fraude y cumplimiento de políticas/leyes |
| **Categorías de datos (ejemplos)** | Identificadores publicitarios (AAID/IDFA), información de IP/red, información del dispositivo/aplicación, información de interacción con anuncios, estado de consentimiento |
| **Período de conservación** | Sujeto a las políticas de Google y a las leyes aplicables |
| **Efecto del rechazo** | Los anuncios personalizados pueden verse limitados, pueden mostrarse anuncios no personalizados o algunas funciones relacionadas con anuncios pueden estar restringidas |

El desarrollador no recopila ni vende los datos principales de registros de personas de la aplicación a través de su propio servidor.

---

## 7. Información sobre los Permisos Utilizados

La aplicación puede utilizar los siguientes permisos:

- `INTERNET`: comunicación para SDK publicitarios y funciones de red relacionadas
- `com.google.android.gms.permission.AD_ID`: uso de identificadores publicitarios (AdMob)
- `READ_MEDIA_IMAGES` (Android 13 o superior), `READ_EXTERNAL_STORAGE` (Android 12 o inferior): adjuntar/seleccionar fotos

Los permisos se utilizan únicamente dentro del alcance necesario para proporcionar las funciones correspondientes.

---

## 8. Instalación, Funcionamiento y Rechazo de Mecanismos de Recopilación Automática

Esta aplicación no utiliza directamente cookies generales de sitios web.  
Sin embargo, en relación con las funciones de publicidad y gestión de consentimiento, los SDK de terceros pueden procesar automáticamente identificadores publicitarios, información de red, información del dispositivo y datos similares.

Los usuarios pueden ajustar la configuración correspondiente de las siguientes maneras:

- Cambiar las selecciones dentro de las opciones de privacidad o la pantalla de gestión de consentimiento de la aplicación (cuando esté disponible)
- Restablecer o eliminar el identificador publicitario en la configuración del sistema operativo del dispositivo
- Limitar los anuncios personalizados o ajustar opciones de privacidad relacionadas en la configuración del sistema operativo del dispositivo

Si el usuario limita la publicidad personalizada, pueden mostrarse anuncios no personalizados o ciertas funciones relacionadas con anuncios pueden estar restringidas.

---

## 9. Derechos del Usuario y Cómo Ejercerlos

Conforme a la legislación aplicable, los usuarios pueden tener los siguientes derechos:

- Solicitar acceso, corrección o eliminación de la información personal
- Solicitar la suspensión o limitación del tratamiento
- Retirar el consentimiento para el tratamiento basado en consentimiento
- Cambiar las opciones de publicidad/consentimiento

Estos derechos pueden ejercerse de las siguientes maneras:

- Modificar o eliminar datos directamente dentro de la aplicación
- Inicializar los datos locales eliminando los datos de la aplicación o desinstalando la aplicación
- Cambiar el consentimiento publicitario a través de las opciones de privacidad/pantalla de consentimiento de la aplicación (en regiones donde esté disponible)
- Restablecer/eliminar el identificador publicitario o limitar los anuncios personalizados a través de la configuración del sistema operativo del dispositivo
- Contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 10. Medidas de Seguridad

El desarrollador aplica o procura aplicar las siguientes medidas:

- Los registros del usuario generalmente se almacenan localmente en el dispositivo
- Los archivos de imagen adjuntos se almacenan localmente en forma cifrada (basado en AES-GCM)
- La información de bloqueo de la aplicación se almacena en forma hash en lugar de texto sin formato
- Los archivos de copia de seguridad se almacenan tras ser cifrados con base en una contraseña del usuario
- La comunicación con SDK de terceros se cifra (HTTPS/TLS)
- Los permisos se utilizan con un alcance de acceso minimizado

Sin embargo, no pueden eliminarse por completo los riesgos derivados del estado de seguridad del dispositivo del usuario (como root/jailbreak, aplicaciones maliciosas o exposición de almacenamiento compartido).

---

## 11. Información Relativa a Datos Sensibles

Esta aplicación no requiere la introducción de datos sensibles.  
Se recomienda a los usuarios no introducir contenido sensible, como información de salud, opiniones políticas, religión, información biométrica o información relacionada con la vida sexual, en notas o campos de entrada libre.

Si un usuario introduce voluntariamente contenido sensible, dicha información podrá almacenarse como datos locales en el dispositivo gestionado directamente por el usuario.

---

## 12. Protección de la Información Personal de Menores

Esta aplicación no está diseñada principalmente para menores.  
Los tutores pueden gestionar el uso mediante funciones de control parental proporcionadas por el dispositivo o la tienda de aplicaciones.

---

## 13. Toma de Decisiones Automatizada

Esta aplicación no realiza toma de decisiones automatizada basada en información personal que produzca efectos jurídicos o impactos significativos similares.

---

## 14. Aviso de Seguridad de los Datos (Google Play, etc.)

El desarrollador procura mantener y actualizar los elementos de divulgación de seguridad de los datos en los mercados de aplicaciones (como Google Play) de acuerdo con las prácticas reales de tratamiento de la aplicación y las prácticas reales de tratamiento de los SDK de terceros.

Sin embargo, la información mostrada en las tiendas de aplicaciones puede variar según la versión de la aplicación, el país de distribución, la configuración de SDK de terceros y los cambios de políticas.

---

## 15. Aviso de Código Abierto

La aplicación utiliza determinadas bibliotecas de código abierto.  
La información sobre las licencias correspondientes puede encontrarse en la pantalla relacionada dentro de la aplicación o en los avisos proporcionados a través del canal de distribución.

---

## 16. Contacto

Para consultas relacionadas con esta Política de Privacidad:

- **Responsable de Protección de Datos Personales / Persona de contacto:** frog-im
- **Correo electrónico:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

---

## 17. Cambios en esta Política de Privacidad

Esta Política puede ser revisada debido a cambios en leyes/políticas, funciones de la aplicación o SDK de terceros.  
Si hubiera cambios sustanciales, podrá notificarse a través de avisos dentro de la aplicación, la página de distribución o actualizaciones de la página de la política.

Última actualización: **2026-03-04**