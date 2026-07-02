---
title: Política de privacidad | FileGuard
description: Política de privacidad de FileGuard
lang: es
last_updated: 2026-06-23
---

# Política de privacidad (FileGuard)

- **Aplicación:** FileGuard
- **Desarrollador:** frog-im
- **Contacto de privacidad:** frog-im
- **Correo electrónico:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)
- **Fecha de entrada en vigor:** 23 de junio de 2026
- **Última actualización:** 23 de junio de 2026

> Esta Política describe la implementación actual de la aplicación FileGuard. Las leyes obligatorias de su país o región pueden prevalecer.

---

## 1. Alcance y finalidad

FileGuard es una utilidad de seguridad que le permite conservar archivos seleccionados, contenido multimedia capturado, notas y texto del portapapeles en bóvedas cifradas en su dispositivo, y crear archivos de copia de seguridad cifrados.

La aplicación no requiere registro ni inicio de sesión. El desarrollador no opera ningún servidor que reciba sus archivos de bóveda, contenido de archivos, contraseñas, nombres de bóvedas o historial de actividad. En Android, sin embargo, la aplicación puede usar Google AdMob y Google User Messaging Platform (UMP) para publicidad y opciones de privacidad.

## 2. Información procesada

### 2.1 Datos de bóveda seleccionados o creados por usted

La aplicación puede procesar la siguiente información en su dispositivo:

- Fotos, videos, documentos y otros archivos que seleccione mediante el selector de archivos del sistema
- Fotos o videos capturados con la aplicación, incluido el audio grabado con un video
- Texto del portapapeles que guarde manualmente o que se detecte cuando habilite la protección automática del portapapeles
- Nombre de archivo, tipo MIME, tamaño, hora de creación, título e información relacionada con la vista previa
- Nombre e identificador de la bóveda, clasificación de seguridad, estado del archivo original y referencia del archivo original
- Paquetes cifrados de exportación, transferencia o copia de seguridad que usted cree

Esta información se procesa en su dispositivo para proporcionar las funciones de la aplicación. El desarrollador no la carga en un servidor operado por el desarrollador.

### 2.2 Información de autenticación y seguridad

La aplicación puede procesar la siguiente información en almacenamiento seguro de su dispositivo:

- Salts, ajustes de derivación de claves y paquetes de claves cifrados utilizados para derivar o proteger claves de cifrado
- Credenciales de acceso a la bóveda y claves locales protegidas por una clave vinculada al dispositivo para acceso biométrico
- Preferencias de seguridad como protección contra capturas de pantalla, borrado del portapapeles, reautenticación biométrica y protección automática

Su contraseña en texto claro no se envía al desarrollador. La autenticación biométrica la realiza el sistema operativo. La aplicación no recopila imágenes de huellas dactilares o del rostro ni plantillas biométricas; solo recibe el resultado de la autenticación.

### 2.3 Información local de actividad y copia de seguridad

La aplicación puede almacenar localmente:

- El tipo, la descripción, la hora y los identificadores de elementos relacionados para eventos de protección, bloqueo, eliminación, eliminación del original, copia de seguridad y restauración
- Hasta 500 entradas del registro de actividad
- Destino de la copia de seguridad, hora de la última copia, número de elementos y estado de éxito o error
- Si la copia de seguridad automática está habilitada y la contraseña necesaria para actualizar esa copia
- Opciones de privacidad de anuncios, opción de procesamiento de datos restringido y un recuento de elementos protegidos utilizado para la frecuencia de anuncios

Los ajustes sensibles, incluido el estado de la copia de seguridad y la contraseña de copia automática, se almacenan en un almacén local cifrado con una clave del dispositivo. Usted es responsable de mantener segura su contraseña de copia de seguridad.

### 2.4 Información procesada durante publicidad y consentimiento

En la plataforma publicitaria compatible, actualmente Android, la aplicación puede usar Google AdMob y UMP. Google y los proveedores de tecnología publicitaria pueden procesar:

- Identificadores publicitarios, de instancia de aplicación o relacionados con el dispositivo
- Dirección IP y ubicación aproximada inferida a partir de información como la dirección IP
- Modelo del dispositivo, sistema operativo, versión de la aplicación, idioma e información de red
- Solicitudes de anuncios, impresiones, clics, interacciones y diagnósticos
- Estado del consentimiento y opciones regionales de privacidad

