Este projeto analisa os resultados do Exame Nacional do Ensino Médio (ENEM) de 2019 no estado de São Paulo. O objetivo principal é explorar e interpretar os dados para identificar padrões e obter insights relevantes sobre o desempenho dos participantes.

Os dados foram obtidos no site oficial do INEP: Microdados ENEM.

Detalhamento Técnico

Limpar e transformar os dados para garantir a qualidade da análise.

Realizar uma análise exploratória para identificar padrões e relações nos dados.

Fornecer uma base organizada para visualizações e análises estatísticas mais aprofundadas.

Principais Etapas do Projeto

1. Extração e Limpeza de Dados

Fonte dos dados: O arquivo de micro dados foi carregado e lido utilizando a biblioteca Pandas.

Ajustes realizados:

Remoção de colunas desnecessárias, como códigos redundantes de UF e municípios.

Tratamento de valores ausentes em campos importantes, como notas das provas.

Correção de escalas de notas que estavam fora do padrão (ex.: divisão por 10 em algumas variáveis).

Renomeação de colunas para melhorar a compreensão (ex.: NU_NOTA_CN para NOTA_CN).

2. Transformação de Dados

Categorias reorganizadas:

A classificação de raça foi substituída por valores descritivos (ex.: "1" para "Branca").

Informações como tipo de escola e acesso à internet também foram ajustadas para valores textuais.

Filtragem:

Exclusão de registros com idades menores que 12 anos devido à alta probabilidade de erros.

Separação entre treineiros e vestibulandos para análises mais específicas.

3. Análise Exploratória

Distribuição de idades: A maior parte dos participantes está na faixa etária de 16 a 20 anos.

Taxas de presença:

Provas de Linguagens e Códigos e Ciências Humanas tiveram as maiores taxas de presença.

Números consideráveis de ausências foram registrados em todas as provas.

Notas:

Notas foram avaliadas para identificar padrões de desempenho.
Casos de nota zero na redação foram destacados.

* Resultados Destacados

Presença nas provas:

Ciências da Natureza: 500.805 presentes, 218.693 ausentes, 270 eliminados.
Ciências Humanas: 533.142 presentes, 185.969 ausentes, 657 eliminados.
Linguagens e Códigos: 533.142 presentes, 185.969 ausentes, 657 eliminados.
Matemática: 500.805 presentes, 218.693 ausentes, 270 eliminados.

Notas da Redação:

Casos de nota zero foram analisados e relacionados às composições individuais (COMP1, COMP2, etc.).
Principais faixas de nota incluem 540 a 640 pontos.

* Possíveis Aplicações

Políticas Públicas: Os insights obtidos podem auxiliar na formulação de políticas educacionais para melhorar o desempenho e a participação dos alunos, realizando estudos também nos anteriores e seguintes da análise.

Estudos Acadêmicos: O conjunto de dados tratado e os códigos disponibilizados podem ser úteis para pesquisadores em estudos futuros.

Gestão Escolar: As escolas podem identificar grupos que necessitam de maior suporte acadêmico.
