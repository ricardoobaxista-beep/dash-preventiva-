# ⚡ Dashboard Preventiva

Painel de controle de produção, faturamento e equipes — construído em HTML/CSS/JS puro, sem dependência de backend.

## ✨ Funcionalidades

- 📊 Gráficos interativos (Chart.js) com KPIs de produção e faturamento
- 📁 Importação de dados via planilha Excel/CSV (SheetJS)
- 📝 Lançamento manual de registros e justificativas (dias parados, motivos)
- 📤 Exportação de relatórios em imagem/PDF (html2canvas + jsPDF)
- 🌗 Tema claro/escuro com preferência salva no navegador
- 🧪 Modo de dados de demonstração para testar o painel sem planilha real

## 🚀 Como usar

### Localmente
Basta abrir o arquivo `index.html` em qualquer navegador moderno — não requer instalação, servidor ou build.

### Publicando no GitHub Pages
1. Suba este repositório no GitHub
2. Vá em **Settings → Pages**
3. Em **Source**, selecione a branch `main` e a pasta `/ (root)`
4. Salve — o dashboard ficará disponível em `https://<seu-usuario>.github.io/<nome-do-repositorio>/`

## 🛠️ Tecnologias

| Biblioteca | Uso |
|---|---|
| [Chart.js](https://www.chartjs.org/) | Gráficos |
| [chartjs-plugin-datalabels](https://chartjs-plugin-datalabels.netlify.app/) | Rótulos de dados nos gráficos |
| [SheetJS (xlsx)](https://sheetjs.com/) | Leitura de planilhas Excel/CSV |
| [html2canvas](https://html2canvas.hertzen.com/) | Captura de tela para exportação |
| [jsPDF](https://github.com/parallax/jsPDF) | Geração de PDF |

## 📂 Estrutura

```
.
├── index.html   # Aplicação completa (HTML + CSS + JS)
└── README.md
```

## ⚠️ Observações

- Todos os dados são processados **localmente no navegador** — nada é enviado para servidores externos.
- Os dados carregados (planilhas, lançamentos manuais) não são persistidos entre sessões, exceto a preferência de tema, que fica salva em `localStorage`.