Esta información puede utilizarse para la entrega de anuncios, anuncios no personalizados, limitación de frecuencia, medición, prevención del fraude, gestión del consentimiento, seguridad y cumplimiento legal. La aplicación está implementada para inicializar el SDK de Google Mobile Ads solo después de que UMP indique que pueden solicitarse anuncios.

Consulte la [Política de privacidad de Google](https://policies.google.com/privacy) y la [información sobre tecnologías publicitarias de Google](https://policies.google.com/technologies/ads).

## 3. Finalidades del procesamiento

FileGuard procesa información para:

- Almacenar y mostrar contenido seleccionado o capturado en bóvedas cifradas
- Controlar el acceso a la bóveda con bloqueo, contraseñas y autenticación biométrica
- Importar, exportar, mover, eliminar y hacer seguimiento del estado del archivo original del contenido
- Crear y restaurar copias de seguridad cifradas en una ubicación seleccionada por usted
- Mantener preferencias de seguridad y borrar archivos temporales descifrados y contenido del portapapeles
- Mostrar actividad de seguridad local y estado de errores
- Entregar anuncios de Android, controlar la frecuencia de anuncios y proporcionar opciones de privacidad
- Prevenir abusos, proteger el servicio y cumplir obligaciones legales

## 4. Almacenamiento y conservación

| Categoría | Almacenamiento y conservación | Cómo eliminar |
|---|---|---|
| Archivos y metadatos cifrados de la bóveda | Almacenados en el almacenamiento local privado de la aplicación hasta que usted los elimine | Elimine el elemento o la bóveda en la aplicación, borre los datos de la aplicación o desinstale |
| Credenciales y ajustes de seguridad | Almacenados en almacenamiento seguro del sistema operativo y almacenamiento cifrado con clave del dispositivo hasta que se cambien o se eliminen los datos de la aplicación | Deshabilite la función correspondiente, borre los datos de la aplicación o desinstale |
| Historial de actividad | Hasta 500 entradas en almacenamiento local cifrado | Borre los datos de la aplicación o desinstale |
| Archivos temporales descifrados | Escritos temporalmente en la caché de la aplicación y borrados al iniciar, pasar a segundo plano o completar la función, según el mejor esfuerzo | Cierre la aplicación o borre su caché/datos |
| Contenido del portapapeles | Procesado a través del portapapeles del sistema operativo cuando se usa copiar o protección automática | Borrado automático según el mejor esfuerzo, copie otro contenido o reinicie el dispositivo |
| Archivos de copia de seguridad cifrados | Almacenados en una carpeta del dispositivo, proveedor de documentos o ubicación sincronizada en la nube que usted seleccione hasta que los elimine | Elimine mediante el administrador de archivos o servicio de almacenamiento correspondiente |
| Datos publicitarios de Google | Conservados conforme a las políticas y obligaciones legales de Google y sus procesadores | Cambie los ajustes de anuncios de la aplicación/dispositivo o use los controles de privacidad de Google |

El sistema operativo, el fabricante del dispositivo, el proveedor de documentos o el proveedor de copia de seguridad en la nube pueden conservar copias separadas de los datos de la aplicación o de los archivos de copia de seguridad que usted cree. Esas copias se rigen por las políticas del proveedor correspondiente.

## 5. Terceros, proveedores de servicios y venta

El desarrollador no vende contenido de bóvedas, contraseñas ni historial de actividad dentro de la aplicación, ni los proporciona a terceros a través de un servidor operado por el desarrollador.

Cuando funcionan las funciones de publicidad o consentimiento de Android, Google LLC, afiliadas de Google, proveedores de tecnología publicitaria y procesadores relacionados pueden procesar la información descrita en la Sección 2.4. Consulte el [Aviso de transferencia internacional de datos](policy/) separado.

Si selecciona directamente una aplicación externa o servicio en la nube mediante un selector de archivos, función de compartir o destino de copia de seguridad, ese proveedor puede procesar archivos bajo su dirección. Se aplican su política de privacidad y sus ajustes de seguridad, y el desarrollador no controla las prácticas del proveedor.

## 6. Transferencias internacionales de datos

El contenido de la bóveda no se transfiere a un servidor operado por el desarrollador. La información de publicidad y consentimiento puede ser procesada por Google y procesadores relacionados en Estados Unidos y otros países donde operen infraestructura.

Si elige un servicio en la nube extranjero como ubicación de una copia de seguridad cifrada, el archivo puede sincronizarse con servidores fuera de su país bajo su dirección. Consulte el [Aviso de transferencia internacional de datos](policy/) para obtener detalles.

## 7. Permisos

La aplicación puede usar los siguientes permisos o capacidades del sistema cuando usted use la función correspondiente:

- **Archivos y fotos:** Importar únicamente contenido que usted seleccione
- **Cámara:** Capturar fotos o videos para la bóveda
- **Micrófono:** Incluir audio al grabar video
- **Biometría:** Confirmar el acceso a la bóveda o cambios de ajustes sensibles
- **Internet y estado de red en Android:** Solicitar anuncios de AdMob e información de consentimiento de UMP
- **ID de publicidad en Android:** Admitir funciones publicitarias de Google
- **Portapapeles:** Copiar contenido o proteger texto del portapapeles cuando habilite explícitamente la protección automática

Denegar un permiso puede deshabilitar solo la función relacionada. Cuando se usa el selector de archivos del sistema, el acceso generalmente se limita a los elementos que usted seleccione.

## 8. Medidas de seguridad y limitaciones

La implementación actual usa medidas que incluyen:

- Cifrado AES-256-GCM para contenido e índices de bóveda
- Derivación de claves PBKDF2-HMAC-SHA256 para claves basadas en contraseña
- Protección Android Keystore o StrongBox para claves locales en dispositivos Android compatibles
- Cifrado con clave del dispositivo para ajustes sensibles e historial de actividad
- Bloqueo de bóveda y limpieza de archivos temporales y portapapeles según el mejor esfuerzo cuando la aplicación pasa a segundo plano
- Protección opcional contra capturas de pantalla y reautenticación biométrica
- Paquetes portátiles de copia de seguridad cifrados con contraseña

Ningún método de seguridad elimina todos los riesgos. El robo del dispositivo, malware, vulnerabilidades del sistema operativo, contraseñas débiles, archivos compartidos por usted o problemas de seguridad en un proveedor de almacenamiento externo pueden exponer información.

Abrir o exportar contenido descifrado a otra aplicación puede crear una copia separada. La eliminación del archivo original y la limpieza de archivos temporales o del portapapeles pueden estar restringidas por el sistema operativo, por lo que debe verificar la eliminación del contenido sensible.

## 9. Sus derechos y opciones

La mayor parte de la información permanece solo en su dispositivo, por lo que el desarrollador no puede acceder a ella, corregirla o eliminarla de forma remota. Usted puede:

- Eliminar elementos de bóveda o bóvedas en la aplicación
- Cambiar ajustes de seguridad, biometría, protección automática, portapapeles y copia de seguridad automática
- Borrar datos o caché de la aplicación, o desinstalarla
- Eliminar archivos de copia de seguridad y exportados desde su ubicación de almacenamiento
- Donde esté disponible, cambiar el consentimiento mediante las opciones de privacidad de anuncios de Google en la aplicación
- Eliminar o restablecer el identificador de publicidad o limitar la personalización de anuncios en los ajustes del dispositivo

Puede contactarnos en relación con la información que haya proporcionado directamente al desarrollador, como un correo electrónico de consulta. Cuando corresponda, la ley local puede otorgarle derechos de acceso, corrección, eliminación, restricción, retirada del consentimiento y reclamación ante una autoridad supervisora.

## 10. Niños

FileGuard no está diseñado principalmente para niños y no requiere que los niños proporcionen información personal. Los tutores pueden usar los controles parentales proporcionados por el dispositivo o la tienda de aplicaciones. La configuración de consentimiento de menores para publicidad de Android debe revisarse por separado frente al público previsto y la ley aplicable antes de la distribución.

## 11. Contacto

Para preguntas sobre esta Política:

- **Contacto:** frog-im
- **Correo electrónico:** [g.ns.0700g@gmail.com](mailto:g.ns.0700g@gmail.com)

Para datos publicitarios procesados por Google, use los controles de privacidad y procedimientos de contacto descritos en la [Política de privacidad de Google](https://policies.google.com/privacy).

## 12. Cambios en esta Política

Podemos actualizar esta Política cuando cambien las leyes, las funciones de la aplicación, los permisos o las prácticas de SDK de terceros. Los cambios materiales pueden comunicarse en esta página, en la aplicación o a través de la página de distribución.

Última actualización: **23 de junio de 2026**
