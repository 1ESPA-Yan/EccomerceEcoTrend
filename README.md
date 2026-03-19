# 🌿 EcoTrend

E-commerce especializado em produtos sustentáveis e ecológicos, desenvolvido como projeto de checkpoint da disciplina de Front-end Design. O site apresenta uma loja completa com páginas de home, categorias, detalhes de produto e contato, com foco em HTML semântico, CSS responsivo e uso do framework Bootstrap.

## 🔗 Acesse o Site

[https://1espa-yan.github.io/EccomerceEcoTrend/](https://1espa-yan.github.io/EccomerceEcoTrend/)

---

## 📋 Sobre o Projeto

O EcoTrend é um e-commerce fictício focado em produtos sustentáveis e ecológicos, promovendo um estilo de vida mais consciente. O projeto foi desenvolvido para demonstrar conhecimentos em HTML5 semântico, CSS3 responsivo, sistema de grid do Bootstrap e boas práticas de organização de código.

### Tipos de produtos comercializados
- Roupas e acessórios sustentáveis
- Produtos de beleza e cuidados pessoais naturais
- Itens para casa sustentáveis
- Tecnologia verde

---

## 🛠️ Tecnologias Utilizadas

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=flat&logo=bootstrap&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-181717?style=flat&logo=github&logoColor=white)

**HTML5**
- Estrutura semântica com tags apropriadas (`header`, `nav`, `main`, `section`, `footer`)
- Atributos de acessibilidade (`aria-label`, `aria-current`, `alt`)
- Organização por páginas com navegação entre elas

**CSS3**
- Variáveis CSS (`custom properties`) para paleta de cores consistente
- Flexbox para alinhamento de componentes
- Media queries para responsividade em três breakpoints (mobile, tablet, desktop)
- Transições suaves em hover de cards e botões
- Arquivos CSS separados por responsabilidade (`global.css` + CSS específico por página)

**Bootstrap 5**
- Sistema de grid responsivo com `container`, `row` e `col`
- Componente de carrossel (`carousel`) para o banner da home
- Cards (`card`) para exibição de produtos
- Navbar responsiva com offcanvas para mobile
- Formulário estilizado com `form-control` e `form-label`
- Breadcrumb para navegação na página de produto
- Classes utilitárias (`d-flex`, `g-3`, `mx-auto`, `h-100`, `w-100` etc.)

