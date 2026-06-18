# Monitora — Painel de Controle de Liquidações PMBA

Sistema de dashboard interativo para monitoramento e análise de liquidações da **Polícia Militar da Bahia**, exercício 2026.

## 🚀 Como usar

1. Abra o arquivo `painel_controle_pmba.html` diretamente no navegador (Chrome, Edge ou Firefox).
2. Clique em **"Selecionar arquivo"** ou arraste o arquivo Excel (`.xlsx`) da planilha **Controle** para a área de upload.
3. O painel será carregado automaticamente com os dados.

## ✨ Funcionalidades

- **Upload de Excel** — carrega a planilha `Controle` do arquivo `.xlsx` sem necessidade de servidor
- **Gráficos interativos** — clique em barras, fatias e segmentos para filtrar os dados dinamicamente
- **Chips de filtro ativo** — indicadores visuais dos filtros aplicados, removíveis com um clique
- **Toggle Dark / Light** — alternância de tema com preferência salva no navegador
- **Filtros em cascata** — Mês, Tipo de instrumento, Grupo de despesa e Unidade Gestora
- **Top 20 credores** com barras de participação
- **Tabela de registros** paginada com busca por texto
- **Totalmente client-side** — nenhum dado é enviado a servidores

## 📊 Gráficos

| Gráfico | Filtro ao clicar |
|---|---|
| Liquidações por mês | Mês |
| Tipo de instrumento (rosca) | Tipo |
| Top 10 unidades gestoras | Unidade Gestora |
| Distribuição mensal por tipo | Mês + Tipo simultaneamente |

## 🗂️ Estrutura da planilha esperada

O sistema detecta automaticamente a aba **"Controle"** e mapeia as colunas:
- `Nome da Unidade Gestora`
- `Tipo do Instrumento`
- `Código e Descrição do Grupo de Despesa`
- `Código e Descrição do Elemento de Despesa`
- `Valor LIQ`
- `Nome do Credor`
- `CPF/CNPJ`
- `Mês`
- `DATA DA LIQ`
- `Histórico/Objeto`

## 🛠️ Tecnologias

- HTML5 + CSS3 + JavaScript (vanilla)
- [Chart.js 4.4.1](https://www.chartjs.org/)
- [SheetJS (xlsx) 0.18.5](https://sheetjs.com/)
- [Google Fonts — Inter](https://fonts.google.com/specimen/Inter)

## 📁 Arquivos

```
Monitora/
├── painel_controle_pmba.html   # Sistema principal
└── README.md
```

> **Nota:** Os arquivos `.xlsx` não são versionados por conterem dados institucionais. Utilize sua própria planilha no formato esperado.

---

Desenvolvido com ❤️ para a PMBA — 2026
