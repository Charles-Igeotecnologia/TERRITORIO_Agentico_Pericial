# Controle de Versões

## Convenção
Usar versionamento semântico para o projeto: `MAJOR.MINOR.PATCH`.

- **MAJOR**: alteração estrutural incompatível com versões anteriores.
- **MINOR**: nova funcionalidade, módulo, workflow ou conjunto de dados compatível.
- **PATCH**: correção, ajuste documental ou melhoria sem mudança estrutural.

## Estado atual
- Versão: **0.2.0**
- Data: 24/09/2026
- Situação: estrutura-base operacional com padrão de saída para planta georreferenciada e memorial descritivo.

## Alterações da versão 0.2.0
- criação do padrão operacional de planta georreferenciada e memorial descritivo;
- definição de fonte única de dados entre planta, quadro analítico e memorial;
- memorial obrigatório em PDF e DOCX editável;
- padronização de quadrícula, Norte, legenda, escala gráfica e painel técnico;
- regra explícita de prevenção de sobreposição de elementos;
- inclusão de conferência visual obrigatória antes da entrega.

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
