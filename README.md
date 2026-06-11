# ✦ Markmap

Crie mapas mentais elegantes a partir de texto Markdown. Minimalista, leve e bonito — tudo em um único arquivo `index.html`.

## ✨ Funcionalidades

- **Markdown → Mapa Mental** em tempo real — escreva e veja o mapa se formar enquanto digita
- **Sintaxe de listas** — use `-` com indentação para criar hierarquias, muito mais intuitivo que `##` e `###`
- **Modo Foco** — oculta toda a interface para apresentações e gravações de tela sem distração
- **Navegação passo a passo** — o mapa começa fechado e você revela nó por nó com as setas do teclado
- **Múltiplos mapas** — crie e alterne entre mapas, tudo salvo automaticamente no navegador
- **Personalização via YAML** — controle cores, fonte e tema diretamente no topo do arquivo
- **Conteúdo rico** — links, imagens (`!IMG[url]`), **negrito**, *itálico* e `código inline`
- **Exportação** — PNG em alta resolução ou arquivo `.md` para editar depois
- **Interface premium** — dark mode com gradiente violeta, glassmorphism e micro-animações

## ✍️ Como escrever

A raiz do mapa é sempre um título `#`. A partir daí, use **listas indentadas** — a hierarquia fica clara pelo recuo visual:

```markdown
# Título do Mapa
- Tópico principal
  - Subtópico
    - Detalhe mais profundo
  - Outro subtópico
- Segundo tópico
  - Item A
  - Item B
```

> Dois espaços de indentação = um nível mais fundo na árvore. Tão simples quanto uma lista de compras.

Você também pode usar headings (`##`, `###`) se preferir — ambos funcionam.

### Quebra de linha

Textos longos **quebram automaticamente** dentro dos nós — sem precisar fazer nada. A largura máxima padrão é 260px. Para controlar via YAML:

```yaml
---
max_largura: 200   # px — menor = quebra mais cedo (padrão: 260)
---
```

Para forçar uma quebra manual num ponto específico, use `<br>` no texto do nó:

```markdown
- Primeira linha<br>Segunda linha do mesmo nó
```

### Recursos extras

```markdown
# Mapa com recursos ricos
- **Texto em negrito** e *itálico*
- Link: [YouTube](https://youtube.com)
- Imagem: !IMG[https://url-da-imagem.com/foto.jpg]
- `código inline` nos nós
```

### Personalização com YAML

Coloque um bloco `---` no topo do arquivo para customizar o visual:

```yaml
---
tema: dark          # ou "white" para fundo claro
cor_linhas: "#a78bfa"
cor_destaque: "#c4b5fd"
cor_fonte: "rgba(255,255,255,0.85)"
font_family: "Outfit"   # qualquer fonte do Google Fonts
---
# Seu Mapa
- Tópico
```

Para destacar um nó específico, adicione `(!!)` ao texto:
```markdown
- Ponto mais importante (!!)
```

## ⌨️ Atalhos de teclado

| Tecla | Ação |
| :--- | :--- |
| `→` ou `Espaço` | Revelar próximo nó |
| `←` | Voltar ao nó anterior |
| `E` | Mostrar / ocultar editor |
| `F` | Encaixar o mapa na tela |
| `Esc` | Sair do Modo Foco |
| `Ctrl + T` | Novo mapa |

## 🎬 Para gravações de YouTube

1. Escreva seu mapa no editor
2. Clique em **Foco** na barra superior (ou use o atalho `E` para ocultar o editor)
3. Use `←` `→` para revelar o conteúdo nó por nó durante a explicação
4. Pressione `Esc` a qualquer momento para voltar à interface normal

## 🚀 Como usar

Abra o arquivo `index.html` em qualquer navegador moderno. Não precisa de servidor, instalação ou internet (exceto para carregar as fontes e bibliotecas na primeira vez).

## 🛠️ Tecnologias

- **Core**: HTML5, CSS3, Vanilla JavaScript — arquivo único, zero dependências locais
- **Renderização**: [D3.js](https://d3js.org/) + [Markmap](https://markmap.js.org/)
- **Utilitários**: [js-yaml](https://github.com/nodeca/js-yaml) (config) · [html-to-image](https://github.com/bubkoo/html-to-image) (exportação PNG)
- **Fontes**: [Google Fonts](https://fonts.google.com/) — Outfit + JetBrains Mono

---

Desenvolvido com foco em simplicidade, estética visual e usabilidade para apresentações.