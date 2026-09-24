# Workflow — Reconstituição Cartográfica

## Entrada
Planta, croqui, memorial, quadro de coordenadas, imagem digitalizada ou descrição perimetral.

## Procedimento
1. Identificar escala, orientação, referências e sistema geodésico declarados.
2. Vetorizar apenas elementos identificáveis, preservando a distinção entre leitura e inferência.
3. Quando houver coordenadas, reconstruir vértices a partir dos valores documentados.
4. Quando houver rumos/azimutes e distâncias, calcular a poligonal e verificar fechamento.
5. Quando houver imagem sem coordenadas, selecionar controles justificáveis e registrar o método de transformação.
6. Calcular resíduos, área, perímetro e discrepâncias relevantes.
7. Comparar a geometria reconstituída com bases de referência somente após harmonização de CRS.
8. Produzir versão vetorial, tabela de vértices e relatório de inconsistências.

## Controles
- não forçar fechamento sem registrar o ajuste;
- não assumir Norte verdadeiro, magnético ou de quadrícula sem evidência;
- não atribuir precisão superior à permitida pela fonte;
- registrar qualquer transformação entre SAD69, SIRGAS 2000 e outros referenciais.
