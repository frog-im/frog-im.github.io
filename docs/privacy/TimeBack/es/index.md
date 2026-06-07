---
title: Política de Privacidad | TimeBack
description: Política de privacidad de TimeBack
lang: es
last_updated: 2026-06-06
---

# Política de privacidad (TimeBack)

- **Nombre de la aplicación:** TimeBack
- **Desarrollador:** frog-im
- **Contacto:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Fecha de entrada en vigor:** 2026-06-03
- **Última actualización:** 2026-06-06

Esta Política de Privacidad se basa en la implementación actual de la aplicación TimeBack. TimeBack proporciona revisión del tiempo de pantalla, objetivos diarios, registros de tiempo recuperado, reflexiones, desafíos, notificaciones, uso compartido y funciones publicitarias.

## 1. Características

TimeBack proporciona las siguientes características:

- Revisión del tiempo de uso de la aplicación mediante el permiso de acceso al uso de Android
- Objetivos de uso diario, recordatorios y notificaciones de uso de la barra de estado
- Notificaciones de advertencia de límite estricto y visualización superpuesta
- Selección de aplicación de excepción de superposición
- Registros de actividad de tiempo reclamado
- Registros diarios de reflexión.
- Progreso del desafío y gestión de la lista de verificación.
- Compartir imágenes de estadísticas de uso
- Anuncios de Google AdMob y opciones de privacidad basadas en UMP

## 2. Información que procesamos

### 2-1. Lectura de información mediante permiso de acceso de uso

Si el usuario otorga permiso a Android `PACKAGE_USAGE_STATS`, la aplicación puede leer la siguiente información del dispositivo:

- Nombre del paquete de la aplicación
- Nombre de la aplicación
- Tiempo de uso de la aplicación
- Intervalo de fechas y horas utilizado para la agregación de uso

Esta información se utiliza para proporcionar estadísticas de uso y comparar el uso con los objetivos del usuario.

### 2-2. Información ingresada o configurada por el usuario

- Objetivo de uso diario
- Estado e intervalo habilitados para el recordatorio de uso
- Configuración de visualización de uso de la barra de estado
- Categoría de actividad de tiempo recuperado, título, hora de inicio y duración
- Texto de reflexión diaria
- Progreso del desafío y entradas de la lista de verificación
- Lista de aplicaciones de excepción de superposición

### 2-3. Información almacenada en el dispositivo

La aplicación puede almacenar la siguiente información en una base de datos local SQLite o SharedPreferences:

- Registros de tiempo de uso de la aplicación
- Metas y configuraciones diarias
- Registros de actividad de tiempo reclamado
- Registros diarios de reflexión.
- Progreso del desafío y estado de la lista de verificación
- Estado de finalización de la incorporación
- Configuraciones como recordatorios de uso, advertencias de límites estrictos, visualización de la barra de estado y aplicaciones de excepción superpuestas
- Consentimiento de publicidad local y estado de la opción de privacidad

Según la implementación actual, estos registros locales no se cargan automáticamente en los servidores de frog-im.

### 2-4. Datos de publicidad y consentimiento

Cuando se utilizan los anuncios móviles de Google SDK (AdMob) y UMP, Google o sus afiliados pueden procesar información como la siguiente:

- Identificadores de publicidad, como Android AD_ID
- IP dirección e información de red
- Información del dispositivo, versión OS e información de la aplicación
- Impresiones de anuncios, clics, datos de medición y señales de error
- Consentimiento publicitario y estado de la opción de privacidad
- Ubicación aproximada

## 3. Finalidades del Tratamiento

La aplicación procesa información para los siguientes propósitos:

- Leer el tiempo de uso, mostrar estadísticas y comparar el uso con los objetivos
- Almacenamiento de registros de tiempo recuperado y reflexión ingresados ​​por el usuario
- Gestionar el progreso del desafío
- Proporcionar recordatorios y notificaciones de la barra de estado
- Proporcionar notificaciones de advertencia de límites estrictos, visualización superpuesta y manejo de excepciones superpuestas
- Compartir imágenes de estadísticas de uso cuando lo solicite el usuario
- Publicar anuncios, medir el rendimiento de los anuncios y aplicar opciones de consentimiento para los anuncios
- Mantener la estabilidad de la aplicación y responder a errores

