# Comparativo Bootstrap x Tailwind CSS

## Objetivo

Atividade de front-end em que o mesmo layout (protótipo "Empresa", aqui adaptado para o site fictício "Raízes do Sul") foi desenvolvido duas vezes, uma com **Bootstrap 5** e outra com **Tailwind CSS**, para comparar a experiência de desenvolvimento das duas tecnologias. As duas versões têm os mesmos elementos e a mesma organização visual: hero com título, bloco de conteúdo com imagem e textos, e uma seção cinza com três cards e botões arredondados laranja.

## Estrutura do repositório

| Branch | Conteúdo |
|---|---|
| `bootstrap` | Desenvolvimento da versão com Bootstrap |
| `tailwind` | Desenvolvimento da versão com Tailwind CSS |
| `main` | As duas versões finalizadas (`bootstrap/` e `tailwind/`) e este README |

```
.
├── README.md
├── bootstrap/
│   ├── index.html
│   └── style.css
└── tailwind/
    └── index.html
```

## Como cada versão foi construída

### Bootstrap
- Bootstrap 5.3 carregado por CDN.
- Layout feito com o sistema de grid (`container`, `row`, `col-md-4`) e utilitários (`py-5`, `fw-bolder`, `rounded-pill`).
- O `style.css` guarda só o que o Bootstrap não oferece pronto: a imagem de fundo do hero e a cor laranja do botão (`.btn-laranja`).

### Tailwind CSS
- Tailwind carregado por CDN (script Play CDN, sem etapa de build).
- Todo o estilo está nas classes utilitárias do HTML (`grid md:grid-cols-3`, `rounded-full`, `bg-laranja`).
- A cor laranja foi registrada em `tailwind.config` e usada como `bg-laranja`.
- Não existe arquivo CSS: a imagem de fundo do hero fica em um `style` inline, por ser uma imagem específica.

## Como executar

Não é necessário instalar nada. Precisa de internet, pois Bootstrap, Tailwind e as imagens vêm de CDN.

1. Clone o repositório: `git clone <link-do-repositorio>`
2. Abra `bootstrap/index.html` ou `tailwind/index.html` no navegador (duplo clique ou "Open with Live Server" no VS Code).
