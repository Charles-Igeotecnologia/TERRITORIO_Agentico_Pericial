# 05 — Produtos Periciais

**Versão operacional do projeto: 0.2.1**

Área destinada aos produtos técnico-documentais consolidados.

Subcategorias previstas:
- `notas_tecnicas/`;
- `laudos/`;
- `plantas/`;
- `memoriais_descritivos/`.

Todo produto deve indicar versão, fontes, metodologia, limitações e vínculo com os dados que lhe deram origem.

## Planta georreferenciada
A planta deverá seguir o padrão definido em:

`../07_WORKFLOWS_AGENTICOS/padrao_planta_memorial.md`

O padrão prevê representação vetorial, quadro analítico, quadrícula confinada ao mapa, Norte integrado ao quadro cartográfico, legenda, escala gráfica e painel técnico organizado sem sobreposição.

## Memorial descritivo
Sempre gerar:
- PDF;
- DOCX editável.

O PDF e o DOCX devem derivar da mesma base técnica, mantendo coerência de coordenadas, distâncias, azimutes, área, perímetro e confrontações.

## Regra de qualidade
Nenhum produto deve ser entregue com sobreposição de textos, linhas, quadrícula, legenda, escala, dados cadastrais ou tabela analítica.

## Regra de versão
A versão operacional indicada neste documento deve permanecer idêntica à versão corrente registrada em `../README.md`, `../catalogo.json` e `../00_DOCUMENTACAO/CONTROLE_VERSOES.md`.
