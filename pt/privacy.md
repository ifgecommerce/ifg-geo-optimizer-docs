---
title: IFG GEO Optimizer
description: Documentação, FAQ e páginas legais do app Shopify IFG GEO Optimizer.
lang: pt
---

# Privacy Policy

<div class="lang-switcher">
{% include lang-switcher.html current="pt" slug="privacy" %}
</div>

**IFG GEO Optimizer** — um app Shopify para Generative Engine Optimization
Última atualização: julho de 2026

## 1. Controlador dos dados

O controlador dos dados pessoais tratados através do **IFG GEO Optimizer** é:

**IFG eCommerce** — sediada em Roma, Itália
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. O que coletamos

- **Dados da conta do lojista (via Shopify OAuth)**: o domínio da sua loja, um token de acesso à API e o e-mail associado à sua conta Shopify.
- **Dados do catálogo (somente leitura)**: títulos de produtos, descrições, fornecedor, preços, opções e especificações técnicas — usados para executar auditorias, simular o comportamento de crawlers, pontuar a extratibilidade do conteúdo e redigir FAQs ou descrições reescritas.
- **Configuração da loja**: seu plano ativo, os detalhes da política de devolução e envio e os dados da empresa que você insere em Settings, as auditorias salvas, os rascunhos de FAQ e de reescrita de conteúdo, e os prompts que você escolhe rastrear para a visibilidade em IA.
- **Mensagens do chat de suporte**: o texto que você troca com o assistente de IA dentro do app, incluindo a transcrição encaminhada para nós se você pedir explicitamente para falar com um humano.
- **Tráfego anônimo da loja online (Web Pixel, Grow/Unlimited)**: quando um visitante chega a uma página de produto vindo de um motor de IA reconhecido (ChatGPT, Perplexity, Claude, Gemini, Copilot), registramos o motor, a URL da página e um timestamp — apenas se o visitante já tiver dado consentimento de analytics através do banner de cookies da sua loja. Nenhum identificador de visitante, cookie ou dado de sessão é coletado.
- **Dados técnicos**: timestamps de requisições, identificadores internos de registro e logs do sistema.

> O app **nunca solicita ou recebe dados pessoais de clientes finais** — nenhum nome, e-mail, endereço ou pedido. As permissões Shopify solicitadas são `read_products`, `write_products` (catálogo e dados estruturados), `read_themes` (verificar se o embed do tema está ativo) e `write_pixels` (ativar o pixel anônimo de tráfego acima).

## 3. Por que tratamos esses dados, e sob qual base legal

Tratamos esses dados para fornecer o serviço para o qual você instalou o app — sob o Art. 6(1)(b) do RGPD, execução de contrato: analisar e melhorar a visibilidade do seu catálogo em motores de busca generativos, incluindo a redação assistida por IA de FAQs e a reescrita de conteúdo, o chat de suporte dentro do app, o rastreamento semanal de visibilidade em IA sobre os prompts que você escolhe, e a medição anônima de tráfego de referência de IA — todos iniciados pelo lojista ou, no caso do pixel de tráfego, condicionados a consentimento na sua loja online.

## 4. Como coletamos

Os dados da conta são coletados uma única vez, através do fluxo OAuth da Shopify, na instalação. Os dados do catálogo são lidos através da Admin API da Shopify apenas quando você aciona uma ação a partir do dashboard. O pixel de tráfego é executado na sua loja online e reporta eventos somente após o consentimento; nada mais roda em segundo plano sem que você o solicite.

## 5. Com quem compartilhamos

- **Google Firebase / Cloud Firestore** — armazena sua configuração, sessões e rascunhos. A Google LLC (EUA) participa do EU-US Data Privacy Framework. Os dados são armazenados na região europe-west1 (Bélgica).
- **Anthropic PBC (EUA)** — fornece o modelo Claude usado na redação de FAQs, na reescrita de conteúdo e no chat de suporte dentro do app, apenas mediante sua ação explícita. Recebe apenas os atributos do produto ou o texto do chat que você fornece — nunca dados de clientes.
- **OpenAI, Inc. (EUA)** e **Perplexity AI, Inc. (EUA)** — usadas exclusivamente para o rastreamento semanal de visibilidade em IA sobre os prompts que você escolhe explicitamente monitorar. Recebem apenas o texto do prompt rastreado — nunca dados de clientes.
- **Google LLC (EUA)** — fornece o modelo Gemini, usado da mesma forma que OpenAI/Perplexity acima para o rastreamento de visibilidade (um uso distinto do Firebase/Firestore, que é apenas armazenamento).
- **Resend, Inc. (EUA)** — nos envia uma notificação, com o nome da loja e a transcrição do chat de suporte, apenas quando você pede explicitamente para falar com um humano no chat de suporte.
- **Shopify Inc.** — a própria plataforma, e a fonte da Admin API e da infraestrutura de Web Pixel usadas pelo app.

Não vendemos dados, e não os usamos para marketing ou perfilamento comportamental.

## 6. Por quanto tempo os mantemos

- **Tokens de sessão**: gerenciados pelo ciclo de vida dos tokens offline da Shopify, rotacionados automaticamente.
- **Configuração, auditorias, rascunhos e eventos de tráfego**: mantidos enquanto o app estiver instalado. A desinstalação aciona o webhook `shop/redact` da Shopify, que exclui completamente a configuração e as sessões da sua loja.
- **Logs técnicos**: retidos conforme a retenção padrão de logging do Google Cloud.

## 7. Seus direitos

Sob os Artigos 15–22 do RGPD, você pode solicitar acesso aos seus dados, correção de dados incorretos ou exclusão — o jeito mais simples é desinstalar o app — ou se opor ao tratamento. Você também pode registrar uma reclamação junto à sua autoridade local de proteção de dados. Como o app nunca trata dados pessoais de clientes finais, os webhooks de compliance `customers/data_request` e `customers/redact` respondem confirmando que não há nada a exportar ou excluir.

## 8. Segurança

Todo o tráfego roda sobre HTTPS/TLS 1.2+. Os tokens de autenticação da Shopify nunca são expostos ao navegador. Cada webhook é verificado com uma checagem HMAC SHA-256 de tempo constante antes de ser processado. O banco de dados só é acessível a partir do backend, autenticado pela própria identidade de serviço da plataforma de hospedagem — não há credenciais estáticas no código, e o acesso direto do cliente é negado pelas próprias regras de segurança do banco de dados. Os dados são criptografados em repouso e em trânsito.

## 9. Alterações

Podemos atualizar esta política periodicamente. Alterações relevantes serão refletidas aqui, com a data no topo sempre atualizada.

---

**Perguntas sobre seus dados?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Back to Help Center](index.html)
