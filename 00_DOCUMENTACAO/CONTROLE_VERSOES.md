# Controle de Versões

## Convenção
Usar versionamento semântico para o projeto: `MAJOR.MINOR.PATCH`.

- **MAJOR**: alteração estrutural incompatível com versões anteriores.
- **MINOR**: nova funcionalidade, módulo, workflow ou conjunto de dados compatível.
- **PATCH**: correção, ajuste documental, sincronização ou melhoria sem mudança estrutural.

## Estado atual
- Versão: **0.2.1**
- Data: 24/09/2026
- Situação: estrutura-base operacional com padrão de saída para planta georreferenciada e memorial descritivo, incluindo controle de sincronização documental.

## Alterações da versão 0.2.1
- sincronização da versão declarada em todos os arquivos de governança que exibem a versão do projeto;
- atualização de `README.md`, `catalogo.json` e deste controle de versões;
- inclusão de regra permanente para que toda mudança de versão seja replicada, na mesma operação, em todos os documentos que declarem versão operacional;
- reforço da prevenção de divergência documental entre governança, catálogo, workflows e produtos.

## Alterações da versão 0.2.0
- criação do padrão operacional de planta georreferenciada e memorial descritivo;
- definição de fonte única de dados entre planta, quadro analítico e memorial;
- memorial obrigatório em PDF e DOCX editável;
- padronização de quadrícula, Norte, legenda, escala gráfica e painel técnico;
- regra explícita de prevenção de sobreposição de elementos;
- inclusão de conferência visual obrigatória antes da entrega.

## Política de sincronização de versão
Sempre que houver alteração da versão operacional do projeto, atualizar obrigatoriamente, na mesma operação:
1. `README.md`;
2. `catalogo.json`;
3. `00_DOCUMENTACAO/CONTROLE_VERSOES.md`;
4. `AGENTS.md`, quando declarar versão operacional;
5. `05_PRODUTOS_PERICIAIS/README.md`, quando declarar versão operacional;
6. workflows ou manuais que exibam explicitamente a versão corrente.

Antes de concluir a atualização, realizar uma busca no repositório pelas versões anteriores e pela nova versão. Qualquer referência antiga que represente o estado corrente deve ser corrigida.

Versões históricas citadas no changelog podem permanecer, desde que estejam claramente identificadas como histórico.

## Regra contra divergência documental
Nenhum commit de atualização de versão deverá deixar arquivos de governança com números de versão correntes diferentes. Se houver divergência, considerar a atualização incompleta.

## Registro mínimo por alteração
Cada atualização relevante deve indicar:
- data;
- autor/responsável;
- arquivos afetados;
- natureza da mudança;
- fonte ou justificativa;
- impacto sobre produtos derivados.

## Dados geoespaciais
Mudanças em geometrias devem preservar a versão anterior ou registrar claramente a substituição. Alterações em CRS, reprojeções, ajustes de controle, simplificações e correções topológicas devem ser documentadas.
