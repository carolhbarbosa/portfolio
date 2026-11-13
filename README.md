# 💼 Portfólio Profissional - Carolina Barbosa

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![Status](https://img.shields.io/badge/STATUS-CONCLUÍDO-brightgreen?style=for-the-badge)

## 👩‍💻 Aluna

Carolina Barbosa

Atividade da **Agenda 15** de Desenvolvimento de Sistemas I, do curso Técnico em Desenvolvimento de Sistemas.

## 📌 Descrição do portfólio

Página de portfólio pessoal para apresentar meu perfil, as tecnologias que estou estudando e os projetos que desenvolvi ao longo do curso.

O site tem:

- menu de navegação (navbar) fixo no topo;
- carousel de destaque na abertura;
- seção **Perfil**, com foto, apresentação, informações e tecnologias;
- seção **Projetos**, com cards dos meus trabalhos e links para cada repositório;
- seção **Contato**, com e-mail, GitHub e LinkedIn;
- rodapé.

## 🛠️ Tecnologias utilizadas

- HTML5
- CSS3
- Bootstrap 5.3
- GitHub e GitHub Pages
- VS Code

## 🔗 Site publicado

👉 [**LINK-DO-GITHUB-PAGES**](https://carolhbarbosa.github.io/portfolio/)

## ⚙️ Como o projeto funciona

O projeto é um único arquivo `index.html`, com as imagens na pasta `imagens/`.

- O **Bootstrap** é carregado por CDN (um link na internet) e fornece o layout responsivo, a navbar, o carousel, os cards e os botões.
- Os links do menu (`#perfil`, `#projetos`, `#contato`) levam até as seções da página, que têm o `id` correspondente.
- O site se adapta a celular, tablet e computador, por causa da `meta viewport` e do sistema de colunas do Bootstrap (`row` e `col`).
- Os cards de projetos têm um botão "Ver projeto" que abre o repositório no GitHub em uma nova aba.

### Estrutura de arquivos

```
portfolio/
├── index.html
├── README.md
└── imagens/
    ├── perfil.png
    ├── slide1.png, slide2.png, slide3.png
    └── p1.png, p2.png, p3.png
```

## ✨ Recurso novo adicionado

**Efeito de hover nos cards de projetos.**

Ao passar o mouse sobre um card da seção Projetos, ele sobe suavemente e ganha uma sombra maior, o que deixa o site mais interativo e destaca o projeto que o visitante está olhando.

### Como o recurso foi implementado

Criei uma classe CSS própria, chamada `.card-projeto`, no `<style>` dentro do `<head>`, e adicionei essa classe aos três cards de projetos:

```css
.card-projeto {
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card-projeto:hover {
    transform: translateY(-8px);
    box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.25) !important;
}
```

- `transition` faz a mudança acontecer de forma suave, em 0,3 segundo.
- `:hover` aplica o estilo apenas quando o mouse está sobre o card.
- `transform: translateY(-8px)` levanta o card em 8 pixels.
- `box-shadow` aumenta a sombra para dar sensação de profundidade.
- O `!important` foi necessário porque a classe `shadow-sm` do Bootstrap também usa `!important`.

## 👤 Autora

Feito por **Carolina Barbosa** · [GitHub](https://github.com/carolhbarbosa)
