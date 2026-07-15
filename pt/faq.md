---
title: IFG GEO Optimizer
description: Documentação, FAQ e páginas legais do app Shopify IFG GEO Optimizer.
lang: pt
---

# Frequently Asked Questions

<div class="lang-switcher">
{% include lang-switcher.html current="pt" slug="faq" %}
</div>

**Qual é a diferença entre GEO e SEO?**
O SEO tradicional otimiza para motores de busca que classificam e listam links. O GEO (Generative Engine Optimization) otimiza para sistemas de IA que leem o seu conteúdo e geram uma resposta ou recomendação diretamente — ChatGPT, Perplexity, Gemini, Claude e Google AI Overviews. As duas disciplinas se sobrepõem, mas o GEO se importa com coisas que as ferramentas clássicas de SEO não verificam: se a página do produto tem dados estruturados completos, se um crawler de IA consegue realmente ler o seu conteúdo sem executar JavaScript, e se o seu texto é escrito de um jeito fácil de citar.

**O app chega a tocar nos dados dos meus clientes?**
Não, nenhum dado pessoal de clientes. As permissões Shopify do app são `read_products`, `write_products`, `read_themes` e `write_pixels` — ler e melhorar seu catálogo, verificar se o embed do tema está ativo, e ativar um pixel anônimo de tráfego da loja (veja abaixo). Ele nunca solicita pedidos ou registros de clientes. Veja a [Privacy Policy](privacy.html) para o detalhamento completo.

**O que é o pixel de tráfego de referência de IA, e ele rastreia meus clientes?**
No Grow e no Unlimited, um pequeno Web Pixel detecta quando uma visita à loja online chega a partir de um motor de IA conhecido (via referrer do navegador) e informa o motor, a página e um timestamp — nada que identifique o visitante, sem cookies, sem dados de sessão. Ele só é executado se o visitante já tiver dado consentimento de analytics através do banner de cookies da sua loja (Customer Privacy API da Shopify). É usado para exibir um cartão no Dashboard ("Tráfego de referência de IA, últimos 7 dias") — o complemento do rastreamento de Visibility AI, que diz se você é mencionado, mas não se essa menção enviou alguém.

**O que o botão "Fix" na auditoria do catálogo realmente altera?**
Ele grava dados estruturados schema.org ausentes em um metafield do produto — coisas como especificações técnicas derivadas das opções já existentes do produto. Ele nunca toca no título, na descrição, nas imagens ou no preço do seu produto, e nunca inventa dados que não consegue verificar: um código de barras ausente, por exemplo, permanece ausente em vez de ser adivinhado.

**As respostas de FAQ e as descrições reescritas são inventadas pela IA, ou baseadas no meu produto real?**
O modelo só vê os dados de produto que você já possui — título, descrição, fornecedor e especificações técnicas — e é explicitamente instruído a não acrescentar nada que não esteja presente nesses dados. Você revisa cada FAQ ou descrição reescrita antes que seja publicada; nada vai ao ar automaticamente.

**O que acontece com meus dados se eu desinstalar o app?**
A configuração da sua loja, as auditorias salvas, os rascunhos de FAQ e de reescrita de conteúdo, os prompts de visibilidade e os eventos de tráfego de referência de IA são excluídos automaticamente quando a Shopify nos notifica da desinstalação. O app não guarda nada depois que você sai.

**Posso cancelar ou fazer downgrade sem contatar o suporte?**
Sim. Vá em **Pricing** dentro do app e mude para o Free a qualquer momento — a mudança tem efeito imediato, sem necessidade de e-mail.

## Limites dos planos

| Funcionalidade | Free | Grow | Unlimited |
|---|---|---|---|
| Auditoria do catálogo | Primeiros 20 produtos, uma única vez, sem histórico | Catálogo completo + histórico | Catálogo completo + histórico |
| Simulador de crawler | 20/mês | 300/mês | 1.000/mês |
| Comparação com concorrentes | 10/mês | 50/mês | 150/mês |
| Geração de FAQ | Não incluído | 500/mês | 500/mês |
| Reescrita de conteúdo | Não incluído | 300/mês | 300/mês |
| Visibility AI (prompts rastreados) | Não incluído | 5 prompts | 15 prompts |
| Pixel de tráfego de referência de IA | Não incluído | Incluído | Incluído |
| Chat de suporte com IA | 1.000 mensagens/mês | 1.000 mensagens/mês | 1.000 mensagens/mês |
| Idiomas da interface | Todos os 30 | Todos os 30 | Todos os 30 |

Preços mensais: Free $0, Grow $9,99, Unlimited $19,99. A cobrança anual no Grow/Unlimited equivale a cerca de dois meses grátis em comparação com o pagamento mensal.

**Por que o plano Free só cobre 20 produtos?**
A ideia é deixar você ver resultados reais no seu próprio catálogo antes de se comprometer com um plano pago. Grow e Unlimited removem esse limite e mantêm um histórico completo das auditorias anteriores.

**Existe mesmo um limite para a geração de FAQ, mesmo no Unlimited?**
Sim — 500 gerações por mês, deliberadamente, mesmo no plano mais alto. Isso mantém a funcionalidade sustentável no preço atual; se você tem um catálogo de alto volume que precisa de mais, entre em contato e encontraremos uma solução.

**Por que o chat de suporte com IA é o mesmo em todos os planos?**
É uma decisão de produto, não um descuido: a assistência está incluída para todos, nunca é um diferencial pago. O limite de mensagens (1.000/mês) existe apenas como uma proteção técnica contra abuso, não como um limite real de uso — nenhum uso legítimo chega perto disso.

**Encontrei um bug ou algo parece errado. A quem devo avisar?**
Envie um e-mail para [info@ifgecommerce.com](mailto:info@ifgecommerce.com) com o que você viu e, se possível, qual produto ou página — geralmente isso já é suficiente para identificar o problema rapidamente. Você também pode usar o chat de suporte com IA dentro do app e pedir para falar com um humano.

[← Back to Help Center](index.html)
