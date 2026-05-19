---
title: Política de Privacidad | QDiary
description: Política de Privacidad de QDiary
---

# Política de Privacidad (QDiary)

- Nombre de la aplicación: QDiary
- Desarrollador: frog-im
- Contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Fecha de entrada en vigor: 2026-04-19
- Última actualización: 2026-04-19

Esta Política de Privacidad ha sido redactada con base en la implementación actual de la aplicación QDiary. QDiary ofrece funciones de escritura de diarios, generación y reflexión de misiones, inicio de sesión, guardado manual en la nube, publicidad y notificaciones, y en ese proceso puede tratar información personal o información que pueda constituir información personal en la medida necesaria.

## 1. Funciones proporcionadas

QDiary ofrece las siguientes funciones:

- Escritura, edición y visualización de diarios
- Clasificación por categorías y visualización en calendario
- Generación de misiones, reflexión sobre misiones y gestión de finalización de misiones
- Bloqueo local de la aplicación de diario y cifrado local
- Inicio de sesión con correo electrónico, verificación de correo electrónico, inicio de sesión anónimo (invitado) y restablecimiento de contraseña
- Guardado y carga en la nube iniciados por el usuario
- Visualización de anuncios y gestión de opciones de privacidad relacionadas con los anuncios
- Notificaciones recordatorias de misiones

## 2. Categorías de información tratada

### 2-1. Información introducida directamente por el usuario

- Dirección de correo electrónico
- Contraseña
- Título, contenido, fecha, categoría y dificultad del diario
- Respuestas de misión, contenido de reflexión e información de la misión seleccionada
- Valores seleccionados relacionados con el perfil de misión y texto de resumen
- Frase de contraseña para el bloqueo de la aplicación de diario

### 2-2. Información almacenada por la aplicación en el dispositivo

- Base de datos local del diario (SQLite)
- Información del estado de las misiones de los diarios locales
- Valores de estado relacionados con asistencia, configuración, idioma, notificaciones y anuncios
- Valores de verificación del bloqueo de la aplicación, salt y metadatos de cifrado
- Información de programación de notificaciones de misiones

### 2-3. Información de cuenta e identificación

La siguiente información puede tratarse a través de Firebase Authentication:

- UID de Firebase
- Dirección de correo electrónico
- Si se ha completado la verificación del correo electrónico
- Si se está utilizando el inicio de sesión anónimo

### 2-4. Información de publicidad y consentimiento

Al utilizar Google AdMob y el SDK de UMP, puede tratarse la siguiente información:

- Identificadores publicitarios (como Android AD_ID)
- Dirección IP e información de red
- Información del dispositivo, versión del sistema operativo e información de la aplicación
- Información sobre impresiones, clics y procesamiento de recompensas de anuncios
- Estado del consentimiento publicitario y estado de las opciones de privacidad

### 2-5. Información relacionada con las notificaciones

- Si se ha concedido el permiso de notificaciones
- Valores identificadores de los diarios que contienen misiones en curso
- Texto de la notificación de misión
- Horarios programados de las notificaciones

## 3. Finalidades del tratamiento

La aplicación trata la información para los siguientes fines:

- Registro, inicio de sesión, verificación de correo electrónico y restablecimiento de contraseña
- Escritura, guardado y visualización de diarios
- Generación de misiones, reflexión y determinación de finalización
- Cifrado y descifrado local asociados con el bloqueo de la aplicación
- Guardado y carga en la nube solicitados por el usuario
- Proporcionar notificaciones de misiones
- Proporcionar anuncios, procesar recompensas publicitarias y reflejar el estado del consentimiento publicitario
- Seguridad, respuesta a errores y operación del servicio

## 4. Almacenamiento local, almacenamiento en la nube y tratamiento externo

### 4-1. Almacenamiento local

La información del diario y de las misiones se almacena principalmente en la base de datos local del dispositivo.

- Si el bloqueo de la aplicación no está habilitado: se almacena localmente en forma general
- Si el bloqueo de la aplicación está habilitado: cierta información, como el título, el contenido y el estado de la misión, puede almacenarse cifrada localmente

