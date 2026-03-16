# Consumo de Álcool em Estudantes: Análise Estatística

Projeto da disciplina de **Estatística Descritiva** do MBA em Ciência de Dados.

## Objetivo

Analisar o consumo de álcool de estudantes do ensino médio em Portugal, identificando padrões relacionados a hábitos sociais, desempenho escolar e variáveis demográficas.

## Dados

| Arquivo | Fonte | Descrição |
|---|---|---|
| `Student_Alcohol.csv` | UCI / Kaggle | Dataset principal: 395 estudantes com notas, hábitos e consumo de álcool |
| `colunas_pt.json` | Autoria própria | Mapeamento de nomes de colunas para português |
| `valores_pt.json` | Autoria própria | Mapeamento de valores categóricos para português |

Fonte externa: [Kaggle — Student Alcohol Consumption](https://www.kaggle.com/datasets/uciml/student-alcohol-consumption)

## Estrutura do Notebook

1. **Imports**
2. **Preparação do Dataset:** carregamento do CSV, tradução de colunas e valores, visão geral
3. **Análise Exploratória**
   - 3.1 Distribuição por Endereço
   - 3.2 Consumo de Álcool em Dias Úteis
   - 3.3 Consumo por Endereço
   - 3.4 Consumo por Status dos Pais
   - 3.5 Nota Final × Tempo de Estudo por Nível de Álcool
4. **Síntese e Conclusões**
   - 4.1 Medidas Descritivas Gerais
   - 4.2 Síntese: Consumo × Desempenho
   - 4.3 Conclusões

## Principais Achados

**Perfil da amostra:** 395 estudantes, 77.7% urbanos. 88.9% consomem muito baixo ou baixo álcool em dias úteis.

**Consumo e endereço:** estudantes rurais apresentam consumo médio mais alto (12.5%) que urbanos (4.9%), mas a desproporção da amostra (307 vs 88) limita comparações absolutas.

**Consumo e estrutura familiar:** estudantes com pais separados têm maior proporção de consumo médio e alto (14.7% vs 8.2%), porém o grupo representa apenas 41 estudantes (10.4% da amostra).

**Consumo e desempenho:** os dados não mostram associação entre consumo de álcool e aprovação. O grupo de muito alto consumo tem 77.8% de aprovação, acima de baixo (58.7%) e medio (65.4%). Não há padrão linear. Os grupos de alto e muito alto somam apenas 18 estudantes, o que limita qualquer conclusão sobre esses níveis.

**Mecanismo observado:** o que os dados mostram com clareza é a associação entre consumo e tempo de estudo. Quem bebe mais durante os dias de semana estuda menos. A média de tempo de estudo no grupo de muito baixo consumo é 2.14, contra valores abaixo de 1.88 nos demais grupos.

## Requisitos

```
pandas
matplotlib
scipy
numpy
```
