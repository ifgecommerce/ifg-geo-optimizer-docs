---
title: IFG GEO Optimizer
description: Documentação, FAQ e páginas legais do app Shopify IFG GEO Optimizer.
lang: pt
---

# Getting Started

<div class="lang-switcher">
{% include lang-switcher.html current="pt" slug="getting-started" %}
</div>

O IFG GEO Optimizer tem nove áreas, todas acessíveis a partir da navegação superior assim que a configuração inicial estiver concluída: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** e **Support**. Este guia percorre todas elas, na ordem em que a maioria dos lojistas costuma usá-las.

## 1. Instale e conclua o assistente de configuração

Na primeira abertura, um pequeno assistente guiado (cerca de 2 minutos) coleta o essencial: idioma da interface, os detalhes da sua política de devolução e envio, os dados da sua empresa e — a única etapa que realmente importa tecnicamente — a ativação do app embed **GEO Schema** no editor de tema. Nada do que o app faz depois chega à sua loja online até que esse embed seja ativado, então vale a pena não pular essa etapa. Você pode sempre alterar qualquer uma dessas respostas depois em **Settings**.

## 2. Dashboard

Sua base inicial. Mostra sua pontuação GEO atual (da última auditoria), uma **Readiness Matrix** com oito sinais à primeira vista — extratibilidade de conteúdo, schema Organization, `llms.txt`, `agents.md`, acesso de crawlers, prontidão MCP, conectividade do Link Coach e tráfego de referência de IA — além de uma lista priorizada de "corrija isto primeiro" e os contadores de uso do seu plano (gerações de FAQ, tamanho do catálogo). Tudo aqui leva diretamente à página onde você pode agir.

## 3. Audit catalog

Clique em **Rescan catalog** para verificar cada produto em relação a nove campos de dados estruturados que os motores de busca procuram: imagem, descrição, marca, SKU, GTIN, preço, especificações técnicas, política de devolução e política de envio. Produtos abaixo de 80/100 mostram exatamente o que está faltando.

- **Correção em um clique**: quando o app consegue derivar com segurança o dado ausente (geralmente especificações técnicas a partir das opções já existentes do produto), você verá um botão **Fix** que grava o dado diretamente nos dados estruturados do produto. Nada é adivinhado para campos que o app não consegue verificar — um código de barras ausente, por exemplo, permanece ausente em vez de ser inventado.
- **Content chunking score**: junto com a verificação de dados estruturados, cada produto recebe uma pontuação de extratibilidade separada — não "o campo está presente", mas "um sistema de IA/RAG consegue realmente extrair um fato limpo dessa descrição". Textos rasos e carregados de adjetivos pontuam mais baixo mesmo com markup schema.org perfeito.
- **`llms.txt`**: gera um arquivo `llms.txt` real, compatível com o padrão, resumindo seu catálogo para sistemas de IA, servido na raiz verdadeira da sua loja (`/llms.txt`), e não escondido sob um caminho de app proxy onde os crawlers não conseguem encontrá-lo.
- **`agents.md`**: gera um arquivo que descreve sua loja para agentes de compra autônomos — variantes, busca, checkout — construído apenas com dados reais que sua loja já expõe, nada inventado.
- **Schema Organization**: publica os dados da sua empresa (razão social, CNPJ/NIF, endereço) como dados estruturados, para que os motores de IA possam verificar que você é um negócio real e responsável antes de recomendá-lo.

No plano Free, as auditorias cobrem os primeiros 20 produtos, uma única vez, sem histórico. Grow e Unlimited analisam todo o catálogo e mantêm cada auditoria anterior para comparação de tendências.

## 4. Crawler AI

Escolha um produto e o app busca a página exatamente como um crawler de IA faria — sem execução de JavaScript, igual ao GPTBot, ClaudeBot ou PerplexityBot — para que você veja precisamente o que é visível para esses motores: se o seu `robots.txt` os bloqueia (verificado por bot, não apenas um permitir/negar genérico), e se seus dados estruturados realmente sobrevivem no HTML bruto que esses bots leem.

