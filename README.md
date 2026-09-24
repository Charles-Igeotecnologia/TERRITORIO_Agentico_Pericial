# TERRITÓRIO Agêntico Pericial

Ambiente técnico para organização, análise e produção de informação territorial aplicada a atividades periciais, reconstituição cartográfica, georreferenciamento, análise espacial e geração de produtos técnico-documentais.

## Versão
**v0.1.0 — estrutura-base operacional**

## Objetivos
- preservar rastreabilidade de documentos, bases e transformações;
- apoiar leitura documental e extração de elementos espaciais;
- reconstituir plantas, memoriais e poligonais;
- analisar confrontações, divergências e sobreposições;
- organizar bases cartográficas e dados de imóveis;
- gerar mapas, tabelas, notas técnicas, laudos, plantas e memoriais;
- preparar uma camada WebGIS para consulta e apresentação de resultados;
- estabelecer workflows agênticos com revisão humana obrigatória.

## Estrutura
```text
TERRITORIO_Agentico_Pericial/
├── README.md
├── AGENTS.md
├── catalogo.json
├── 00_DOCUMENTACAO/
├── 01_BASE_CARTOGRAFICA/
├── 02_IMOVEIS_E_POLIGONAIS/
├── 03_RECONSTITUICAO_CARTOGRAFICA/
├── 04_ANALISE_ESPACIAL/
├── 05_PRODUTOS_PERICIAIS/
├── 06_WEBGIS/
└── 07_WORKFLOWS_AGENTICOS/
```

## Princípios
O projeto distingue documento-fonte, observação, dado derivado, inferência técnica e conclusão. Sistemas de referência espacial não devem ser presumidos. Toda transformação, reprojeção, georreferenciamento ou ajuste geométrico deve permanecer documentado.

## Fluxo principal
**Documento → identificação espacial → validação do CRS → reconstituição → consistência geométrica → sobreposição/confrontação → produtos cartográficos → produto pericial → revisão humana.**

## Governança agêntica
As regras operacionais estão em [`AGENTS.md`](AGENTS.md). Os procedimentos especializados ficam em [`07_WORKFLOWS_AGENTICOS`](07_WORKFLOWS_AGENTICOS/).

## Situação atual
A versão 0.1 estabelece o núcleo metodológico e documental. As próximas etapas são incorporar bases de referência, modelos de dados, rotinas de validação geoespacial e componentes do WebGIS.