### 4-2. Almacenamiento en la nube

La aplicación almacena datos en Firebase Firestore únicamente cuando el usuario ejecuta directamente la función `Guardar`.

Según la configuración actual del proyecto:

- No se utiliza sincronización automática completa
- Los datos se almacenan en Firestore `savedDiaries` solo cuando el usuario los guarda manualmente
- Al guardarse, el título, el contenido y el estado de la misión del diario pueden almacenarse en forma cifrada según el estado actual del bloqueo de la aplicación
- Los datos se vuelven a cargar en el almacenamiento local solo cuando el usuario ejecuta `Cargar`

### 4-3. Tratamiento externo para la generación y reflexión de misiones

Cuando el usuario solicita la generación o reflexión de una misión, la siguiente información puede utilizarse para tratamiento externo a través de Firebase Functions:

- Título del diario
- Contenido del diario o contenido de la reflexión
- Categoría
- Dificultad
- Misión seleccionada
- Información resumida del perfil de misión

Esta información se utiliza para la generación y evaluación de misiones a través de la API de OpenAI.

Importante:

- El contenido relacionado del diario se utiliza para tratamiento externo solo cuando se utiliza la función de misión.
- Según la configuración actual del proyecto, no se utiliza código que almacene registros de misiones en una colección separada llamada `questLogs`.

## 5. Servicios de terceros y tratamiento encargado

### 5-1. Google Firebase

Finalidad:

- Autenticación (Firebase Authentication)
- Almacenamiento en Firestore
- Ejecución de Cloud Functions

Información que puede tratarse:

- UID, dirección de correo electrónico y estado de autenticación
- Datos del diario guardados manualmente por el usuario
- Datos de solicitud de misión

### 5-2. OpenAI

Finalidad:

- Generación de misiones
- Reflexión sobre misiones y evaluación de finalización

Información que puede tratarse:

- Título/contenido del diario
- Texto de la misión
- Dificultad y categoría
- Contenido de reflexión introducido por el usuario
- Información resumida del perfil de misión

### 5-3. Google AdMob / UMP

Finalidad:

- Proporcionar anuncios de banner, intersticiales y recompensados
- Gestionar el consentimiento publicitario y las opciones de privacidad

Información que puede tratarse:

- Identificadores publicitarios
- Información del dispositivo y de la red
- Información de interacción con anuncios
- Estado del consentimiento

## 6. Aviso sobre transferencias internacionales

La aplicación puede tratar información personal o información relacionada fuera del país del usuario en los siguientes casos:

| Elemento | Detalles |
|---|---|
| Destinatario | Google LLC, OpenAI y operadores de infraestructura relacionados |
| País de destino | Estados Unidos, etc. |
| Momento de la transferencia | Durante el inicio de sesión, la generación/reflexión de misiones, las solicitudes de anuncios y el tratamiento del consentimiento |
| Método de transferencia | Comunicación de red cifrada |
| Finalidad de la transferencia | Autenticación, almacenamiento de datos, procesamiento serverless, generación/evaluación de misiones con IA y publicidad |

## 7. Período de conservación y uso

La aplicación conserva la información conforme a los siguientes criterios:

- Información local del diario/configuración: hasta que el usuario la elimine o desinstale la aplicación
- Información de la cuenta de Firebase: mientras el usuario mantenga la cuenta
- Datos almacenados en Firestore: mientras el usuario conserve los elementos guardados
- Datos de procesamiento de solicitudes de misión: en la medida necesaria para el procesamiento serverless
- Datos relacionados con anuncios/consentimiento: de acuerdo con la política de cada proveedor externo

Además, el proyecto actual incluye la siguiente lógica de limpieza automática:

- Limpieza de cuentas de usuarios anónimos y de los datos de subcolecciones de Firestore del usuario después de cierto período
- Limpieza de cuentas de usuarios regulares inactivos durante largo tiempo y de los datos de subcolecciones de Firestore del usuario

