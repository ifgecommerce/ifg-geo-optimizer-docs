---
title: IFG GEO Optimizer
description: Documentación, preguntas frecuentes y páginas legales de la app de Shopify IFG GEO Optimizer.
---

# Primeros pasos

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <a class="lang-item" href="../it/"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <a class="lang-item" href="../de/"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <a class="lang-item" href="../fr/"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <span class="lang-item lang-current"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</span>
</div>

Esta guía recorre todo el proceso, desde instalar la app hasta publicar tu primera FAQ optimizada para IA.

## 1. Instala y abre el panel

Una vez instalada, IFG GEO Optimizer se abre dentro de tu admin de Shopify. El panel es tu base de operaciones — se va completando con la puntuación GEO de tu tienda y la actividad reciente a medida que usas la app.

## 2. Completa tus políticas

Ve a **Configuración** e introduce los datos de tu política de devoluciones y de envío (plazo de devolución, quién paga el envío de vuelta, tiempos de gestión y de tránsito, país de destino). Estos datos alimentan directamente los datos estructurados que la app publica en cada producto — las páginas de producto de Shopify no exponen esta información a los motores de búsqueda por sí solas, así que este solo paso ya mejora de forma medible tu puntuación de audit.

## 3. Ejecuta tu primer audit del catálogo

Abre **Audit del catálogo** y haz clic en **Reescanear catálogo**. La app lee tu catálogo de productos a través de la Admin API de Shopify y comprueba cada producto frente a nueve campos de datos estructurados que buscan los motores de búsqueda: imagen, descripción, marca, SKU, GTIN, precio, especificaciones técnicas, política de devoluciones y política de envío.

Los productos por debajo de 80/100 muestran exactamente qué falta. Cuando la app puede corregirlo automáticamente — normalmente derivando especificaciones técnicas a partir de las opciones de producto ya existentes — verás un botón **Corregir**. Un solo clic escribe los datos schema.org que faltan directamente en el producto; nada se supone ni se inventa en los campos que la app no puede derivar con seguridad (un código de barras, por ejemplo, nunca se genera automáticamente).

En el plan Free, los audits cubren tus primeros 20 productos y no conservan historial. Grow y Unlimited cubren todo tu catálogo y guardan cada escaneo.

## 4. Activa el bloque de tema

Los datos estructurados que corrige tu audit no aparecen en tu tienda online hasta que los actives. En el editor de temas, ve a **Bloques de la app** y activa **GEO Schema**. Es un interruptor que se activa una sola vez — a partir de ahí, cada página de producto incluye automáticamente el JSON-LD generado por tu audit.

## 5. Comprueba lo que realmente ve un bot

Abre **Crawler IA** y elige un producto. La app obtiene la página exactamente igual que lo hace un crawler de IA — sin ejecutar JavaScript, igual que GPTBot, ClaudeBot o PerplexityBot — para que veas con precisión qué es visible para estos motores, incluyendo si tu robots.txt los está bloqueando y si tus datos estructurados están completos en el HTML en bruto.

## 6. Genera FAQs

En Grow o Unlimited, abre **FAQ de producto**, elige un producto y haz clic en **Generar 3 FAQs**. La app redacta tres pares de pregunta y respuesta a partir del título, la descripción y las especificaciones reales de tu producto — nunca a partir de detalles inventados. Revisa cada borrador y luego pulsa **Aprobar y publicar** en las que quieras dejar activas; las FAQs aprobadas aparecen en la página de producto y se marcan como datos estructurados FAQPage para los motores de búsqueda. Nada se publica sin tu revisión.

## 7. Elige un plan

**Precios** muestra Free, Grow y Unlimited en paralelo, con facturación mensual y anual. Puedes cambiar de plan o volver a Free en cualquier momento, directamente desde la app — sin necesidad de contactar con soporte para bajar de plan.

Ese es el ciclo completo. La mayoría de los comerciantes vuelve a ejecutar un audit después de añadir nuevos productos, y revisa el simulador de crawler cada vez que actualiza una descripción de producto.

[← Volver al Centro de ayuda](index.html)
