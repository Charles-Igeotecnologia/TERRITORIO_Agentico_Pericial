# AGENTS.md — Território Agêntico Pericial

## Finalidade
Orientar agentes de IA e colaboradores humanos na leitura, organização, análise e produção de resultados técnico-cartográficos e periciais.

## Princípios operacionais
1. Preservar rastreabilidade de fontes, versões e transformações.
2. Nunca assumir sistema de referência espacial quando não estiver explicitamente documentado.
3. Registrar datum, projeção, EPSG, unidade, origem e data de cada base.
4. Separar evidência documental, dado observado, inferência técnica e conclusão.
5. Não alterar dados-fonte originais; trabalhar com cópias versionadas.
6. Toda reconstituição cartográfica deve registrar pontos de controle, método de ajuste, resíduos e limitações.
7. Sobreposições devem ser descritas com critério geométrico, tolerância e fonte das camadas comparadas.
8. Produtos periciais devem indicar metodologia, fontes, limitações e responsabilidade técnica aplicável.

## Fluxo agêntico padrão
1. Leitura documental.
2. Identificação espacial e cadastral.
3. Validação de referência geodésica/cartográfica.
4. Reconstituição vetorial, quando necessária.
5. Fechamento e consistência de poligonais.
6. Análise de confrontações e sobreposições.
7. Geração de mapas, tabelas e métricas.
8. Produção de nota técnica, laudo, planta ou memorial.
9. Revisão humana obrigatória antes de uso oficial.

## Regras de evidência
- Documento original: fonte primária.
- Base oficial: registrar órgão, camada, data e acesso.
- Conversão/reprojeção: registrar CRS de origem e destino.
- Georreferenciamento: registrar controles e erro residual.
- Inferências: devem ser explicitamente identificadas como inferência técnica.

## Sistemas de referência
Priorizar SIRGAS 2000 quando aplicável ao contexto brasileiro contemporâneo. Não converter automaticamente dados em SAD69 ou outros referenciais sem registrar transformação e parâmetros utilizados.

## Saídas mínimas
Cada análise deverá, quando aplicável, produzir:
- síntese técnica;
- fontes e metadados;
- mapa ou representação cartográfica;
- tabela de coordenadas/atributos;
- limitações;
- histórico de versão.
