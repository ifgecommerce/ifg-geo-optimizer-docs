---
title: IFG GEO Optimizer
description: Documentación, preguntas frecuentes y páginas legales de la app de Shopify IFG GEO Optimizer.
lang: es
---

# Primeros pasos

<div class="lang-switcher">
{% include lang-switcher.html current="es" slug="getting-started" %}
</div>

IFG GEO Optimizer tiene nueve áreas, todas accesibles desde la navegación superior una vez completada la configuración: **Panel**, **Audit del catálogo**, **Crawler IA**, **FAQ de producto**, **Link Coach**, **Visibility AI**, **Precios**, **Configuración** y **Soporte**. Esta guía las recorre todas, en el orden en que la mayoría de los comerciantes las usa.

## 1. Instala y completa el asistente de configuración

Al abrir la app por primera vez, un breve asistente guiado (unos 2 minutos) recopila los datos básicos: idioma de la interfaz, los detalles de tu política de devoluciones y de envío, la información de tu empresa y — el único paso que realmente importa a nivel técnico — la activación del bloque de app **GEO Schema** en el editor de temas. Nada de lo que la app hace después llega a tu tienda online hasta que este bloque está activado, así que vale la pena no saltárselo. Siempre puedes cambiar cualquiera de estas respuestas más tarde desde **Configuración**.

## 2. Panel

Tu base de operaciones. Muestra tu puntuación GEO actual (de tu último audit), una **Readiness Matrix** con ocho señales de un vistazo — extraibilidad del contenido, schema de Organización, `llms.txt`, `agents.md`, acceso de crawlers, preparación MCP, conectividad de Link Coach y tráfico de referencia de IA — además de una lista priorizada de "qué corregir primero" y los contadores de uso de tu plan (generaciones de FAQ, tamaño del catálogo). Todo aquí enlaza directamente a la página donde puedes actuar sobre ello.

## 3. Audit del catálogo

Haz clic en **Reescanear catálogo** para comprobar cada producto frente a nueve campos de datos estructurados que buscan los motores de búsqueda: imagen, descripción, marca, SKU, GTIN, precio, especificaciones técnicas, política de devoluciones y política de envío. Los productos por debajo de 80/100 muestran exactamente qué falta.

- **Corrección con un clic**: cuando la app puede derivar con seguridad los datos que faltan (normalmente especificaciones técnicas a partir de las opciones de producto ya existentes), verás un botón **Corregir** que los escribe directamente en los datos estructurados del producto. Nada se supone en los campos que la app no puede verificar — un código de barras que falta, por ejemplo, sigue faltando en lugar de ser inventado.
- **Puntuación de content chunking**: junto con la comprobación de datos estructurados, cada producto recibe una puntuación de extraibilidad independiente — no "¿está presente el campo?" sino "¿puede un sistema de IA/RAG extraer realmente un hecho limpio de esta descripción?". Un texto pobre y cargado de adjetivos puntúa más bajo incluso con un marcado schema.org perfecto.
- **`llms.txt`**: genera un archivo `llms.txt` real, conforme al estándar, que resume tu catálogo para los sistemas de IA, servido en la raíz real de tu tienda (`/llms.txt`), no escondido bajo una ruta de app proxy donde los crawlers no lo encontrarían.
- **`agents.md`**: genera un archivo que describe tu tienda a los agentes de compra autónomos — variantes, búsqueda, checkout — construido únicamente a partir de datos reales que tu tienda ya expone, nada inventado.
- **Schema de Organización**: publica los datos de tu empresa (razón social, NIF/CIF, dirección) como datos estructurados, para que los motores de IA puedan verificar que eres un negocio real y responsable antes de recomendarte.

En el plan Free, los audits cubren tus primeros 20 productos, una sola vez, sin conservar historial. Grow y Unlimited analizan todo tu catálogo y guardan cada escaneo anterior para comparar tendencias.

## 4. Crawler IA

