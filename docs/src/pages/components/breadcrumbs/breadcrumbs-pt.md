---
title: Componente React para Navegação estrutural
components: Breadcrumbs, Link, Typography
githubLabel: 'component: Breadcrumbs'
waiAria: 'https://www.w3.org/TR/wai-aria-practices/#breadcrumb'
---

# Navegação estrutural

<p class="description">Breadcrumbs consist of a list of links that help a user visualize a page's location within the hierarchical structure of a website, and allow navigation up to any of its "ancestors".</p>

{{"component": "modules/components/ComponentLinkHeader.js"}}

## Navegação estrutural simples

{{"demo": "pages/components/breadcrumbs/BasicBreadcrumbs.js"}}

## Último caminho ativo

Mantendo o último caminho de navegação interativo.

{{"demo": "pages/components/breadcrumbs/ActiveLastBreadcrumb.js"}}

## Separador customizado

Nos exemplos a seguir, nós estamos usando dois separadores de string e um ícone SVG.

{{"demo": "pages/components/breadcrumbs/CustomSeparator.js"}}

## Navegação estrutural com ícones

{{"demo": "pages/components/breadcrumbs/IconBreadcrumbs.js"}}

## Navegação estrutural retraída

{{"demo": "pages/components/breadcrumbs/CollapsedBreadcrumbs.js"}}

## Navegação estrutural customizada

Aqui está um exemplo de customização do componente. Você pode aprender mais sobre isso na [página de documentação de sobrescritas](/customization/how-to-customize/).

{{"demo": "pages/components/breadcrumbs/CustomizedBreadcrumbs.js"}}

## Integração com react-router

{{"demo": "pages/components/breadcrumbs/RouterBreadcrumbs.js", "bg": true}}

## Acessibilidade

(WAI-ARIA: https://www.w3.org/TR/wai-aria-practices/#breadcrumb)

Certifique-se de adcionar uma descrição `aria-label` no componente `Breadcrumbs`.

A acessibilidade neste componente conta com:

- O conjunto de links são estruturados usando uma lista ordenada (elemento `<ol>`).
- Para prevenir que os leitores de tela pronunciem os separadores visuais entre os links, eles são escondidos com `aria-hidden`.
- Um elemento `nav` rotulado com `aria-label` identifica a estrutura como uma trilha de navegação estrutural e faz uma marcação na navegação para facilitar a localização.