## 4. Almacenamiento local y procesamiento externo

### 4-1. Almacenamiento local

TimeBack almacena los datos del usuario principalmente en el almacenamiento interno de la aplicación en el dispositivo. Según la implementación actual, los registros de uso, los objetivos, las reflexiones y la información de los desafíos no se cargan automáticamente en los servidores de frog-im.

El almacenamiento local puede incluir lo siguiente.

| Almacenamiento | Artículos almacenados | Objetivo | Método de eliminación |
|---|---|---|---|
| SQLbase de datos del sitio | Registros de uso de aplicaciones, nombres de paquetes, nombres de aplicaciones, tiempo de uso, agregados basados ​​en fechas | Mostrar estadísticas de uso y comparar el uso con los objetivos | Funciones de eliminación dentro de la aplicación, borrado de datos de la aplicación o desinstalación de la aplicación |
| SQLbase de datos del sitio | Actividades de tiempo recuperado, reflexiones, progreso del desafío, entradas de la lista de verificación | Mostrar registros y gestionar el progreso | Funciones de eliminación dentro de la aplicación, borrado de datos de la aplicación o desinstalación de la aplicación |
| Preferencias compartidas | Estado de finalización de la incorporación, configuración de recordatorio, configuración de advertencia de límite estricto, configuración de visualización de la barra de estado, lista de aplicaciones de excepción superpuestas, estado de consentimiento de publicidad local | Mantener la configuración de la aplicación | Borrar datos de la aplicación o desinstalar la aplicación |
| Archivos temporales/caché | Imágenes de estadísticas de uso compartidas y archivos temporales similares | Realizar el intercambio solicitado por el usuario. | Eliminado después de compartir cuando sea posible, o de acuerdo con las políticas de limpieza de OS/aplicación |

Cuando el usuario borra los datos de la aplicación o la desinstala, los datos almacenados en el almacenamiento interno de la aplicación generalmente se eliminan. Sin embargo, la copia de seguridad de Android, la copia de seguridad del fabricante, la copia de seguridad en la nube o los archivos compartidos directamente por el usuario pueden conservarse por separado de acuerdo con las políticas de esos servicios.

Los registros de uso y el texto de reflexión pueden revelar rutinas o intereses personales. En dispositivos compartidos, los usuarios deben utilizar medidas de seguridad adecuadas, como el bloqueo del dispositivo o cuentas OS separadas.

### 4-2. Cargas del servidor

Según el proyecto actual, TimeBack no carga automáticamente registros de uso, reflexiones o registros de desafío a los servidores de frog-im. Si el usuario utiliza la función para compartir, una imagen estadística generada puede transferirse a la aplicación o servicio externo seleccionado por el usuario.

### 4-3. Procesamiento publicitario

Google AdMob y UMP se utilizan para la publicidad dentro de la aplicación y la gestión del consentimiento. La información relacionada con la publicidad puede procesarse en la infraestructura de Google.

## 5. Servicios y procesadores de terceros

### 5-1. Google AdMob/UMP

Objetivo:

- Entrega de anuncios publicitarios
- Consentimiento publicitario y manejo de opciones de privacidad
- Medición del rendimiento publicitario y prevención del fraude

Información que podrá ser tratada:

- Identificadores publicitarios
- Información del dispositivo y de la red
- Información de interacción con anuncios
- Estado de consentimiento y opción de privacidad

### 5-2. Compartir aplicaciones o servicios de destino

Si el usuario utiliza directamente la función para compartir imágenes de estadísticas de uso, la aplicación o servicio externo seleccionado puede procesar la imagen compartida. Ese tratamiento se rige por la política de privacidad del servicio seleccionado.

## 6. Aviso de transferencia transfronteriza

La información podrá ser procesada fuera del país del usuario en los siguientes casos.

