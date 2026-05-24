# Projeto Imobiliária — Análise de Dados com Pandas

Este projeto simula a atuação de um Analista de Dados no setor imobiliário, com foco na exploração, limpeza, transformação e análise estatística de uma base de dados real de aluguéis residenciais e comerciais na cidade do Rio de Janeiro. 

O principal objetivo foi transformar dados brutos em inteligência de negócios, estruturando relatórios e insights visuais para dar suporte à tomada de decisões estratégicas de precificação e investimento.

## 📊 Contexto de Negócio e Objetivos

Dentro de uma operação imobiliária, a consistência dos dados é fundamental para prever tendências de mercado e evitar prejuízos com imóveis desocupados ou precificados incorretamente. Este projeto abordou os seguintes desafios práticos:
- **Saneamento da Base:** Identificar e tratar registros inconsistentes, nulos ou duplicados que distorcem as métricas de desempenho.
- **Segmentação de Mercado:** Agrupar e filtrar imóveis por tipologia (residencial vs. comercial) e localização para análises direcionadas.
- **Métricas Relevantes:** Calcular médias de preços, distribuições de frequência e proporções por categoria.
- **Visualização de Desempenho:** Gerar gráficos claros para facilitar a interpretação dos resultados pelas áreas de negócios.

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Python**: Linguagem principal para desenvolvimento dos scripts.
- **Pandas**: Biblioteca central utilizada para manipulação, limpeza e análise estruturada de dados.
- **Matplotlib**: Biblioteca empregada para a geração de visualizações gráficas (gráficos de barras).
- **Trello (Kanban)**: Ferramenta de gestão de projetos utilizada para organizar o fluxo de tarefas (A Fazer, Em Andamento, Concluído), garantindo previsibilidade e organização no desenvolvimento.

## ⚙️ Habilidades Técnicas Aplicadas (Pipeline de Dados)

O desenvolvimento do projeto cobriu todas as etapas essenciais de manipulação de dados em ambientes corporativos:

### 1. Carga e Diagnóstico Inicial de Dados
- Importação da biblioteca Pandas e leitura de arquivos `.csv`.
- Inspeção inicial da estrutura dos dados através dos métodos `.head()` e `.tail()`.
- Verificação das dimensões do conjunto de dados (`.shape`) e mapeamento dos tipos de variáveis (`.dtypes`).

### 2. Análise Exploratória de Dados (EDA)
- Cálculo de estatísticas descritivas básicas, como médias de valores (`.mean()`).
- Identificação de valores únicos (`.unique()`) e contagem de frequência de categorias (`.value_counts()`).
- Agrupamento de dados (`.groupby()`) combinado com filtros dinâmicos (`.query()`) para analisar o comportamento de variáveis sob diferentes condições de mercado.

### 3. Tratamento de Inconsistências e Limpeza (Data Cleaning)
- Detecção de dados omissos utilizando `.isnull()`.
- Tomada de decisão sobre valores ausentes através da remoção de linhas/colunas inválidas (`.dropna()`) ou inputação de valores substitutos (`.fillna()`).
- Substituição de caracteres ou padrões inconsistentes na base de dados empregando `.replace()`.

### 4. Engenharia de Atributos e Transformação
- Criação e modificação de colunas numéricas, categóricas e binárias para enriquecer a análise.
- Ordenação de DataFrames (`.sort_values()`) para destacar extremos de mercado.
- Aplicação de funções customizadas em massa utilizando `.apply()` combinada com expressões `lambda`.
- Conversão e estruturação de objetos `Series` para estruturas tabulares `DataFrame`.

### 5. Visualização de Dados e Entrega
- Geração de gráficos de barras via `Matplotlib` para comparar o valor médio de aluguel por tipo de imóvel.
- Exportação das bases de dados tratadas e filtradas de volta para o formato `.csv` pronto para consumo por ferramentas de BI ou relatórios gerenciais.

## 📁 Estrutura do Repositório

- `dados/`: Diretório contendo os arquivos `.csv` originais e os arquivos tratados resultantes da análise.
- `notebooks/`: Jupyter Notebooks contendo o código passo a passo, documentado e com as análises exploratórias.
- `README.md`: Documentação técnica do projeto.

---
*Projeto desenvolvido como parte da formação em dados na plataforma Alura, sob orientação da instrutora Milena Gena.*
