<img width="1636" height="218" alt="image" src="https://github.com/user-attachments/assets/708b1bf2-e71e-49ba-b34b-6f50a7580b85" />

# Projeto final - Prática em Ciência de Dados 2026

# Gráficos e cálculos e parâmetros estatísticos e incertezas para dados experimentais
**Aluna:** Ana Luiza de Lima Silva.

**Turma:** 2026

**Docentes responsáveis:** Prof. Dr. Daniel Roberto Cassar, Prof. Dr. James Moraes de Almeida e Prof. Dr. Leandro Nascimento Lemos.

**Disciplina:** Prática em Ciência de Dados - 1° semestre de 2026.

**Instituição:** Ilum escola de ciência.

## Descrição do projeto
Projeto final desenvolvido para a disciplina de Práticas em Ciências de Dados no primeiro semestre de 2026. A proposta visa integrar o recebimento, tratamento, organização, visualização e exportação de dados experimentais, permitindo ao usuário a inserção dos dados via arquivos nos formatos .txt e .xlsx ou manualmente, além de possibilitar a exportação de tabelas no formato .xlsx com os parâmetros estatísticos obtidos e gráficos no formato .png conforme o ajuste escolhido dentre as opções - linear, quadrático, exponencial ou logarítmico.

## Objetivo
Desenvolver uma ferramenta computacional em Python para análise estatística de dados experimentais, gerando tabelas e gráficos visualizáveis e exportáveis com as devidas análises de incertezas associadas. O projeto integra o cálculo parâmetros estatísticos, realização de regressões matemáticas baseadas no Método dos Quadrados Mínimos e geração de barras de erro e de bandas de predição e confiança a fim de automatizar o tratamento e visualização desses dados.

## Instalação
Para utilizar o projeto, clone o repositório em sua máquina, garantindo a existência de um ambiente compatível com a linguagem Python, como o JupyterLab. Antes da execução do notebook, garanta a instalação de todas as bibliotecas utilizadas. Execute as células sequencialmente, adicionando os dados experimentais e informações solicitadas.

## Bibliotecas utilizadas
- pandas - utilizada na etapa de inserção e leitura dos dados fornecidos;
  
- numpy - utilizada na etapa de geração dos gráficos e ajustes;
  
- math - utilizada para cálculos associados às funções auxiliares desenvolvidas;
  
- ipywidgets - utilizada para criação de uma interface interativa para guiar o usuário nas etapas de exportação da tabela e escolha dos parâmetros para os gráficos;
  
- matplotlib.pyplot - utilizada para a geração e viualização dos gráficos;
  
- ast - utilização do objeto "literal_eval" durante a etapa de recebimento dos dados para avaliar os dados inseridos pelo usuário;

- scipy.stats - uso do objeto "t" durante a etapa de geração dos gráficos para calcular o valor crítico associado aos valores informados para a análise de incertezas por meio da distribuição t-Student.
  
- IPython.display - uso do objeto "display" para exibição do Dataframe de devolução dos parâmetros estatísticos e dos gráficos e opções de escolha associados aos ajustes e exportações.

## Funcionalidades
- Importação e inserção de dados a partir de arquivos nos formatos .txt ou .xlsx ou via inserção manual a partir de listas;
  
- Cálculo e análise de parâmetros estatísticos, como média simples, desvio padrão amostral ou populacional, variância amostral ou populacional, erro padrão, erro relativo e porcentagem de erro;
  
- Ajustes matemáticos dos tipos lineares, quadráticos, exponenciais e logarítmicos pautados em regressões lineares que se baseiam no Método dos Quadrados Mínimos;
  
- Devolução das equações e coeficientes de determinação (R²) relacionados aos ajustes escolhidos;
  
- Avaliação da qualidade do ajuste escolhido;
  
- Inserção de barras de erro associadas aos pontos que representam os dados experimentais;
  
- Inserção de bandas de predição e confiança nos gráficos;
  
- Opção de exportação da tabela obtida para os parâmetros estatísticos calculados no formato .xlsx;
  
- Opção de exportação dos gráficos produzidos para o formato .png.

## Avisos importantes antes da utilização do projeto
- Atente-se às opções oferecidas, aquelas que não estão explícitas não são aceitas ou reconhecidas. Por exemplo, se para o tipo de arquivo as opções são ".txt", ".xlsx" ou "não", escolha uma delas e garanta a grafia correta;
  