Sin embargo, si esto se refleja realmente en el entorno de producción puede variar según el estado del despliegue y la configuración del servidor.

## 8. Aviso sobre bloqueo de la aplicación y cifrado local

La aplicación ofrece una función separada de `Bloqueo de la aplicación de diario`.

- La frase de contraseña del bloqueo de la aplicación es independiente de la contraseña de la cuenta.
- La frase de contraseña del bloqueo de la aplicación se utiliza para cifrar y descifrar el diario localmente.
- Incluso si se introduce una frase de contraseña incorrecta, es posible que la aplicación en sí no quede completamente bloqueada; en su lugar, cierto contenido del diario puede permanecer ilegible.
- Algunos diarios pueden cifrarse por separado según la frase de contraseña utilizada en el momento de la escritura o del desbloqueo temporal.

Los usuarios deben conservar su frase de contraseña de forma segura y, si se pierde, la recuperación de algunos datos locales puede resultar difícil.

## 9. Aviso sobre notificaciones de misiones

Si el usuario habilita las notificaciones de misiones, pueden programarse notificaciones locales para cada diario con una misión en curso.

- La programación se gestiona principalmente mediante la programación interna del dispositivo.
- Según la configuración actual del proyecto, no existe una estructura confirmada en la que el texto original del diario se transmita periódicamente a un servidor central únicamente con fines de notificación.

## 10. Aviso sobre el uso de permisos

La aplicación puede utilizar los siguientes permisos para proporcionar sus funciones:

- `INTERNET`: comunicación con Firebase, OpenAI y los SDK publicitarios
- `com.google.android.gms.permission.AD_ID`: uso de identificadores publicitarios
- `POST_NOTIFICATIONS`: mostrar notificaciones de misiones
- `RECEIVE_BOOT_COMPLETED`: restaurar notificaciones programadas después del reinicio del dispositivo

Los permisos se utilizan solo en la medida necesaria para llevar a cabo las funciones correspondientes.

## 11. Derechos del titular de los datos y cómo ejercerlos

Los usuarios pueden ejercer los siguientes derechos:

- Acceder, modificar y eliminar datos dentro de la aplicación
- Eliminar o sobrescribir datos almacenados en la nube
- Solicitar cierre de sesión y eliminación de la cuenta
- Cambiar las opciones de privacidad publicitaria
- Desactivar los permisos de notificación

Cómo ejercer estos derechos:

- Eliminar o editar directamente los diarios dentro de la aplicación
- Eliminar la aplicación o restablecer los datos locales
- Cerrar sesión en la cuenta y solicitar la eliminación por separado
- Cambiar las notificaciones, los identificadores publicitarios y los permisos en la configuración del dispositivo
- Correo de contacto: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

## 12. Medidas de seguridad

La aplicación aplica o puede aplicar las siguientes medidas de protección:

- Comunicación basada en HTTPS
- Bloqueo y cifrado de la aplicación de diario local
- Almacenamiento separado de los valores de verificación de la frase de contraseña
- Uso de Firebase Authentication
- Solicitud de permisos mínimos

Sin embargo, pueden surgir riesgos dependiendo del estado de seguridad del dispositivo del usuario, como root, jailbreak, malware o uso de un dispositivo compartido.

## 13. Información personal de menores

La aplicación no está diseñada como un servicio dirigido principalmente a menores. Sin embargo, pueden aplicarse opciones relacionadas con la edad dentro de UMP durante el tratamiento de anuncios/consentimiento.

## 14. Cambios en esta política

Esta Política puede revisarse debido a cambios en las leyes, servicios de terceros o funciones de la aplicación.

- Última actualización para la versión actual: **2026-04-19**

## 15. Contacto

- Desarrollador: frog-im
- Correo electrónico: [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- Guía de eliminación de cuenta: [Instrucciones de eliminación](https://docs.google.com/forms/d/e/1FAIpQLSexIrSPRwSmVG5aU-Mp0wq0uRyXTh2Xh9Gag3Y4QBisWmFZWw/viewform?usp=dialog)

