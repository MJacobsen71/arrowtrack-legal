# Política de privacidad — JacArrow

**Última actualización:** 2026-05-20
**Responsable del tratamiento:** Morten Jacobsen, Noruega
**Contacto:** galge.vender.0a@icloud.com

---

## Versión corta

JacArrow almacena **todos tus datos localmente en tu dispositivo**. No tenemos
servidores que reciban tus tiros, sesiones u objetivos. Cuando desinstalas
la aplicación, todos los datos desaparecen.

Los únicos terceros que reciben información son:
- **Apple** — gestiona las compras de App Store y las notificaciones
- **RevenueCat** (después de comprar Pro) — verifica tu compra

Tienes todos los derechos RGPD de acceso, supresión y portabilidad de los datos.

---

## Qué almacenamos

### En tu dispositivo (localmente, nunca sale del teléfono)
- **Datos de tiro:** sesiones, rondas, posiciones de flechas, puntuaciones, etiquetas, objetivos, arcos y juegos de flechas
- **Ajustes:** idioma seleccionado, tema, mano dominante, categoría de competición, opciones de notificación
- **Historial de la app:** estado de los coach-marks (qué consejos has visto), indicadores de tutoriales completados

Todos estos datos se almacenan en una base de datos SQLite y en AsyncStorage en tu iPhone.
Ni JacArrow ni ningún tercero tiene acceso a estos datos.

### iCloud (solo si iCloud Drive está activado)
JacArrow planea usar iCloud Key-Value Storage para un propósito específico:
recordar si ya has iniciado el período de prueba. Esto se sincroniza
a través de tu cuenta iCloud para impedir que desinstalar + reinstalar
conceda un nuevo período de prueba gratuito.

- Apple es el encargado del tratamiento (nuestro acuerdo se rige por sus términos estándar)
- Los valores almacenados son **únicamente**: la fecha de inicio de la prueba y un estado «prueba usada»
- Esta función se activará cuando lancemos el modelo Pro (Fase 4b)

Si has desactivado iCloud Drive, o desactivado iCloud Drive específicamente
para JacArrow, no se usa iCloud.

---

## Terceros

### Apple App Store
Todas las compras dentro de la app las gestiona Apple. Nunca recibimos información
de tarjeta, direcciones u otros detalles de pago. La
[política de privacidad de Apple](https://www.apple.com/es/legal/privacy/) se aplica al
proceso de compra.

### Apple Push Notification Service (APNS)
JacArrow envía notificaciones locales (RP conseguido, expiración del período de prueba,
recordatorios de objetivos). Para entregarlas, iOS registra un token de dispositivo anónimo
con Apple. No tenemos servidores que envíen mensajes push — todas las notificaciones
se generan localmente en tu dispositivo según el estado de la app.

### RevenueCat (solo después de comprar Pro)
Cuando compras JacArrow Pro, RevenueCat registra tu recibo y un
`appUserId` anónimo (UUID generado en tu dispositivo). Esto es necesario
para que la app pueda verificar tu compra en usos posteriores y durante «Restaurar
compras». La
[política de privacidad de RevenueCat](https://www.revenuecat.com/privacy) se aplica. Nunca enviamos
tu nombre, correo electrónico u otros datos personales.

### Apple Analytics / Informes de fallos
Si has activado «Compartir análisis de la app» en los Ajustes de iOS, Apple envía
datos agregados anónimos sobre uso y fallos al desarrollador.
JacArrow los usa para corrección de errores y optimización de rendimiento. Puedes
desactivarlo en:
**Ajustes de iOS → Privacidad y seguridad → Análisis y mejoras**.

---

## Lo que NO recopilamos

- Ninguna cuenta de usuario, correo electrónico ni contraseña
- Ningún dato de GPS ni de ubicación
- Ningún acceso a contactos, calendario, cámara o micrófono
- Ningún rastreador de terceros (Firebase, Google Analytics, Facebook Pixel, etc.)
- Ningún identificador publicitario (IDFA)
- Ningún seguimiento de vídeo ni huella digital del dispositivo

---

## Tus derechos (RGPD)

Tienes los siguientes derechos en virtud del Reglamento General de Protección de Datos:

**Derecho de acceso (Art. 15):** Todos tus datos están almacenados localmente en tu dispositivo.
Tienes visibilidad completa a través de:
- Ajustes → Mis sesiones (todas las rondas históricas)
- Ajustes → Mis objetivos (todos los objetivos activos y archivados)
- Ajustes → Arcos / Juegos de flechas / Campos (gestión del equipamiento)

**Derecho a la portabilidad de los datos (Art. 20):** Usa
**Ajustes → Exportar mis datos** para descargar todos tus datos como archivo JSON.
El archivo se puede compartir a través de la hoja de compartir de iOS por correo, AirDrop, Archivos, etc.
Esta es tu historia de tiro completa en formato estándar.

**Derecho de supresión (Art. 17):**
- *Eliminar una sesión individual:* desliza la sesión en la pantalla principal → Eliminar
- *Eliminar todos los datos:* desinstala JacArrow — iOS elimina automáticamente toda
  la base de datos SQLite y AsyncStorage. El recibo de RevenueCat (si has
  comprado Pro) lo conservan Apple y RevenueCat para fines de reembolso y soporte.

**Derecho de limitación y oposición (Art. 18–21):** JacArrow no toma
ninguna decisión automatizada sobre ti. El motor Smart Insights solo analiza
tus propios datos de entrenamiento localmente en tu dispositivo y presenta
observaciones — no toma decisiones en tu nombre.

**Derecho a retirar el consentimiento (Art. 7):** El opt-in de Apple Analytics se controla
a través de los Ajustes de iOS. Los datos de RevenueCat se eliminan cuando eliminas tu ID de Apple.

---

## Cambios

Actualizaremos esta política cuando se produzcan cambios significativos en cómo procesamos
los datos. Los cambios se comunican mediante:
1. Fecha «Última actualización» en la parte superior de esta página
2. Banner in-app en el primer arranque después de la actualización si el cambio es sustancial
   (p. ej. nuevos terceros, nueva recopilación de datos)

---

## Reclamaciones

Si crees que estamos tratando tus datos personales en violación del RGPD,
tienes derecho a presentar una reclamación ante tu autoridad nacional de protección de datos:

- **España:** [Agencia Española de Protección de Datos (AEPD)](https://www.aepd.es/)
- **UE/EEE:** encuentra tu autoridad en
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Te animamos a contactarnos primero en galge.vender.0a@icloud.com — nos tomamos
todas las consultas de privacidad en serio.
