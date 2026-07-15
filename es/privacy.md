---
title: IFG GEO Optimizer
description: Documentación, preguntas frecuentes y páginas legales de la app de Shopify IFG GEO Optimizer.
lang: es
---

# Política de privacidad

<div class="lang-switcher">
{% include lang-switcher.html current="es" slug="privacy" %}
</div>

**IFG GEO Optimizer** — una app de Shopify para la Generative Engine Optimization
Última actualización: julio de 2026

## 1. Responsable del tratamiento

El responsable del tratamiento de los datos personales procesados a través de **IFG GEO Optimizer** es:

**IFG eCommerce** — con sede en Roma, Italia
Correo electrónico: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Qué recopilamos

- **Datos de la cuenta del comerciante (vía OAuth de Shopify)**: el dominio de tu tienda, un token de acceso a la API y la dirección de correo electrónico de tu cuenta de Shopify.
- **Datos del catálogo (solo lectura)**: títulos, descripciones, proveedor, precios, opciones y especificaciones técnicas de los productos — usados para ejecutar audits, simular el comportamiento de los crawlers, puntuar la extraibilidad del contenido y redactar FAQ o descripciones reescritas.
- **Configuración de la tienda**: tu plan activo, los datos de política de devoluciones y envío y la información de empresa que introduces en Configuración, los audits guardados, los borradores de FAQ y de reescritura de contenido, y los prompts que eliges monitorizar para la visibilidad en IA.
- **Mensajes del chat de soporte**: el texto que intercambias con el asistente de IA dentro de la app, incluida la transcripción que nos reenvías si pides explícitamente hablar con una persona.
- **Tráfico anónimo de la tienda (Web Pixel, Grow/Unlimited)**: cuando un visitante llega a una página de producto desde un motor de IA reconocido (ChatGPT, Perplexity, Claude, Gemini, Copilot), registramos el motor, la URL de la página y una marca de tiempo — solo si el visitante ya ha dado su consentimiento de analítica a través del banner de cookies de tu tienda. No se recopila ningún identificador de visitante, cookie ni dato de sesión.
- **Datos técnicos**: marcas de tiempo de las solicitudes, identificadores internos de registro y logs del sistema.

> La app **nunca solicita ni recibe datos personales de clientes finales** — ni nombres, correos, direcciones ni pedidos. Los permisos de Shopify solicitados son `read_products`, `write_products` (catálogo y datos estructurados), `read_themes` (comprobar que el bloque de tema está activo) y `write_pixels` (activar el pixel anónimo de tráfico descrito arriba).

## 3. Por qué lo procesamos, y bajo qué base legal

Procesamos estos datos para prestar el servicio para el que instalaste la app — conforme al Art. 6(1)(b) RGPD, ejecución de un contrato: analizar y mejorar la visibilidad de tu catálogo en los motores de búsqueda generativos, incluida la redacción de FAQ asistida por IA y la reescritura de contenido, el chat de soporte dentro de la app, el seguimiento semanal de visibilidad en IA sobre los prompts que eliges, y la medición anónima del tráfico de referencia de IA — todo ello iniciado por el comerciante o, en el caso del pixel de tráfico, sujeto al consentimiento en tu tienda online.

## 4. Cómo lo recopilamos

Los datos de la cuenta se recopilan una sola vez, a través del flujo OAuth de Shopify, al instalar la app. Los datos del catálogo se leen a través de la Admin API de Shopify solo cuando activas una acción desde el panel. El pixel de tráfico se ejecuta en tu tienda online e informa de eventos solo tras el consentimiento; nada más se ejecuta en segundo plano sin que tú lo pidas.

## 5. Con quién lo compartimos

- **Google Firebase / Cloud Firestore** — almacena tu configuración, sesiones y borradores. Google LLC (EE. UU.) participa en el Marco de Privacidad de Datos UE-EE. UU. Los datos se almacenan en la región europe-west1 (Bélgica).
- **Anthropic PBC (EE. UU.)** — proporciona el modelo Claude usado para la redacción de FAQ, la reescritura de contenido y el chat de soporte dentro de la app, solo cuando realizas una acción explícita. Recibe únicamente los atributos de producto o el texto del chat que proporcionas — nunca datos de clientes.
- **OpenAI, Inc. (EE. UU.)** y **Perplexity AI, Inc. (EE. UU.)** — usados exclusivamente para el seguimiento semanal de visibilidad en IA sobre los prompts que eliges explícitamente monitorizar. Reciben únicamente el texto de los prompts monitorizados — nunca datos de clientes.
- **Google LLC (EE. UU.)** — proporciona el modelo Gemini, usado del mismo modo que OpenAI/Perplexity arriba para el seguimiento de visibilidad (un uso distinto de Firebase/Firestore, que es solo almacenamiento).
- **Resend, Inc. (EE. UU.)** — nos envía una notificación, con el nombre de la tienda y la transcripción del chat de soporte, solo cuando pides explícitamente hablar con una persona en el chat de soporte.
- **Shopify Inc.** — la propia plataforma, y la fuente de la Admin API y de la infraestructura de Web Pixel que usa la app.

No vendemos datos, ni los usamos con fines de marketing o de perfilado conductual.

## 6. Cuánto tiempo los conservamos

- **Tokens de sesión**: gestionados por el ciclo de vida de los tokens offline de Shopify, renovados automáticamente.
- **Configuración, audits, borradores y eventos de tráfico**: se conservan mientras la app esté instalada. Desinstalarla activa el webhook `shop/redact` de Shopify, que elimina por completo la configuración y las sesiones de tu tienda.
- **Logs técnicos**: conservados conforme a la política de retención de logs estándar de Google Cloud.

## 7. Tus derechos

Conforme a los Artículos 15–22 del RGPD, puedes solicitar el acceso a tus datos, la corrección de datos inexactos o su eliminación — la forma más sencilla es desinstalar la app — u oponerte al tratamiento. También puedes presentar una reclamación ante tu autoridad local de protección de datos. Dado que la app nunca procesa datos personales de clientes finales, los webhooks de cumplimiento `customers/data_request` y `customers/redact` responden confirmando que no hay nada que exportar ni eliminar.

## 8. Seguridad

Todo el tráfico circula por HTTPS/TLS 1.2+. Los tokens de autenticación de Shopify nunca se exponen al navegador. Cada webhook se verifica con una comprobación HMAC SHA-256 en tiempo constante antes de procesarse. La base de datos solo es accesible desde el backend, autenticado mediante la propia identidad de servicio de la plataforma de hosting — no hay credenciales estáticas en el código, y el acceso directo desde el cliente está denegado por las propias reglas de seguridad de la base de datos. Los datos se cifran tanto en reposo como en tránsito.

## 9. Cambios

Podemos actualizar esta política de vez en cuando. Los cambios sustanciales se reflejarán aquí, manteniendo siempre actualizada la fecha en la parte superior.

---

**¿Preguntas sobre tus datos?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Volver al Centro de ayuda](index.html)