| Artículo | Detalles |
|---|---|
| Beneficiario | Google LLC y sus afiliados |
| Destino | Estados Unidos y otros países/regiones donde se encuentra la infraestructura de Google |
| Momento | Cuando la aplicación se ejecuta, solicita anuncios, muestra o mide anuncios, procesa clics o maneja el consentimiento |
| Método | Comunicación de red cifrada (HTTPS/TLS) |
| Objetivo | Entrega de anuncios, manejo del estado de personalización, medición, análisis, mejora de la estabilidad del servicio, cumplimiento legal |
| Datos | Identificadores de publicidad, información del dispositivo/aplicación/red, información de interacción con anuncios, estado de consentimiento, ubicación aproximada, etc. |
| Retención | De acuerdo con las políticas de Google y la legislación aplicable |

Para obtener más información, consulte [Cross-Border Transfer Notice](./policy/).

## 7. Lista de aplicaciones instaladas y excepciones de superposición

En Android, si el usuario configura aplicaciones de excepción de superposición, la aplicación puede leer los nombres de los paquetes y los nombres de las aplicaciones que se pueden iniciar en el dispositivo para mostrar una lista de selección. Los nombres de los paquetes seleccionados por el usuario como excepciones se almacenan en SharedPreferences en el dispositivo y se usan solo para evitar mostrar superposiciones de advertencia de límite estricto encima de esas aplicaciones.

## 8. Retención

La aplicación retiene información bajo los siguientes estándares:

- Información de uso local, objetivos, reflexión y desafíos: hasta que el usuario la elimine, borre los datos de la aplicación o la desinstale.
- Configuración de SharedPreferences: hasta que el usuario borre los datos de la aplicación o la desinstale
- Archivos temporales para imágenes compartidas: según sea necesario para compartir o según las políticas de limpieza OS
- Datos publicitarios y relacionados con el consentimiento: según las políticas de Google y otros terceros relevantes

## 9. Permisos

La aplicación puede utilizar los siguientes permisos:

- `PACKAGE_USAGE_STATS`: leer el tiempo de uso de la aplicación
- `POST_NOTIFICATIONS`: muestra recordatorios de uso y notificaciones de la barra de estado
- `SYSTEM_ALERT_WINDOW`: muestra superposiciones de advertencia de límite estricto
- `INTERNET`: comunicarse con el anuncio SDKs y mostrar páginas de aviso legal
- `ACCESS_NETWORK_STATE`: comprobar el estado de la red
- `com.google.android.gms.permission.AD_ID`: utilizar identificadores de publicidad

Los permisos se utilizan solo según sea necesario para las funciones de la aplicación. Los usuarios pueden revocar permisos en la configuración del dispositivo, pero las funciones relacionadas pueden ser limitadas.

## 10. Derechos y opciones del usuario

Los usuarios pueden:

- Ver, editar o eliminar registros dentro de la aplicación
- Elimine información local borrando los datos de la aplicación o desinstalando la aplicación
- Cambiar la configuración del identificador de publicidad, notificación y acceso de uso en la configuración del dispositivo
- Revocar el permiso de superposición y cambiar la configuración de la aplicación de excepción de superposición
- Cambiar las opciones de privacidad de los anuncios
- Contáctenos si tiene preguntas sobre privacidad o solicitudes de eliminación

Correo electrónico de contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 11. Medidas de seguridad

La aplicación aplica o puede aplicar las siguientes salvaguardas:

- Comunicación externa basada en HTTPS/TLS
- Procesamiento de datos local primero
- Solicitudes de permiso mínimas necesarias para las funciones de la aplicación
- Aplicación del estado de consentimiento publicitario.

Las condiciones de seguridad del dispositivo, como rooting, jailbreak, malware o uso de dispositivos compartidos, pueden crear riesgos adicionales.

## 12. Privacidad de los niños

TimeBack no está diseñado principalmente para niños. Es posible que se apliquen configuraciones relacionadas con la edad o políticas de plataforma de Google Mobile Ads SDK y UMP durante el procesamiento de publicidad y consentimiento.

## 13. Cambios

Esta Política puede actualizarse debido a cambios en la ley, la configuración de servicios de terceros o las características de la aplicación. Los cambios materiales se notificarán mediante un aviso en la aplicación o actualizando esta página.

## 14. Contacto

- Desarrollador: frog-im
- Correo electrónico: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
