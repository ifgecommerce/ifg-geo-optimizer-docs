---
title: IFG GEO Optimizer
description: Documentación, preguntas frecuentes y páginas legales de la app de Shopify IFG GEO Optimizer.
lang: es
---

# Preguntas frecuentes

<div class="lang-switcher">
{% include lang-switcher.html current="es" slug="faq" %}
</div>

**¿Cuál es la diferencia entre GEO y SEO?**
El SEO tradicional optimiza para motores de búsqueda que clasifican y listan enlaces. El GEO (Generative Engine Optimization) optimiza para sistemas de IA que leen tu contenido y generan directamente una respuesta o una recomendación — ChatGPT, Perplexity, Gemini, Claude y Google AI Overviews. Ambas disciplinas se solapan, pero el GEO se ocupa de aspectos que las herramientas SEO clásicas no comprueban: si tu página de producto tiene datos estructurados completos, si un crawler de IA puede leer realmente tu contenido sin ejecutar JavaScript, y si tus textos están escritos de forma que resulten fáciles de citar.

**¿La app accede alguna vez a los datos de mis clientes?**
No, a ningún dato personal de clientes. Los permisos de Shopify de la app son `read_products`, `write_products`, `read_themes` y `write_pixels` — para leer y mejorar tu catálogo, comprobar que el bloque de tema está activo, y activar un pixel anónimo de tráfico de la tienda (ver más abajo). Nunca solicita acceso a pedidos ni a fichas de clientes. Consulta la [Política de privacidad](privacy.html) para el detalle completo.

**¿Qué es el pixel de tráfico de referencia de IA, y hace seguimiento de mis clientes?**
En todos los planes, un pequeño Web Pixel detecta cuándo una visita a la tienda llega desde un motor de IA reconocido (a través del referrer del navegador) e informa del motor, la página y una marca de tiempo — nada que identifique al visitante, sin cookies, sin datos de sesión. Solo se ejecuta si el visitante ya ha dado su consentimiento de analítica a través del banner de cookies de tu tienda (Customer Privacy API de Shopify). Se usa para mostrar un panel en el Dashboard ("Tráfico de referencia de IA, últimos 7 días") — el complemento del seguimiento de Visibility AI, que te dice si te mencionan pero no si esa mención envió a alguien.

**¿Qué cambia realmente el botón "Corregir" del audit del catálogo?**
Escribe los datos estructurados schema.org que faltan en un metafield del producto — cosas como especificaciones técnicas derivadas de las opciones de producto ya existentes. Nunca toca el título, la descripción, las imágenes ni el precio de tu producto, y nunca inventa datos que no puede verificar: un código de barras que falta, por ejemplo, sigue faltando en lugar de ser adivinado.

**¿Las respuestas de las FAQ y las descripciones reescritas se las inventa la IA, o se basan en mi producto real?**
El modelo solo ve los datos de producto que ya tienes — título, descripción, proveedor y especificaciones técnicas — y recibe la instrucción explícita de no añadir nada que no esté presente en esos datos. Tú revisas cada FAQ o descripción reescrita antes de que se publique; nada se publica automáticamente.

**¿Qué pasa con mis datos si desinstalo la app?**
La configuración de tu tienda, los audits guardados, los borradores de FAQ y de reescritura de contenido, los prompts de visibilidad y los eventos de tráfico de referencia de IA se eliminan automáticamente cuando Shopify nos notifica la desinstalación. La app no conserva nada después de que te vayas.

**¿Puedo cancelar o bajar de plan sin contactar con soporte?**
Sí. Ve a **Precios** dentro de la app y cambia a Free en cualquier momento — el cambio se aplica de inmediato, sin necesidad de enviar ningún correo.

## Límites de los planes

| Función | Free | Grow | Unlimited |
|---|---|---|---|
| Audit del catálogo | Primeros 20 productos, una sola vez, sin historial | Catálogo completo + historial | Catálogo completo + historial |
| Simulador de crawler | 20/mes | 300/mes | 1,000/mes |
| Comparación con la competencia | 10/mes | 50/mes | 150/mes |
| Generación de FAQ | No incluido | 500/mes | 500/mes |
| Reescritura de contenido | No incluido | 300/mes | 300/mes |
| Visibility AI (prompts monitorizados) | No incluido | 5 prompts | 15 prompts |
| Pixel de tráfico de referencia de IA | Incluido | Incluido | Incluido |
| Chat de soporte con IA | 1,000 mensajes/mes | 1,000 mensajes/mes | 1,000 mensajes/mes |
| Idiomas de la interfaz | Los 30 | Los 30 | Los 30 |

Precio mensual: Free $0, Grow $9.99, Unlimited $19.99. La facturación anual en Grow/Unlimited equivale aproximadamente a dos meses gratis en comparación con el pago mensual.

**¿Por qué el plan Free solo cubre 20 productos?**
Su objetivo es que puedas ver resultados reales sobre tu propio catálogo antes de comprometerte con un plan de pago. Grow y Unlimited eliminan ese límite y conservan un historial completo de los audits anteriores.

**¿Hay realmente un límite en la generación de FAQ incluso en Unlimited?**
Sí — 500 generaciones al mes, de forma deliberada, incluso en el plan superior. Esto mantiene la funcionalidad sostenible al precio actual; si tienes un catálogo de gran volumen y necesitas más, ponte en contacto con nosotros y buscaremos una solución.

**¿Por qué el chat de soporte con IA es igual en todos los planes?**
Es una decisión de producto, no un descuido: la asistencia está incluida para todos, nunca es un diferenciador de pago. El límite de mensajes (1,000/mes) existe únicamente como salvaguarda técnica contra el abuso, no como un límite real de uso — ningún uso legítimo se acerca siquiera a él.

**He encontrado un error o algo no parece funcionar bien. ¿A quién se lo digo?**
Escribe a [info@ifgecommerce.com](mailto:info@ifgecommerce.com) contando lo que viste y, si puedes, qué producto o página estaba implicado — normalmente es suficiente para localizarlo rápidamente. También puedes usar el chat de soporte con IA dentro de la app y pedir hablar con una persona.

[← Volver al Centro de ayuda](index.html)
