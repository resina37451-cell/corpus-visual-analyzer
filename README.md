# Corpus Visual Analyzer

**Ferramenta de análise exploratória e triagem para revisões sistemáticas**

Criado por **Felipe Villela**

https://resina37451-cell.github.io/corpus-visual-analyzer

---

## O que é

O **Corpus Visual Analyzer** é um programa de página única (HTML) que roda inteiramente no navegador — sem servidor, sem instalação, sem envio de dados para nenhum lugar. Ele recebe arquivos bibliográficos nos formatos **RIS** e **NBIB** (exportados do PubMed, Zotero, Rayyan, Covidence etc.) e oferece três ambientes de trabalho integrados:

| Aba | O que faz |
|---|---|
| **Ordination cloud** | Mapa determinístico que posiciona cada artigo pelo número de categorias PICOS cobertas (eixo X) e pelo ano de publicação (eixo Y). Clique em qualquer ponto para abrir o abstract. |
| **Análise de termos** | Lista os termos mais representativos do corpus, frequência geral em gráfico de barras e combinações de termos PICOS com termos sugeridos. |
| **Triagem** | Interface de inclusão/exclusão artigo a artigo com exportação dos resultados em RIS ou TXT. |

---

## Funcionalidades principais

- **Upload de arquivo RIS ou NBIB** — arraste e solte ou selecione pelo botão
- **Corpus de demonstração** embutido para teste imediato
- **Configuração PICOS** — defina população, intervenção, comparação, desfechos e tipos de estudo antes de analisar
- **Motor de análise** — TF-IDF leve rodando no próprio navegador
- **Mapa Ordination cloud** com Plotly.js — interativo, com zoom e hover
- **Lista de artigos** com busca por título, abstract, ano, DOI ou PMID; filtros AND/NOT; ordenação por data
- **ABS deck** — modo de leitura rápida de abstracts estilo "cartas"
- **Sublinhado automático** de termos PICOS e de classificação no abstract
- **Triagem** com contadores de incluídos / excluídos / não revisados
- **Exportação** de incluídos e excluídos em `.ris` e `.txt`
- **Exportar / importar sessão** em JSON para retomar o trabalho depois
- **Tema claro e escuro** com alternância pelo botão ☾/☀
- **Painéis redimensionáveis** (sidebar, lista de artigos, painel de abstract)
- **100 % offline** após o primeiro carregamento — nenhum dado sai do navegador

---

## Como usar

### Online (GitHub Pages)

Acesse diretamente pelo link do GitHub Pages deste repositório — nenhuma instalação necessária.

### Localmente

1. Baixe o arquivo `index.html`
2. Abra-o em qualquer navegador moderno (Chrome, Brave, Firefox, Edge)
3. Pronto — o programa já está funcionando

### Instalar como aplicativo no Brave (ou Chrome)

1. Abra a página no Brave
2. Clique no ícone **⊕** na barra de endereços (ou menu → *Instalar Corpus Visual Analyzer*)
3. Confirme a instalação
4. O programa aparecerá como um aplicativo independente na sua área de trabalho

---

## Fluxo de trabalho típico

```
1. Abrir o programa
2. Configurar área de pesquisa e critérios PICOS
3. Fazer upload do arquivo RIS / NBIB exportado do seu gerenciador de referências
4. Explorar o Ordination cloud para ter uma visão geral do corpus
5. Usar a Análise de termos para refinar o vocabulário de busca
6. Triar os artigos um a um na aba Triagem
7. Exportar os incluídos em RIS para importar no Zotero, Rayyan etc.
8. Salvar a sessão em JSON para continuar depois
```

---

## Formatos de entrada suportados

| Formato | Extensão | Exportado por |
|---|---|---|
| RIS | `.ris` | Zotero, Rayyan, PubMed, Covidence, EndNote, Scopus, Web of Science |
| NBIB (PubMed) | `.nbib` | PubMed |
| Texto simples RIS | `.txt` | Qualquer exportador que salve RIS como texto |

---

## Tecnologias utilizadas

- **HTML5 / CSS3 / JavaScript** puro — zero dependências de framework
- **[Plotly.js](https://plotly.com/javascript/)** (CDN) — gráficos interativos
- **TF-IDF** implementado diretamente no navegador

---

## Privacidade

Nenhum dado é enviado para servidores externos. Todo o processamento acontece localmente no navegador do usuário. O único recurso externo carregado é a biblioteca Plotly.js via CDN ao abrir a página pela primeira vez.

---

## Licença

Distribuído livremente para uso em pesquisa acadêmica.

---

## Autor

**Felipe Villela**  
Ferramenta desenvolvida para apoiar revisões sistemáticas e metanálises.