**Comparação com concorrentes** (aba própria nesta página): cole a URL de produto de um concorrente e obtenha os mesmos sinais de GEO comparados lado a lado com os seus — a mesma diferença qualitativa que você teria numa auditoria manual, sem precisar se cadastrar nas ferramentas do próprio concorrente.

## 5. FAQ product

No Grow ou Unlimited, escolha um produto e clique em **Generate FAQs** para obter de três a cinco pares de pergunta e resposta gerados apenas a partir do título, descrição, fornecedor e especificações reais desse produto — o modelo é explicitamente instruído a nunca acrescentar um detalhe que não esteja já nos seus dados. Revise cada rascunho; nada é publicado sem o seu **Approve** explícito. As FAQs aprovadas aparecem na página do produto ao vivo e são marcadas como dados estruturados `FAQPage`, ficando ao mesmo tempo legíveis por humanos e citáveis por máquinas.

**Reescrita de conteúdo** (aba própria nesta página): o app pode reescrever a descrição de um produto para torná-la mais densa em fatos verificáveis e mais fácil de citar por um motor generativo — você sempre vê uma comparação antes/depois e aprova antes que qualquer coisa seja gravada de volta no produto.

## 6. Link Coach

Analisa o quão bem seus produtos estão conectados entre si por meio de coleções, fornecedores e tags compartilhadas — o linking interno é um sinal que os sistemas de IA usam para entender o que o seu catálogo cobre como um todo, não apenas uma página de cada vez. Mostra produtos órfãos, sem conexões significativas, e sugestões explicáveis para corrigir isso.

## 7. Visibility AI

Adicione até um punhado de prompts que você razoavelmente esperaria que um cliente fizesse a um assistente de IA (o limite depende do seu plano — veja Pricing abaixo), e toda semana o app verifica se Claude, ChatGPT, Gemini e Perplexity mencionam sua loja na resposta, com o histórico rastreado por motor ao longo do tempo. No Grow e no Unlimited, isso também mostra como você se compara a concorrentes nomeados nos mesmos prompts.

**Tráfego de referência de IA** (Grow e Unlimited): um pixel leve e que respeita a privacidade detecta quando uma visita à loja online realmente se origina de um desses motores de IA (via referrer, apenas depois que o visitante deu consentimento de analytics através do banner de cookies da sua loja) e informa quantas visitas desse tipo você teve nos últimos 7 dias — a segunda metade do ciclo que o rastreamento de visibilidade sozinho não consegue mostrar: não apenas "somos mencionados", mas "essa menção está enviando alguém".

## 8. Support

Um assistente de chat com IA vive dentro do app (ícone no canto inferior direito) para perguntas sobre GEO, os resultados da sua auditoria, ou como uma funcionalidade específica funciona. Se ele não conseguir ajudar, você pode pedir para falar com um humano e a conversa é encaminhada diretamente para a IFG eCommerce.

## 9. Settings

Onde você gerencia as respostas do assistente de configuração (políticas, dados da empresa, idioma da interface — troque instantaneamente entre 30 idiomas, sem atraso de recarregamento), reverifica a ativação do embed do tema, e vê os escopos Shopify da sua conta.

## 10. Pricing

**Pricing** mostra Free, Grow e Unlimited lado a lado, mensal ou anual (o anual equivale a cerca de 2 meses grátis em ambos os planos pagos). Você pode fazer upgrade, downgrade ou voltar ao Free a qualquer momento, diretamente pelo app — sem precisar de e-mail. Veja o [FAQ](faq.html) para os limites exatos de cada plano.

Esse é o ciclo completo. A maioria dos lojistas reexecuta uma auditoria após adicionar novos produtos, verifica o simulador de crawler sempre que atualiza uma descrição, e dá uma olhada semanal na Readiness Matrix do Dashboard.

[← Back to Help Center](index.html)