- Caso seu arquivo seja do tipo .txt ou .xlsx, garanta que ele está no mesmo diretório (pasta) que seu notebook. Verifique se o nome inserido está correto e não se esqueça de adicionar após ele o formato, por exemplo: meu_arquivo.txt ou meu_arquivo.xlsx;
  
- Para arquivos em .txt ou .xlsx, verifique e assegure que o nome selecionado para os dados referentes às abscissas e ordenadas coincide com aquele presente no arquivo;
  
- Caso deseje inserir seus dados manualmente, coloque-os no formato de lista, ou seja, entre colchetes (<b>[]</b>);
  
- Medidas inseridas manualmente cujos erros busca-se avaliar devem ser inseridas no formato de listas dentro de listas, ou seja, uma lista principal contendo sublistas com os valores para cada condição avaliada. Exemplo: [[1,2,3], [4,5,6]];
  
- Caso seus dados não apresentem múltiplas medidas para uma mesma condição, ou seja, não está estruturado como listas dentro de uma lista principal, a análise de incertezas não é possível de ser realizada. Ao ser questionado sobre quais dados devem ser considerados para a análise de erros, responda <b>"nenhuma"</b>;
  
- Certifique-se que, caso insira múltiplas medidas para uma mesma condição, a média delas seja diferente de zero. Caso isso não seja contemplado, erros serão produzidos ao tentar calcular as incertezas associadas a elas;

- Para quaisquer ajustes que desejar estimar e prever o gráfico, certifique-se de inserir ao menos 4 medidas para que esses possam ser gerados adequadamente. Lembre-se que, quantos mais pontos inserir, mais precisas serão as análises.

## Informações adicionais
- Exemplos de arquivos nos formatos .txt e .xlsx que podem ser utilizados para análise de incertezas ou não e cuja estrutura é aceita pelo projeto encontram-se na pasta "Exemplos de documentos para análises", estando devidamente identificados para o caso que atendem;

- Exemplos de tabelas e gráficos obtidos com as análises realizadas encontram-se na pasta "Exemplo de resultados", juntamente com sua identificação.

## Conclusão
Com base no desenvolvimento e utilização do projeto, verifica-se que ele cumpre ao objetivo que se propôs, integrando o recebimento, interpretação, análise e visualização dos dados experimentais recebidos. A automatização da geração de gráficos e cálculo de parâmetros estatísticos apresenta amplo potencial de minimizar erros associados a cálculos e estimativas manuais, além de reduzir o tempo empregado para esse processo. Em síntese, o desenvolvimento da atividade foi satisfatório e útil para verificar e consolidar todos os conceitos vistos na disciplina de Práticas em Ciência de Dados, além de culminar em um projeto útil a ser utilizado em outras disciplinas e análises experimentais futuras.

## Referências
Hoffmann, R., & Univeridade de São Paulo. Escola Superior de Agricultura Luiz de Queiroz. (2017). Análise de regressão: uma introdução à econometria. Univeridade de São Paulo. Escola Superior de Agricultura Luiz de Queiroz.

De, F. L. P. (s. d.). Modelo de regressão linear Teoria e aplicações. Ufpr.br. Acesso em 18 de junho de 2026, de http://leg.ufpr.br/~lucambio/Linear/Regressao.pdf

Dalson Figueiredo Filho, Felipe Nunes, Enivaldo Rocha, Manoel Santos, Mariana Batista, José Alexandre Junior. (2011). O que fazer e o que não fazer com a regressão: pressupostos e aplicações do modelo linear de mínimos quadrados ordinários (MQO) [Data set]. Harvard Dataverse.

Simple Widget Introduction — Jupyter Widgets 8.1.8 documentation. (s. d.). Readthedocs.Io. Acesso em 18 de junho de 2026, de https://ipywidgets.readthedocs.io/en/latest/examples/Widget%20Basics.html

Module: display — IPython 9.14.1 documentation. (s. d.). Readthedocs.Io. Acesso em 18 de junho de 2026, de https://ipython.readthedocs.io/en/stable/api/generated/IPython.display.html

W3schools.com. (s. d.). W3schools.com. Acesso em 18 de junho de 2026, de https://www.w3schools.com/python/numpy/numpy_intro.asp
