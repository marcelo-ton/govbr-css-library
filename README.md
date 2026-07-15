# govbr-css-library

Biblioteca de organização das páginas web (HTML, CSS e JSON) mantidas em portais da plataforma gov.br.

## Motivação

O CMS da plataforma gov.br está na versão 4 e migrará para a versão 6 (desenvolvimento a cargo da equipe de Governo Digital). A versão 6 não interpreta corretamente blocos `<style></style>` inline, o que pode fazer com que páginas percam suas definições de estilo durante a migração.

Este repositório organiza o conteúdo disperso em arquivos `.css` externos por página, para que os estilos sobrevivam à migração independentemente de como a nova versão do CMS trata estilos inline.

## Estrutura

```
pages/
  <nome-da-pagina>/
    content.json   # conteúdo/config da página, quando aplicável
    index.html     # marcação HTML da página
    style.css      # estilos extraídos do <style> inline original
```

## Status

Fase inicial de organização. Conteúdo sendo migrado das páginas do gov.br para este repositório.
