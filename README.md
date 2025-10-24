# ReciclaTech ♻️

ReciclaTech é um projeto simples em HTML + SCSS pensado para demonstrar uma interface de doação/adopção de eletrônicos. O objetivo do README é documentar como o projeto está organizado, como compilar o SCSS para CSS e como fazer um preview local rápido.

## Protótipo 🔗

- [Link do Protótipo](https://www.figma.com/design/hkJmg0Rph4wDe9BJD0ETeP/Recicla-Tech-1.0?node-id=0-1&p=f&t=ttx0ndIZomL0Qlu8-0)

## Tecnologias 🛠️

- HTML5 📄
- SCSS (pré-processador) 🎛️
- CSS 🎨

## Estrutura do repositório (resumo) 🗂️

Raiz:

- `index.html` — página principal (entrada)
- `public/` — arquivos públicos (ex.: `logo.svg`)
- `src/`
  - `assets/` — imagens e ícones usados pela página
    - `imgs/` — imagens de produto e ilustrações
    - `icons/` — ícones bitmap usados no projeto
  - `css/` — CSS compilado e arquivos SCSS
    - `reset.scss` — reset / normalize + variáveis (fonte, cores)
    - `reset.css` — CSS compilado (gerado a partir do SCSS)
    - `navbar/`, `hero/`, `statistics/`, etc. — estilos por seção (SCSS/CSS)
- `README.md` — este arquivo

## Como pré-visualizar ▶️

Opção 1 — Abrir diretamente no navegador:

1. Abra o arquivo `index.html` no navegador (duplo clique ou "Abrir com" → navegador).

Opção 2 — Usar um servidor estático (recomendado para testes):

- Se você tiver a extensão Live Server (VS Code), clique em "Go Live". 🚀
- Ou use o `http-server` via npm (se já tiver Node.js instalado):

```cmd
npx http-server -c-1 .
```

Em ambos os casos, verifique se os caminhos das folhas de estilo (`src/css/*.css`) e das imagens estão corretos. ✅

## Acessibilidade e boas práticas ♿️

- Botões importantes têm `aria-label` no `index.html` (ex.: botões do hero).
- O reset SCSS define um estilo de foco visível por padrão (outline) para navegação por teclado.

## Contribuindo 🤝

Pequenas contribuições são bem-vindas. Sugestões:

- Corrigir ou otimizar imagens (tamanhos, compressão).
- Modularizar SCSS (criar `_variables.scss`, `_components.scss`, etc.).

### Workflow sugerido (local):

1. Crie uma branch: `git checkout -b feat/nova-coisa`
2. Faça alterações e teste localmente (compile SCSS, abra `index.html`).
3. Commit e PR.

## Observações finais / Licença 📄

Desenvolvido para fins educacionais. Se você compartilhar ou usar partes deste projeto, mantenha a referência ao autor quando possível.