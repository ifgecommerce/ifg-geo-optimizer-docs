---
title: IFG GEO Optimizer
description: Documentación, preguntas frecuentes y páginas legales de la app de Shopify IFG GEO Optimizer.
---

# Privacy Policy

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <a class="lang-item" href="../it/"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <a class="lang-item" href="../de/"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <a class="lang-item" href="../fr/"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <span class="lang-item lang-current"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</span>
</div>

**IFG GEO Optimizer** — una app de Shopify para la Generative Engine Optimization
Última actualización: julio de 2026

## 1. Responsable del tratamiento

El responsable del tratamiento de los datos personales procesados a través de **IFG GEO Optimizer** es:

**IFG eCommerce**
Con sede en Roma, Italia
Correo electrónico: [ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

## 2. Qué recopilamos

- **Datos de la cuenta del comerciante (vía OAuth de Shopify)**: el dominio de tu tienda, un token de acceso a la API y la dirección de correo electrónico de tu cuenta de Shopify.
- **Datos del catálogo (solo lectura)**: títulos, descripciones, proveedor, precios, opciones y especificaciones técnicas de los productos — usados para ejecutar audits, simular el comportamiento de los crawlers, puntuar la extraibilidad del contenido y redactar FAQ.
- **Configuración de la tienda**: tu plan activo, los datos de política de devoluciones y envío que introduces en Configuración, y cualquier borrador o aprobación de FAQ que crees.
- **Datos técnicos**: marcas de tiempo de las solicitudes, identificadores internos de registro y logs del sistema.

> La app nunca solicita ni recibe datos de clientes finales — ni nombres, correos, direcciones ni pedidos. Los únicos permisos de Shopify solicitados son `read_products` y `write_products`.

## 3. Por qué lo procesamos, y bajo qué base legal

Procesamos estos datos para prestar el servicio para el que instalaste la app — conforme al Art. 6(1)(b) RGPD, ejecución de un contrato: analizar y mejorar la visibilidad de tu catálogo en los motores de búsqueda generativos (ChatGPT, Perplexity, Gemini, Google AI Overviews), incluida la redacción de FAQ cuando lo solicitas explícitamente.

## 4. Cómo lo recopilamos

Los datos de la cuenta se recopilan una sola vez, a través del flujo OAuth de Shopify, cuando instalas la app. Los datos del catálogo se leen a través de la Admin API de Shopify solo cuando activas una acción — un escaneo, una simulación o una generación de FAQ — desde el panel de la app. Nada se ejecuta en segundo plano sin que tú lo pidas.

## 5. Con quién lo compartimos

- **Google Firebase / Cloud Firestore** — almacena la configuración de tu tienda, las sesiones y los borradores de FAQ. Google LLC (EE. UU.) participa en el Marco de Privacidad de Datos UE-EE. UU. Los datos se almacenan en la región europe-west1 (Bélgica).
- **Anthropic PBC (EE. UU.)** — proporciona el modelo de lenguaje (Claude) usado para redactar las sugerencias de FAQ, solo cuando lo solicitas explícitamente. Recibe únicamente los atributos de producto que ya has introducido — título, descripción, proveedor, especificaciones — nunca datos de clientes. Consulta la propia política de privacidad y las condiciones comerciales de Anthropic para saber cómo gestionan esos datos.
- **Shopify Inc.** — la propia plataforma, y la fuente de la Admin API que usa la app.

No vendemos datos, ni los usamos con fines de marketing o de perfilado conductual.

## 6. Cuánto tiempo los conservamos

- **Tokens de sesión**: gestionados por el ciclo de vida de los tokens offline de Shopify, renovados automáticamente.
- **Configuración, audits y borradores de FAQ**: se conservan mientras la app esté instalada. Al desinstalarla se activa el webhook `shop/redact` de Shopify, que elimina por completo la configuración y las sesiones de tu tienda.
- **Logs técnicos**: conservados conforme a la política de retención de logs estándar de Google Cloud.

## 7. Tus derechos

Conforme a los Artículos 15–22 del RGPD, puedes solicitar el acceso a tus datos, la corrección de datos inexactos o su eliminación — la forma más sencilla es desinstalar la app — u oponerte al tratamiento. También puedes presentar una reclamación ante tu autoridad local de protección de datos. Dado que la app nunca procesa datos de clientes finales, los webhooks de cumplimiento `customers/data_request` y `customers/redact` responden confirmando que no hay nada que exportar ni eliminar.

## 8. Seguridad

Todo el tráfico circula por HTTPS/TLS 1.2+. Los tokens de autenticación de Shopify nunca se exponen al navegador. Cada webhook se verifica con una comprobación HMAC SHA-256 en tiempo constante antes de procesarse. La base de datos solo es accesible desde el backend, autenticado mediante la propia identidad de servicio de la plataforma de hosting — no hay credenciales estáticas en el código, y el acceso directo desde el cliente está denegado por las propias reglas de seguridad de la base de datos. Los datos se cifran tanto en reposo como en tránsito.

## 9. Cambios

Podemos actualizar esta política de vez en cuando. Los cambios sustanciales se reflejarán aquí, manteniendo siempre actualizada la fecha en la parte superior.

---

**¿Preguntas sobre tus datos?**
[ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

[← Volver al Centro de ayuda](index.html)
