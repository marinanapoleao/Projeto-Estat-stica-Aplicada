# Projeto Estatística Aplicada
<img width="1364" height="768" alt="Estatística Aplicada" src="https://github.com/user-attachments/assets/f962a043-a524-449c-a142-bc5f1b4bc532" />

## 📌 Sobre o Projeto

Projeto de estatística aplicada que investiga a diferença de desempenho entre duas estratégias de ensino de matemática para alunos do ensino médio.

O trabalho utiliza amostras de notas geradas por distribuições normais para comparar as médias de desempenho dos dois grupos e verificar, por meio de um teste de hipóteses, se existe diferença estatisticamente significativa entre as estratégias.

## 🎯 Objetivo

Comparar o desempenho médio de alunos submetidos a duas estratégias de ensino (A e B), utilizando testes estatísticos para avaliar se a Estratégia B apresenta resultados significativamente superiores à Estratégia A.

## 💻​ Problema de Negócio / Pergunta de Pesquisa

Uma escola deseja avaliar a eficácia de duas estratégias de ensino de matemática para alunos do ensino médio.

A principal pergunta de pesquisa é:

*A Estratégia B apresenta uma média de notas significativamente maior do que a Estratégia A?*

O projeto busca verificar se a diferença observada entre as médias das duas amostras é estatisticamente significativa ou se pode ser explicada pela variabilidade dos dados.

## 📊 Fonte de Dados

O projeto utiliza dados sintéticos, gerados por meio da biblioteca NumPy, simulando notas de alunos submetidos a duas estratégias de ensino.

Foram criadas duas amostras:

Característica	Estratégia A	Estratégia B

Quantidade de alunos	50	50

Média definida para geração	70	75

Desvio padrão definido	10	12

As amostras foram geradas utilizando a distribuição normal (np.random.normal), com semente aleatória np.random.seed(0) para garantir a reprodutibilidade.

Portanto, é importante destacar que o projeto não utiliza notas reais coletadas de uma escola, mas sim dados simulados para aplicar conceitos de inferência estatística.

## 🛠️ LINGUAGENS E BIBLIOTECAS

- Python: linguagem de programação.

- NumPy: geração das amostras, operações matemáticas e cálculos estatísticos.

- SciPy: testes estatísticos, distribuição normal e distribuição t.

- Matplotlib: construção de gráficos das distribuições estatísticas.

- Pandas, Seaborn e Plotly Express: bibliotecas importadas no ambiente do projeto, mas sem utilização significativa nas análises apresentadas.

## 🔍 Metodologia

*1. Formulação das hipóteses*

O projeto estabelece as seguintes hipóteses:

- H0 (hipótese nula): as médias das notas das duas estratégias são iguais.
- H1 (hipótese alternativa): a média da Estratégia B é maior que a média da Estratégia A.

*2. Geração das amostras*
- Geração de 50 observações para a Estratégia A.
- Geração de 50 observações para a Estratégia B.
- Utilização de distribuições normais com médias e desvios padrão previamente definidos.

*3. Análise descritiva*
- Cálculo das médias amostrais.
- Cálculo das variâncias amostrais.
- Comparação da dispersão das notas entre os grupos.

*4. Definição do teste estatístico*
- Investigação do teste unilateral à direita.
- Definição do nível de significância de 5% (α = 0,05).
- Comparação do desempenho médio das estratégias.

*5. Aplicação do teste Z*
- Cálculo da estatística Z.
- Cálculo do p-valor unilateral e bilateral.
- Comparação do p-valor com o nível de significância.
- Decisão sobre rejeitar ou não a hipótese nula.

*6. Visualização dos resultados*
- Construção de gráfico da distribuição t com região crítica.
- Construção de gráfico da distribuição normal padrão.
- Representação da estatística de teste e das regiões críticas para facilitar a interpretação.
- 
## 📈  Resultados e Métricas

*Estatísticas descritivas das amostras*

Indicador	Estratégia A	Estratégia B
Quantidade de observações	50	50
Média das notas	71,41	74,75
Variância amostral	129,27	110,47
Desvio padrão amostral	11,37	10,51

Diferença entre as médias

74,75-71,41=3,34

A Estratégia B apresentou uma média aproximadamente 3,34 pontos superior à Estratégia A.

*Resultado do teste de hipóteses*

Indicador ----------	Resultado

Estatística Z ----------	1,5133

p-valor unilateral -----	0,0651

p-valor bilateral ------	0,1302

Nível de significância ----	0,05


Não rejeitamos a hipótese nula (H0).

O p-valor unilateral foi de 0,0651, superior ao nível de significância de 0,05.

Portanto, não existem evidências estatísticas suficientes para afirmar que a Estratégia B apresenta uma média de notas significativamente superior à Estratégia A.

## 💡 Principais Insights e Implicações

#### *1. Estratégia B apresenta maior média de desempenho*

- A média das notas da Estratégia B foi de 74,75, enquanto a Estratégia A apresentou média de 71,41.

- A diferença observada foi de aproximadamente 3,34 pontos.

- Implicação para o negócio: a diferença observada pode justificar novas investigações sobre os métodos de ensino, buscando compreender se existem características da Estratégia B que possam favorecer o aprendizado.

#### *2. Estratégia B apresenta menor dispersão nas notas*

- A variância da Estratégia B foi de 110,47, inferior à variância de 129,27 da Estratégia A.

- Isso indica que, na amostra simulada, as notas da Estratégia B apresentam menor dispersão em relação à sua média.

- Implicação para o negócio: investigar se a estratégia apresenta resultados mais consistentes entre os alunos.

#### *3. Diferença entre as médias não apresenta significância estatística*

- Apesar da média superior da Estratégia B, o p-valor unilateral foi de 0,0651, acima do limite de 0,05.

- Implicação para o negócio: não é possível concluir que a Estratégia B seja efetivamente superior à Estratégia A com base nos resultados obtidos.

#### *4. Visualização da região crítica facilita a interpretação*

- O gráfico da distribuição normal padrão permite observar a posição da estatística Z em relação às regiões críticas de rejeição da hipótese nula.

- O valor observado, aproximadamente 1,51, não ultrapassou o limite crítico correspondente ao teste bilateral apresentado no gráfico final.

- Implicação para o negócio: a visualização facilita a comunicação dos resultados estatísticos e a compreensão da decisão tomada.

#### *5. A importância da inferência estatística na tomada de decisão*

- O projeto demonstra que uma diferença observada entre duas médias não significa necessariamente que exista uma diferença estatisticamente significativa entre os grupos.

- Implicação para o negócio: decisões sobre a adoção de novas estratégias educacionais devem considerar não apenas as médias observadas, mas também a variabilidade e a significância estatística dos resultados.

## 👩‍💻 Sobre a Autora

Desenvolvido por Marina Napoleão — Cientista de Dados / Analista de Dados. 
### LinkedIn <https://www.linkedin.com/in/marina-napoleao/>
### GitHub <https://github.com/marinanapoleao> 
