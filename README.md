# 👟 SyntaxWear - E-commerce de Sneakers & Tênis

> Uma landing page moderna, elegante e responsiva para uma loja virtual de calçados esportivos e casuais, desenvolvida com HTML5 e CSS3 puro.

---

## 📌 Sobre o Projeto

O **SyntaxWear** é uma landing page de comércio eletrônico focada no segmento de *sneakers* e calçados modernos. O projeto foi estruturado seguindo as melhores práticas de desenvolvimento web front-end, priorizando:

- **Semântica HTML5** para acessibilidade e otimização em motores de busca (SEO).
- **CSS Modular e Componentizado**, separando as regras de cada bloco da interface para facilitar a manutenção e leitura.
- **Design Totalmente Responsivo**, proporcionando uma experiência fluida tanto em computadores (Desktop) quanto em tablets e smartphones (Mobile).
- **Menu Mobile sem JavaScript**, utilizando a técnica do *Checkbox Hack* em puro CSS.

---

## 🚀 Tecnologias Utilizadas

| Tecnologia | Finalidade no Projeto |
| :--- | :--- |
| **HTML5** | Estruturação semântica da página (`header`, `main`, `section`, `nav`, `footer`). |
| **CSS3** | Estilização, layout visual, animações e responsividade. |
| **CSS Grid & Flexbox** | Construção do mosaico de produtos e alinhamento dos componentes. |
| **Google Fonts** | Tipografia moderna utilizando a família de fontes **Ubuntu**. |
| **Vetores SVG** | Ícones e logotipo em formato vetorial com alta definição e leveza. |

---

## 🎨 Funcionalidades e Seções do Site

1. **Header Flutuante e Fixo:**
   - Barra de navegação com bordas arredondadas e efeito flutuante sobre a página.
   - Logotipo oficial em vetor SVG.
   - Menu principal (Masculino, Feminino, Outlet) e atalhos rápidos (Minha Conta, Ajuda e Carrinho de Compras).
   - Menu Hambúrguer interativo para dispositivos móveis acionado via CSS (`:checked`).

2. **Hero Section (Destaque Principal):**
   - Banner imersivo de apresentação do modelo *Krypton One*.
   - Chamada para ação (*Call to Action* - CTA) com botões estilizados "Ver modelos" e "Comprar".
   - Adaptação inteligente da imagem de fundo para telas menores (`hero-mobile.jpg`).

3. **Categorias de Calçados:**
   - Vitrine rápida dividida em quatro estilos: **Casual**, **Esporte**, **Moderno** e **Futurista**.
   - Cards com máscara escura (*overlay*) para garantir legibilidade dos textos e botões sobre as fotos.

4. **Product Grid (Mosaico de Produtos):**
   - Grade construída com **CSS Grid** e `grid-template-areas`.
   - Layout dinâmico tipo mosaico destacando o tênis principal e modelos complementares.
   - Reorganização automática para 2 colunas em telas de tablets e celulares.

5. **Rodapé Completo (Footer):**
   - Campo para cadastro de Newsletter (captura de e-mail de clientes).
   - Links para redes sociais oficiais (Instagram, WhatsApp, TikTok, Facebook).
   - Mapa de links do site com navegação estruturada.
   - Aviso de direitos autorais (*Copyright*).

---

## 📂 Estrutura de Pastas e Arquivos

O projeto está organizado com uma arquitetura modular de CSS:

```
ecommerce-syntaxwear/
│
├── index.html                   # Página principal da aplicação
├── README.md                    # Documentação do projeto
│
├── css/
│   ├── base.css                 # Estilos globais (body, main, botões reutilizáveis)
│   ├── reset.css                # Limpeza de margens e padrões dos navegadores
│   ├── variables.css            # Variáveis CSS (:root) e importação de fontes externas
│   │
│   └── components/              # Estilos específicos de cada seção/componente
│       ├── header.css           # Estilos do cabeçalho e menu responsivo
│       ├── hero.css             # Banner de destaque inicial
│       ├── product-category.css # Cards de categorias de produtos
│       ├── product-grid.css     # Mosaico de produtos construído em CSS Grid
│       └── footer.css           # Rodapé, formulário de newsletter e redes sociais
│
└── images/
    ├── banners/                 # Banners para desktop e mobile
    ├── favicons/                # Pasta reservada para ícones de navegador
    ├── icons/                   # Ícones da interface em SVG (carrinho, usuário, etc.)
    ├── logo/                    # Logotipo da marca SyntaxWear em SVG
    └── products/                # Fotos dos calçados e modelos da loja
```

---

## 💡 Destaques de Aprendizado e Boas Práticas

- **Checkbox Hack para Menu Mobile:**
  O menu hambúrguer foi criado usando um `<input type="checkbox">` oculto e um `<label>`. Quando o usuário clica no ícone, o estado `:checked` altera a posição do menu (`right: 0`), abrindo a gaveta lateral suavemente com CSS `transition`, sem precisar de uma única linha de JavaScript!

- **Organização Modular do CSS:**
  Em vez de colocar todo o código em um único arquivo gigante, o CSS foi dividido por responsabilidade (`components/`), tornando o código mais limpo, fácil de entender e de manter.

- **Uso do CSS Grid com Áreas Nomeadas (`grid-template-areas`):**
  Facilita visualizar a montagem da grade no próprio código, além de permitir reorganizar completamente as peças na versão mobile apenas alterando o mapa de áreas nas `@media` queries.

- **Unidades Relativas (`rem`, `%`):**
  Uso de `rem` para tamanhos de fonte e espaçamentos, permitindo melhor acessibilidade e consistência visual.

---

## 🖥️ Como Executar o Projeto

Como este projeto utiliza apenas tecnologias nativas da web (HTML e CSS), você não precisa instalar nenhuma ferramenta pesada ou gerenciador de pacotes (como Node.js ou npm).

### Opção 1: Abrir diretamente no Navegador
1. Baixe ou clone este repositório no seu computador.
2. Localize o arquivo `index.html` na pasta do projeto.
3. Dê um duplo clique no arquivo `index.html` ou clique com o botão direito e selecione **"Abrir com"** -> seu navegador favorito (Google Chrome, Edge, Firefox, Brave, etc.).

### Opção 2: Usando o Live Server no VS Code (Recomendado)
1. Abra a pasta do projeto no **Visual Studio Code**.
2. Caso ainda não tenha, instale a extensão **Live Server** (de Ritwick Dey).
3. Clique com o botão direito sobre o arquivo `index.html` e escolha **"Open with Live Server"**.
4. O projeto abrirá automaticamente no endereço `http://127.0.0.1:5500`, atualizando a tela a cada alteração que você salvar nos arquivos!

---

## 📱 Responsividade (Breakpoints)

O design foi ajustado para se adaptar perfeitamente a diferentes tamanhos de tela:
- **Telas Grandes (> 1280px):** Layout completo e espaçoso.
- **Telas Médias (até 1280px):** Cabeçalho adaptativo e menu hambúrguer ativado.
- **Tablets (até 1000px):** Ajuste do rodapé para disposição vertical e centralizada.
- **Smartphones (até 768px):** Banner com imagem mobile exclusiva, cards de categorias em largura total (100%) e grid de produtos reorganizado.

---

## 📄 Licença

Este projeto foi desenvolvido para fins educacionais e de estudo. Sinta-se à vontade para utilizá-lo como referência ou base para seus próprios projetos de portfólio!

---