Elige un producto y la app obtiene su página exactamente igual que lo hace un crawler de IA — sin ejecutar JavaScript, igual que GPTBot, ClaudeBot o PerplexityBot — para que veas con precisión qué es visible para estos motores: si tu `robots.txt` los bloquea (comprobado por bot, no solo un allow/deny genérico), y si tus datos estructurados realmente sobreviven en el HTML en bruto que leen estos bots.

**Comparación con la competencia** (en su propia pestaña desde esta página): pega la URL de producto de un competidor y obtén las mismas señales GEO comparadas en paralelo con las tuyas — la misma diferencia cualitativa que obtendrías de un audit manual, sin necesidad de registrarte en las herramientas del propio competidor.

## 5. FAQ de producto

En Grow o Unlimited, elige un producto y haz clic en **Generar FAQs** para obtener de tres a cinco pares de pregunta y respuesta redactados únicamente a partir del título, la descripción, el proveedor y las especificaciones reales de ese producto — al modelo se le indica explícitamente que nunca añada un detalle que no esté ya en tus datos. Revisa cada borrador; nada se publica sin tu **Aprobación** explícita. Las FAQs aprobadas aparecen en la página de producto en vivo y se marcan como datos estructurados `FAQPage`, de modo que son legibles tanto por personas como citables por máquinas.

**Reescritura de contenido** (en su propia pestaña desde esta página): la app puede reescribir una descripción de producto para que sea más densa en hechos verificables y más fácil de citar para un motor generativo — siempre ves una comparación antes/después y apruebas antes de que se escriba nada de vuelta en el producto.

## 6. Link Coach

Analiza qué tan bien están conectados tus productos entre sí a través de colecciones, proveedores y etiquetas compartidas — el enlazado interno es una señal que los sistemas de IA usan para entender lo que cubre tu catálogo en su conjunto, no solo página por página. Muestra los productos huérfanos sin conexiones significativas y sugerencias explicables para solucionarlo.

## 7. Visibility AI

Añade hasta un puñado de prompts que razonablemente esperarías que un cliente le hiciera a un asistente de IA (el límite depende de tu plan — consulta Precios más abajo), y cada semana la app comprueba si Claude, ChatGPT, Gemini y Perplexity mencionan tu tienda en la respuesta, con seguimiento en el tiempo por motor. En Grow y Unlimited, esto también muestra cómo te comparas con competidores concretos en los mismos prompts.

**Tráfico de referencia de IA** (Grow y Unlimited): un pixel ligero y respetuoso con la privacidad detecta cuándo una visita a la tienda proviene realmente de uno de estos motores de IA (a través del referrer, solo después de que el visitante haya dado su consentimiento de analítica mediante el banner de cookies de tu tienda) e informa de cuántas visitas de este tipo has tenido en los últimos 7 días — la segunda mitad del ciclo que el seguimiento de visibilidad por sí solo no puede mostrar: no solo "¿nos mencionan?", sino "¿esa mención está enviando a alguien?".

## 8. Soporte

Un asistente de chat con IA vive dentro de la app (icono inferior derecho) para preguntas sobre GEO, los resultados de tu audit o cómo funciona una función concreta. Si no puede ayudarte, puedes pedir hablar con una persona y la conversación se reenvía directamente a IFG eCommerce.

## 9. Configuración

Donde gestionas las respuestas del asistente de configuración (políticas, datos de empresa, idioma de la interfaz — cambia al instante entre 30 idiomas, sin retraso de recarga), vuelves a comprobar la activación del bloque de tema y ves los scopes de Shopify de tu cuenta.

## 10. Precios

**Precios** muestra Free, Grow y Unlimited en paralelo, con facturación mensual o anual (la anual equivale aproximadamente a 2 meses gratis en ambos planes de pago). Puedes subir de plan, bajar de plan o volver a Free en cualquier momento, directamente desde la app — sin necesidad de enviar ningún correo. Consulta las [Preguntas frecuentes](faq.html) para los límites exactos de cada plan.

Ese es el ciclo completo. La mayoría de los comerciantes vuelve a ejecutar un audit después de añadir nuevos productos, revisa el simulador de crawler cada vez que actualiza una descripción y le echa un vistazo semanal a la Readiness Matrix del Panel.

[← Volver al Centro de ayuda](index.html)
