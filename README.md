# 🍽️ Sabor - Avaliação Gastronômica

> **Uma landing page moderna e interativa para um futuro aplicativo de avaliação de pratos e restaurantes famosos**

<div align="center">

[![HTML5](https://img.shields.io/badge/HTML5-E34C26?style=flat-square&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://www.w3.org/Style/CSS/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://www.javascript.com/)

[Visão Geral](#visão-geral) • [Funcionalidades](#-funcionalidades) • [Como Usar](#como-usar) • [Tecnologias](#-tecnologias) • [Estrutura](#estrutura-do-projeto)

</div>

---

## 👋 Visão Geral

**Sabor** é uma landing page interativa que apresenta um conceito inovador: um aplicativo web para avaliação coletiva de pratos e restaurantes. O projeto é um trabalho acadêmico que combina design moderno, responsividade e interatividade para criar uma experiência de usuário imersiva e engajante.

O site funciona como vitrine digital, permitindo que usuários explorem pratos, curtam seus favoritos, avaliem com sistema de estrelas e acompanhem seus pratos preferidos em uma página dedicada.

---

## ✨ Funcionalidades

### 🎯 Principais Features

- **🖼️ Galeria de Pratos Interativa**
  - Mosaico responsivo com imagens de alta qualidade (AVIF, WebP, JPG)
  - Cards clicáveis com efeito hover envolvente
  - Design moderno e minimalista

- **❤️ Sistema de Curtir**
  - Marque seus pratos favoritos com um clique
  - Dados persistidos em `localStorage` do navegador
  - Feedback visual imediato com mudança de cor
  - Acesso rápido à página de favoritos

- **⭐ Avaliação com Estrelas**
  - Sistema de rating de 1 a 5 estrelas
  - Comentários sobre cada prato
  - Interface intuitiva e responsiva

- **📄 Página de Curtidos**
  - Visualize todos os pratos que você curtiu
  - Sincronização automática com os dados salvos
  - Mensagem amigável quando nenhum prato foi curtido

- **📚 Seção "Como Funciona"**
  - Guia visual em 3 passos simples
  - Instruções claras sobre como usar a plataforma
  - Demonstração visual das funcionalidades

- **🎯 Seções Temáticas**
  - **Conquistas**: Estatísticas e badges do usuário
  - **Queridinhos**: Pratos mais votados da comunidade

- **✉️ Contato Direto**
  - Formulário de contato funcional
  - Link para email integrado

---

## 🚀 Como Usar

### Navegação

1. **Página Inicial** - Explore a galeria de pratos
2. **Curtir Pratos** - Clique no ❤ para adicionar favoritos
3. **Curtidos** - Acesse seus pratos salvos no menu
4. **Avaliações** - Use o sistema de estrelas para avaliar pratos
5. **Fale Conosco** - Entre em contato através do formulário

### Estrutura de Navegação

```
├── 🏠 Home / Galeria
├── 💕 Curtidos (página separada)
├── 🏆 Conquistas
├── ⭐ Queridinhos
└── 📧 Fale Conosco
```

---

## 🛠️ Tecnologias

### Front-end

| Tecnologia | Descrição |
|-----------|-----------|
| **HTML5** | Estrutura semântica e acessível |
| **CSS3** | Estilos modernos com Grid e Flexbox |
| **JavaScript** | Interatividade e persistência de dados |

### Bibliotecas & Ferramentas

- **[Google Fonts](https://fonts.google.com/)** - Tipografia elegante (Montserrat, Leckerli One)
- **[Font Awesome](https://fontawesome.com/)** - Ícones profissionais
- **[localStorage API](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage)** - Persistência de dados local

### Formatos de Imagem

- **AVIF** - Compressão moderna e eficiente
- **WebP** - Alternativa de alta qualidade
- **JPG** - Compatibilidade universal
- **SVG** - Gráficos vetoriais escaláveis

---

## 📂 Estrutura do Projeto

```
Sabor/
├── 📄 index.html              # Página principal
├── 📄 curtidos.html           # Página de favoritos
├── 📄 README.md               # Este arquivo
│
├── 🎨 style.css               # Estilos globais
├── 🎭 script.js               # Lógica principal
│
├── 📁 css/
│   ├── conquistas.css         # Estilos da seção de conquistas
│   ├── curtidos.css           # Estilos da página de favoritos
│   ├── forms.css              # Estilos do formulário
│   ├── funcionamento.css      # Estilos da seção "Como Funciona"
│   ├── mosaico.css            # Estilos da galeria
│   ├── queridinhos.css        # Estilos dos pratos populares
│   └── topo.css               # Estilos do header/navegação
│
├── 📁 img/
│   ├── f1.avif                # Imagem de prato (AVIF)
│   ├── p1.avif                # Imagem de prato (AVIF)
│   ├── r2.avif                # Imagem de prato (AVIF)
│   ├── logo.svg               # Logo do projeto
│   ├── envelope.svg           # Ícone de email
│   └── [outras imagens]       # Pratos diversos
│
└── 📊 Arquitetura
    └── localStorage           # Armazenamento de curtidos
```

---

## 💻 Arquitetura & Lógica

### Sistema de Curtir

```javascript
// Ao clicar em curtir:
1. Recupera o card completo do HTML
2. Busca/Cria array em localStorage
3. Adiciona novo item ao array
4. Salva no localStorage
5. Atualiza visual do botão
```

### Página de Curtidos

```javascript
// Ao carregar curtidos.html:
1. Busca dados em localStorage
2. Se vazio: mostra mensagem amigável
3. Se preenchido: renderiza todos os cards salvos
```

### Avaliação com Estrelas

- Sistema interativo de rating
- Captura clicks nas estrelas
- Permite comentários após avaliação

---

## 🎨 Design & UX

### Cores e Estilo

- **Design Moderno**: Cards com sombras e efeitos hover
- **Tipografia Elegante**: Google Fonts para melhor legibilidade
- **Responsividade**: Adapta-se perfeitamente a qualquer dispositivo
- **Gradientes**: Títulos com efeito gradiente visual
- **Acessibilidade**: Cores contrastantes e navegação clara

### Funcionalidades Visuais

- ✅ Efeitos hover nos cards
- ✅ Feedback de clique com mudança de cor
- ✅ Carousel para seção de chefs/especialistas
- ✅ Layout flexível e adaptável
- ✅ Imagens otimizadas para web

---

## 🎓 Contexto Acadêmico

Este projeto foi desenvolvido como **atividade escolar** com objetivo de demonstrar:

- ✨ Domínio de HTML5 semântico
- 🎨 CSS3 avançado (Grid, Flexbox, Animações)
- ⚙️ JavaScript puro (Vanilla JS) sem frameworks
- 💾 Manipulação de dados com localStorage
- 📱 Desenvolvimento responsivo
- 🎯 Pensamento em UX/UI design
- 🌐 Integração de APIs (Google Fonts, Font Awesome)

---

## 🚀 Como Executar

1. **Clone ou baixe o projeto**
   ```bash
   git clone <seu-repositorio>
   cd Sabor
   ```

2. **Abra no navegador**
   ```bash
   # Simplesmente abra o arquivo index.html
   # ou use um servidor local:
   python -m http.server 8000
   # Depois acesse: http://localhost:8000
   ```

3. **Explore!**
   - Clique nos ❤ para curtir pratos
   - Avalie com as estrelas
   - Visite a página de curtidos
   - Use a navegação para explorar seções

---

## 📱 Compatibilidade

| Navegador | Suporte |
|-----------|---------|
| Chrome | ✅ Total |
| Firefox | ✅ Total |
| Safari | ✅ Total |
| Edge | ✅ Total |
| Mobile (iOS/Android) | ✅ Total |

---

## 📧 Contato

- **Email**: annastudiomultimidia@gmail.com
- **Projeto**: Sabor - Landing Page de Avaliação Gastronômica
- **Status**: ✅ Completo

---

## 📝 Licença

Projeto acadêmico - Uso livre para fins educacionais.

---

<div align="center">

**Desenvolvido com 💕 e muito sabor** 🍽️

*Sabor: Porque toda refeição merece ser avaliada!*

</div>
