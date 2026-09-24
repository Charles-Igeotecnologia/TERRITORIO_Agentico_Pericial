# TERRITÓRIO Agêntico Pericial

Ambiente técnico para organização, análise e produção de informação territorial aplicada a atividades periciais, reconstituição cartográfica, georreferenciamento, análise espacial e geração de produtos técnico-documentais.

## Versão
**v0.2.1 — padrão operacional sincronizado**

## Objetivos
- preservar rastreabilidade de documentos, bases e transformações;
- apoiar leitura documental e extração de elementos espaciais;
- reconstituir plantas, memoriais e poligonais;
- analisar confrontações, divergências e sobreposições;
- organizar bases cartográficas e dados de imóveis;
- gerar mapas, tabelas, notas técnicas, laudos, plantas e memoriais;
- preparar uma camada WebGIS para consulta e apresentação de resultados;
- estabelecer workflows agênticos com revisão humana obrigatória;
- manter sincronização documental de versão em todos os arquivos que declaram a versão do projeto.

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
**Documento → identificação espacial → validação do CRS → reconstituição → consistência geométrica → sobreposição/confrontação → produtos cartográficos → produto pericial → verificação documental e visual → revisão humana.**

## Governança agêntica
As regras operacionais estão em [`AGENTS.md`](AGENTS.md). Os procedimentos especializados ficam em [`07_WORKFLOWS_AGENTICOS`](07_WORKFLOWS_AGENTICOS/).

O padrão específico para planta georreferenciada e memorial descritivo está em:

`07_WORKFLOWS_AGENTICOS/padrao_planta_memorial.md`

## Controle de versão
A versão declarada neste README deve ser idêntica à registrada em:
- `catalogo.json`;
- `00_DOCUMENTACAO/CONTROLE_VERSOES.md`;
- demais documentos que exibam explicitamente a versão operacional do projeto.

Qualquer atualização de versão deve alterar todos esses registros na mesma operação, evitando divergência documental.

## Situação atual
A versão **0.2.1** consolida o padrão de saída de planta georreferenciada e memorial descritivo, a geração obrigatória do memorial em PDF e DOCX editável, a prevenção de sobreposições de layout e a sincronização documental de versão.
