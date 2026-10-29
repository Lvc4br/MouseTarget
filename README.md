# MouseTarget — Experimento de interação com mouse

Pequeno experimento de front-end para praticar eventos do mouse e efeitos visuais controlados por JavaScript e CSS. O projeto não usa framework, bundler ou backend.

## Objetivo e comportamento

A página demonstra cartões com efeitos visuais associados à posição do cursor. O JavaScript obtém a posição relativa ao elemento e atualiza propriedades CSS, usadas para posicionar o destaque radial e aplicar transições de hover.

## Arquitetura e arquivos

```text
MouseTarget/
└── teste-mouse-houver/
    ├── index.html             # página principal do experimento
    ├── js.js                  # eventos e lógica de interação
    ├── style.css              # layout, cartões e efeitos CSS
    └── teste particle/
        ├── index.html         # experimento separado com partículas
        ├── style.css
        └── img/               # imagens usadas no experimento
```

Fluxo: navegador carrega o HTML → CSS define estrutura visual e estados → JavaScript registra eventos, mede o elemento com `getBoundingClientRect()` e atualiza variáveis/estilos → CSS renderiza o efeito.

## Tecnologias

- HTML5
- CSS3, gradientes radiais, transições e estados de hover
- JavaScript nativo e eventos do DOM

## Executar

Abra `teste-mouse-houver/index.html` no navegador. Como não há processo de build nem dependências npm, não é necessário instalar pacotes. Se recursos locais não carregarem devido a restrições do navegador, sirva a pasta por um servidor HTTP simples.

## Escopo e limitações

- É um estudo demonstrativo, não uma biblioteca de componentes.
- Não há backend, persistência de dados, API ou testes automatizados configurados.
- A pasta `teste particle/` contém um experimento separado; não deve ser confundida com a implementação principal.
- A estrutura documenta os arquivos presentes no repositório; não implica que exista suporte formal a todos os dispositivos de entrada.

## Projetos relacionados

- [LV_Portfolio](https://github.com/Lvc4br/LV_Portfolio) — portfólio principal.
- [webpage](https://github.com/Lvc4br/webpage) — protótipos web anteriores.

**Autor:** Luca Toniolo — [@Lvc4br](https://github.com/Lvc4br)
