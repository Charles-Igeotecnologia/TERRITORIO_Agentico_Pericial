# AGENTS.md — Território Agêntico Pericial

**Versão operacional do projeto: 0.2.1**

## Finalidade
Orientar agentes de IA e colaboradores humanos na leitura, organização, análise e produção de resultados técnico-cartográficos e periciais.

## Princípios operacionais
1. Preservar rastreabilidade de fontes, versões e transformações.
2. Nunca assumir sistema de referência espacial quando não estiver explicitamente documentado.
3. Registrar datum, projeção, EPSG quando aplicável, unidade, origem e data de cada base.
4. Separar evidência documental, dado observado, inferência técnica e conclusão.
5. Não alterar dados-fonte originais; trabalhar com cópias versionadas.
6. Toda reconstituição cartográfica deve registrar pontos de controle, método de ajuste, resíduos e limitações.
7. Sobreposições devem ser descritas com critério geométrico, tolerância e fonte das camadas comparadas.
8. Produtos periciais devem indicar metodologia, fontes, limitações e responsabilidade técnica aplicável.
9. Planta, quadro analítico e memorial devem utilizar uma única base técnica do caso, evitando divergências entre produtos.
10. Sobreposição visual de elementos de layout deve ser tratada como erro e corrigida antes da entrega.
11. Toda alteração de versão deve manter sincronizados os documentos de governança e catálogos que declarem a versão corrente.

## Fluxo agêntico padrão
1. Leitura documental.
2. Identificação espacial e cadastral.
3. Validação de referência geodésica/cartográfica.
4. Reconstituição vetorial, quando necessária.
5. Fechamento e consistência de poligonais.
6. Análise de confrontações e sobreposições.
7. Geração de mapas, tabelas e métricas.
8. Produção de nota técnica, laudo, planta ou memorial.
9. Verificação de consistência numérica, documental e de layout.
10. Revisão humana obrigatória antes de uso oficial.

## Regras de evidência
- Documento original: fonte primária.
- Base oficial: registrar órgão, camada, data e acesso.
- Conversão/reprojeção: registrar CRS de origem e destino.
- Georreferenciamento: registrar controles e erro residual.
- Inferências: devem ser explicitamente identificadas como inferência técnica.

## Sistemas de referência
Priorizar SIRGAS 2000 quando aplicável ao contexto brasileiro contemporâneo. Não converter automaticamente dados em SAD69 ou outros referenciais sem registrar transformação e parâmetros utilizados. Não presumir que parâmetros RTM de um caso-modelo se aplicam a outros casos.

## Saídas mínimas
Cada análise deverá, quando aplicável, produzir:
- síntese técnica;
- fontes e metadados;
- mapa ou representação cartográfica;
- tabela de coordenadas/atributos;
- limitações;
- histórico de versão.

## Padrão de planta e memorial
Para geração de planta georreferenciada e memorial descritivo, seguir obrigatoriamente:

`07_WORKFLOWS_AGENTICOS/padrao_planta_memorial.md`

Regras essenciais:
- coordenadas dos vértices no quadro analítico, não junto aos pontos;
- distâncias e azimutes paralelos e afastados dos segmentos;
- quadrícula confinada ao quadro cartográfico;
- Norte dentro do quadro do mapa;
- painel técnico separado por linhas divisórias, sem quadros sobrepostos;
- legenda sem caixa externa;
- escala gráfica obrigatória;
- memorial com textos justificados;
- geração simultânea do memorial em PDF e DOCX editável;
- conferência visual obrigatória contra sobreposições antes da entrega.

## Sincronização documental
Antes de concluir qualquer atualização de versão:
1. conferir `README.md`;
2. conferir `catalogo.json`;
3. conferir `00_DOCUMENTACAO/CONTROLE_VERSOES.md`;
4. localizar outros arquivos que declarem a versão corrente;
5. atualizar todos para o mesmo número;
6. pesquisar referências à versão anterior e corrigir aquelas que representem o estado atual.

Referências históricas em changelog podem ser mantidas.
