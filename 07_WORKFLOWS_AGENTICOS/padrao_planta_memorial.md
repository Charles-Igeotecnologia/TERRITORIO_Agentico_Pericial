# Padrão de Saída — Planta Georreferenciada e Memorial Descritivo

**Versão operacional do projeto: 0.2.1**

## Finalidade
Definir o modelo operacional obrigatório para geração de planta planimétrica/georreferenciada e memorial descritivo no Território Agêntico Pericial.

Este arquivo contém **regras de composição e validação**. Os valores de coordenadas, confrontantes, áreas, perímetros, inscrições e demais dados pertencem a cada caso concreto e não devem ser reutilizados automaticamente.

## 1. Fonte única de dados
Planta, quadro analítico, memorial PDF e memorial DOCX devem ser derivados da mesma base técnica do caso.

Qualquer alteração em vértice, coordenada, confrontação, azimute, distância, área, perímetro, inscrição cadastral, IPTU, endereço ou sistema de referência deve repercutir em todos os produtos derivados.

Não manter valores divergentes entre quadro analítico, planta e memorial.

## 2. Planta planimétrica/georreferenciada

### 2.1 Representação
- Priorizar representação vetorial.
- Não utilizar base raster quando o produto solicitado for a versão vetorial limpa.
- Preservar poligonal, vértices, confrontações, quadro analítico, quadrícula, norte, escala gráfica, legenda e dados cadastrais.
- Coordenadas dos vértices devem permanecer no quadro analítico; não repeti-las ao lado de P1, P2, P3 etc.

### 2.2 Distâncias e azimutes
- Exibir distância e azimute paralelos ao respectivo segmento.
- Manter afastamento suficiente da linha da poligonal.
- Não permitir sobreposição com vértices, confrontações, quadrícula ou textos cadastrais.

### 2.3 Quadrícula e coordenadas marginais
- Confinar integralmente as linhas de grid ao quadro cartográfico.
- Nenhuma linha da quadrícula pode avançar sobre tabela, legenda, carimbo ou demais blocos.
- Valores E/N devem ficar alinhados às respectivas linhas da quadrícula e próximos às bordas internas do quadro cartográfico.
- Manter correlação direta entre linha da quadrícula e respectivo rótulo de coordenada.

### 2.4 Norte
- Posicionar o Norte dentro do quadro cartográfico.
- Evitar criar espaço externo desnecessário apenas para o símbolo de orientação.
- O Norte não deve cobrir poligonal, confrontações, rótulos ou quadrícula.

### 2.5 Painel técnico lateral
Organizar os elementos na seguinte ordem:

1. Sistema de Referência;
2. linha divisória;
3. Legenda;
4. linha divisória;
5. Escala Gráfica;
6. linha divisória;
7. Planta Georreferenciada do Imóvel / dados cadastrais.

Regras:
- Não utilizar quadro envolvendo a legenda.
- Não utilizar quadros que provoquem sobreposição entre seções.
- Usar apenas linhas divisórias horizontais entre blocos.
- Após a última descrição cadastral, não inserir linha que atravesse ou encoste no texto.
- Manter respiro visual antes do quadro analítico.
- Nenhum bloco pode ocupar a área reservada à tabela de coordenadas.

### 2.6 Legenda
A legenda deve identificar, quando presentes:
- limite do imóvel;
- vértices da poligonal;
- quadrícula RTM ou sistema utilizado;
- confrontações;
- outros elementos vetoriais relevantes.

### 2.7 Escala gráfica
- Inserir escala gráfica obrigatoriamente.
- Vincular seu comprimento à escala efetiva do desenho.
- Posicionar em bloco próprio, sem sobreposição com legenda, sistema de referência ou dados cadastrais.
- Evitar depender apenas de escala numérica.

### 2.8 Sistema de referência
- Informar somente o CRS efetivamente documentado para o caso.
- Registrar datum, projeção, meridiano central, unidades e demais parâmetros aplicáveis.
- Não presumir que todos os casos utilizam o mesmo RTM.
- Parâmetros do caso-modelo servem apenas como exemplo quando coincidirem com a documentação do novo caso.

### 2.9 Quadro analítico
O quadro deve conter, quando disponíveis:
- De;
- Para;
- E;
- N;
- Distância;
- Azimute;
- Confrontações.

As coordenadas do quadro analítico constituem a fonte numérica principal para a geração do memorial.

## 3. Memorial Descritivo

### 3.1 Formatos obrigatórios
Sempre que o memorial for gerado, produzir simultaneamente:
- PDF;
- DOCX editável.

Ambos devem derivar da mesma base técnica e conter o mesmo conteúdo.

### 3.2 Estrutura
O memorial deve conter, conforme aplicável:
- título;
- interessado;
- localização;
- bairro;
- área;
- perímetro;
- ART/RRT;
- IPTU;
- inscrição cadastral;
- data;
- limites e confrontações;
- descrição do perímetro;
- sistema de referência;
- campos de assinatura.

### 3.3 Formatação textual
- Justificar os textos de **Limites e Confrontações**.
- Justificar o texto da **Descrição do Perímetro**.
- Manter padrão tipográfico e hierarquia visual consistentes.
- Evitar aparência de documento digitalizado ou escaneado.
- Gerar texto nativo/editável, preservando seleção e cópia no PDF quando tecnicamente possível.

### 3.4 Precisão numérica
- Utilizar no memorial as coordenadas analíticas da fonte principal.
- Não criar arredondamentos diferentes entre tabela e memorial.
- Área e perímetro devem ser calculados a partir da geometria/coordenadas com precisão integral; valores exibidos podem ser formatados apenas na apresentação.
- Quando houver diferença entre soma de distâncias arredondadas e perímetro calculado geometricamente, prevalece o cálculo geométrico devidamente documentado.

## 4. Controle de sobreposição
Antes da entrega, executar conferência visual obrigatória.

Verificar:
- textos sobre linhas;
- linhas sobre textos;
- grid sobre tabela;
- legenda sobre sistema de referência;
- escala sobre dados cadastrais;
- dados cadastrais sobre quadro analítico;
- norte sobre poligonal ou rótulos;
- cortes em margens;
- elementos fora do quadro cartográfico.

Qualquer sobreposição deve ser tratada como erro de layout e corrigida antes da entrega.

## 5. Produtos mínimos
Quando solicitado o conjunto completo:
1. Planta georreferenciada em PDF vetorial;
2. Memorial descritivo em PDF;
3. Memorial descritivo em DOCX editável;
4. Quando aplicável, conjunto PDF reunindo planta e memorial.

## 6. Sincronização de versão
A versão declarada neste workflow deve permanecer idêntica à versão corrente do projeto registrada em:
- `../README.md`;
- `../catalogo.json`;
- `../00_DOCUMENTACAO/CONTROLE_VERSOES.md`;
- `../AGENTS.md`.

Sempre que a versão do projeto for alterada, atualizar este arquivo na mesma operação.

## 7. Validação humana
Os produtos gerados automaticamente devem ser submetidos à revisão humana antes de uso oficial, assinatura ou emissão vinculada à responsabilidade técnica.
