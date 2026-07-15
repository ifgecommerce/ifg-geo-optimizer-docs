---
title: IFG GEO Optimizer
description: Documentación, preguntas frecuentes y páginas legales de la app de Shopify IFG GEO Optimizer.
lang: es
---

# Registro de cambios

<div class="lang-switcher">
{% include lang-switcher.html current="es" slug="changelog" pages="en,it,de,fr,es" %}
</div>

Todos los cambios que llegan a los comerciantes, del más reciente al más antiguo. Esta es documentación técnica, disponible en 5 idiomas (inglés, italiano, alemán, francés y español) en lugar de los 30 que admite el resto del Centro de ayuda.

## Julio 2026

**Seguimiento del tráfico de referencia de IA** — Añadido un Web Pixel (Grow/Unlimited) que detecta las visitas a la tienda que llegan desde un motor de IA reconocido (ChatGPT, Perplexity, Claude, Gemini, Copilot) y las muestra en un nuevo panel del Dashboard, sujeto a consentimiento y totalmente anónimo — el complemento del seguimiento de Visibility AI: no solo "¿nos mencionan?", sino "¿esa mención está enviando a alguien?".

**Mejoras en el Dashboard y la navegación** — Añadido un empty state adecuado para el primer uso, un skeleton de carga durante la navegación entre páginas, y un desglose por bot en la página del crawler que muestra si una regla de `robots.txt` se ha detectado por nombre o heredado del grupo comodín.

**Rediseño del onboarding** — La barra de progreso del asistente de configuración se convirtió en una checklist paso a paso, con un banner de confirmación visible al completarla en lugar de una recarga instantánea y sin confirmación.

**Facturación y correo de soporte** — El contacto de soporte y privacidad se trasladó a `info@ifgecommerce.com`.

**Internal Link & Entity Graph Coach** — Nuevo análisis de qué tan bien se conectan los productos entre sí a través de colecciones, proveedores y etiquetas compartidas, con sugerencias explicables y un resumen en el Dashboard.

**Readiness Matrix** — El Dashboard incorporó un único panel de un vistazo que agrega todas las señales GEO que rastrea la app: extraibilidad del contenido, schema de Organización, `llms.txt`, `agents.md`, acceso de crawlers, preparación MCP, conectividad de Link Coach y (una vez publicado) tráfico de referencia de IA.

**Motor de reescritura de contenido** — Añadida una herramienta asistida por IA para reescribir una descripción de producto y hacerla más densa en hechos verificables y más fácil de citar para un motor generativo, con una revisión antes/después obligatoria antes de escribir nada de vuelta.

**Comparación con la competencia** — Pega la URL de producto de un competidor y ve las mismas señales GEO comparadas en paralelo con tu propio producto.

**Seguimiento de Visibility AI** — Comprobaciones semanales automatizadas de si Claude, ChatGPT, Gemini y Perplexity mencionan tu tienda en los prompts que eliges monitorizar, con un gráfico de tendencia y un desglose por motor.

**Schema de Organización y `agents.md`** — Añadidos datos estructurados de identidad de empresa (razón social, NIF/CIF, dirección) para que los sistemas de IA verifiquen que un negocio es real, y un archivo `agents.md` generado que describe la tienda a los agentes de compra autónomos.

**Facturación** — Los comerciantes pueden suscribirse a Grow o Unlimited, con facturación mensual o anual, directamente desde la página de Precios, y volver a Free en cualquier momento sin contactar con soporte.

**Revisión de la política de privacidad y cumplimiento del App Store** — Publicado este Centro de ayuda y una política de privacidad formal; confirmado que los permisos de Shopify de la app y la gestión de webhooks RGPD cumplen los requisitos del App Store de cara al envío.

**Generación de FAQ asistida por IA** — Genera de tres a cinco pares de pregunta y respuesta por producto a partir de su título, descripción y especificaciones existentes, revísalos y publica los que apruebes. Las FAQ publicadas aparecen en la página de producto y como datos estructurados `FAQPage`.

**Puntuación de extraibilidad del contenido (chunking)** — El audit del catálogo ahora también puntúa lo fácil que resulta para un sistema de IA extraer y citar la descripción de cada producto — no solo si están presentes los campos de datos estructurados, sino si el propio texto es aprovechable.

**Simulador de crawler** — Obtén cualquier página de producto exactamente como la ve un crawler de IA — sin JavaScript, igual que GPTBot, ClaudeBot y PerplexityBot — incluidas las comprobaciones de `robots.txt` por bot.

**Audit del catálogo y correcciones con un clic** — Lanzado el audit principal: analiza tu catálogo frente a nueve campos de datos estructurados, puntúa cada producto y corrige con un clic todo lo que puede hacerlo de forma segura. Añadida también la generación real de `llms.txt`, servido en la raíz real de tu tienda.

## Versiones anteriores

Lanzamiento inicial: configuración de la app embebida, autenticación de Shopify e infraestructura de datos subyacente.

[← Volver al Centro de ayuda](index.html)
