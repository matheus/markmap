# 🗺️ MindMap Studio

Uma ferramenta web moderna e minimalista para criação de mapas mentais dinâmicos a partir de Markdown. Transforme suas ideias estruturadas em visualizações interativas em segundos.

![MindMap Studio Preview](https://raw.githubusercontent.com/markmap/markmap/master/packages/markmap-cli/assets/demo.png) *(Ilustrativo: o projeto utiliza a biblioteca Markmap para renderização)*

## ✨ Funcionalidades

- **Markdown para Mapa Mental**: Conversão em tempo real de sintaxe Markdown (`#`, `##`, `###`) em estruturas de árvore visuais.
- **Gerenciamento de Abas**: Crie e alterne entre múltiplos mapas mentais. O progresso é salvo automaticamente no seu navegador (`localStorage`).
- **Personalização via YAML**: Ajuste cores de linhas, destaques, temas (Dark/White) e fontes diretamente no cabeçalho do arquivo.
- **Conteúdo Rico**: Suporte para links e imagens (via sintaxe padrão ou customizada `!IMG[url]`).
- **Navegação Inteligente**:
  - Zoom e Pan fluídos.
  - Expansão e recolhimento de nós.
  - Navegação passo a passo pelos tópicos.
- **Tipografia Customizada**: Painel integrado para importar e aplicar qualquer fonte do Google Fonts.
- **Exportação**:
  - Salve seus mapas como arquivos `.md`.
  - Exporte a visualização final como imagem **PNG** de alta qualidade.
- **Interface Premium**: Design elegante com modo escuro nativo, efeitos de glassmorphism e animações suaves.

## ⌨️ Atalhos de Teclado

| Tecla | Ação |
| :--- | :--- |
| `→` | Expandir próximo nó (Navegação passo a passo) |
| `←` | Recolher nó anterior |
| `E` | Alternar visibilidade do Editor |
| `F` | Ajustar mapa à tela (Fit) |
| `Ctrl + T` | Criar novo mapa |

## 🚀 Tecnologias

O projeto é construído com tecnologias web modernas de alto desempenho:
- **Core**: HTML5, CSS3 (Variáveis Modernas & Glassmorphism), Vanilla JavaScript.
- **Renderização**: [D3.js](https://d3js.org/) & [Markmap](https://markmap.js.org/).
- **Processamento**: [js-yaml](https://github.com/nodeca/js-yaml) para configurações e [html-to-image](https://github.com/bubkoo/html-to-image) para exportação.

## 🛠️ Como usar

1. Abra o arquivo `index.html` em qualquer navegador moderno.
2. Digite seu conteúdo no editor à esquerda usando a hierarquia de títulos do Markdown.
3. Use o painel de **Tipografia** para dar uma identidade visual única ao seu mapa.
4. Clique em **PNG** para exportar sua criação.

---
Desenvolvido com foco em simplicidade e estética visual.