**Bibliotecas externas**
- [Bootstrap 5.3](https://getbootstrap.com/) — Framework CSS/JS
- [Font Awesome 6.4](https://fontawesome.com/) — Biblioteca de ícones
- [Google Fonts](https://fonts.google.com/) — Fontes EB Garamond e Inter

---

## 📁 Estrutura de Arquivos

```
EcommerceEcoTrend/
│
├── home.html                  # Página inicial
├── categorias.html            # Página de categorias com filtros
├── produto.html               # Página de detalhes do produto
├── contato.html               # Página de contato com formulário
├── README.md                  # Documentação do projeto
│
└── src/
    ├── css/
    │   ├── global.css         # Estilos globais (navbar, footer, cards, botões)
    │   ├── home.css           # Estilos específicos da home
    │   ├── categorias.css     # Estilos específicos das categorias
    │   ├── produto.css        # Estilos específicos do produto
    │   └── contato.css        # Estilos específicos do contato
    │
    └── images/                # Imagens dos produtos e banners
        ├── RoupaSustentavel.png
        ├── CosmeticosSustentaveis.png
        ├── CasaSustentavel.png
        ├── CamisetaOrganica.png
        └── ...
```

---

## 📄 Páginas

### Página Inicial — `home.html`
A página inicial apresenta a loja com um banner em carrossel destacando promoções e produtos em destaque, seguido de um grid de produtos organizado por categorias. O carrossel usa o componente nativo do Bootstrap com três slides, cada um com título, descrição e botão de ação. Os produtos são exibidos em cards responsivos que se adaptam de 2 colunas no mobile para 4 no desktop.

### Categorias — `categorias.html`
Exibe todos os produtos da loja em um layout de grid com filtros laterais. Os filtros permitem selecionar por categoria, faixa de preço e marca, usando checkboxes e radio buttons estilizados com as cores da marca. O grid de produtos ocupa 9 das 12 colunas do Bootstrap, enquanto os filtros ocupam as 3 restantes.

### Detalhes do Produto — `produto.html`
Apresenta as informações completas de um produto, divididas em duas colunas: imagem à esquerda e informações à direita. Inclui breadcrumb de navegação, badge de categoria, nome, preço, descrição, seletor de tamanho por botões de rádio, seletor de quantidade e botão de adicionar ao carrinho. Uma lista de benefícios com ícones do Font Awesome complementa a página.

### Contato — `contato.html`
Formulário de contato estilizado com Bootstrap contendo campos de nome, email, assunto e mensagem. O formulário é centralizado na página com largura limitada para melhor legibilidade, e o botão de envio segue o estilo principal da marca.

---

## 🎨 Identidade Visual

### Paleta de Cores

| Nome | Hexadecimal | Uso |
|------|-------------|-----|
| Off-White | `#FDFBFA` | Fundo principal da página |
| Carvão | `#1F1F1F` | Fundo do footer |
| Verde Sálvia | `#7C8D7B` | Cor de destaque, CTAs, ícones |
| Bege | `#F8F4EF` | Fundo da navbar, filtros, badges |
| Texto Principal | `#333333` | Títulos e corpo de texto |
| Texto Secundário | `#A6A6A6` | Meta textos e informações secundárias |
| Divisor | `#E8E8E8` | Linhas divisórias entre seções |

### Tipografia

| Fonte | Tipo | Uso |
|-------|------|-----|
| EB Garamond | Serif | Títulos (`h1` a `h5`), nome da marca |
| Inter | Sans-serif | Corpo de texto, botões, preços |

---

## 📱 Responsividade

O layout é totalmente responsivo com três breakpoints principais, seguindo a abordagem ensinada nas aulas:

**Mobile (padrão — até 767px)**
- Navbar com menu offcanvas lateral
- Carrossel com altura de `30vh`
- Cards de produtos em 2 colunas (`col-6`)
- Filtros acima dos produtos (coluna única)

**Tablet (768px+)**
- Carrossel com altura de `40vh`
- Cards de produtos em 2 colunas

**Desktop (992px+)**
- Navbar horizontal completa
- Carrossel com altura de `50vh`
- Cards de produtos em 4 colunas (`col-lg-3`)
- Filtros laterais ao lado do grid de produtos (`col-lg-3` + `col-lg-9`)

---

## 🧩 Componentes Bootstrap Utilizados

| Componente | Página | Finalidade |
|------------|--------|------------|
| Navbar + Offcanvas | Todas | Menu de navegação responsivo |
| Carousel | Home | Banner de promoções |
| Card | Home e Categorias | Exibição de produtos |
| Grid (row + col) | Todas | Layout responsivo |
| Breadcrumb | Produto | Indicação de localização |
| Form + Form Control | Contato | Formulário de contato |
| Input Group | Produto | Seletor de quantidade |
| Btn-check | Produto | Seletor de tamanho |
| Badge | Produto | Categoria do produto |

---

## 🚀 Como Executar o Projeto

### Opção 1: Acesso Online
Acesse o site hospedado no GitHub Pages:
[https://1espa-yan.github.io/EccomerceEcoTrend/](https://1espa-yan.github.io/EccomerceEcoTrend/)

### Opção 2: Execução Local

**Passo 1: Clone o repositório**
```bash
git clone https://github.com/1ESPA-Yan/EccomerceEcoTrend.git
```

**Passo 2: Navegue até a pasta do projeto**
```bash
cd EcommerceEcoTrend
```

**Passo 3: Abra o projeto**

**A) Duplo clique no arquivo `home.html`**
O navegador padrão abrirá automaticamente o site.

**B) Use o Live Server (recomendado)**
1. Instale a extensão "Live Server" no VS Code
2. Abra a pasta do projeto no VS Code
3. Clique com botão direito em `home.html`
4. Selecione "Open with Live Server"

---

## 👥 Integrantes do Grupo

| Nome | RM |
|------|----|
| Yan Lucas Gonçalves da Silva | RM: 567046 |
| João Victor Melo Santos | RM: 566640 |
| Gustavo Macedo Daniel | RM: 567594 |

---

## 📝 Licença

Este projeto foi desenvolvido para fins educacionais como parte do **Check-point 04** da disciplina de Front-end Design — FIAP.

---