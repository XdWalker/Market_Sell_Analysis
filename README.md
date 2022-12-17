# Market_Sell_Analysis

# Análise das vendas de um supermercado turco. (PT-BR)

### Analista de dados:
- Walker Teotônio Correia de Barros

### Queremos responder as perguntas a seguir
 -  Qual o produto mais vendido pelo supermercado?
 -  São os homens ou as mulheres que mais compram no supermercado?
 -  Existe algum período onde o supermercado mais vende?

### Dados utilizados:

#### Kaggle.com
https://www.kaggle.com/datasets/omercolakoglu/turkish-market-sales-dataset-with-9000items/discussion

#### Pré-processamento

##### Estruturação

###### Nomeação e tradução de colunas
Para um melhor entendimento e otimização do desenvolvimento do projeto, foi necessário a tradução e nomeação de algumas colunas e linhas do dataset como as colunas AMOUNT, BRANCHNR, DATE_, BRANCH, SALESMAN, BRANDCODE, e BRAND que foram traduzidas ou renomeadas para QUANTIDADE, FILIALNR, DATE, FILIAL, VENDEDOR, MARCA_CODE e MARCA respectivamente.

###### Correção dos tipos de dados
Em seguida foi necessário setar a coluna CLIENTCODE para o tipo string, pois a mesma possuia valores mistos tornando a leitura do arquivo lenta, já que são 600 mil linhas de dados e tratar os dados das colunas de datas para o tipo date para manipular as mesmas, pois por algum motivo desconhecido
as datas de STARTDATE e ENDDATE estão adiantadas por um dia comparado a coluna DATE, então eu subtraio menos um dia de todas as datas de ENDDATE e STARTDATE e depois eu exporto a correção para um novo arquivo .csv.

Por fim eu traduzo algumas linhas das colunas CATEGORY_NAME1, CATEGORY_NAME2 e CATEGORY_NAME3 para o melhor entendimento do dataset, pois são nomes turcos, produtos turcos ou categorias de produtos turcos o que pode e causa uma certa demora no entendimento desses dados, já que não é uma língua que compreendo e também adciono uma observação sobre os generos da coluna GENDER do dataset, pois E - são homens e K - são mulheres.

#### Remoção de Dados Ruídosos 
Felizmente não foi necessário remover dados incorretos no dataset, pois ele foi bem coletado e os dados que faltam ou que são NAN não irão atrapalhar ou complicar a análise, pois esses dados se encontram em colunas que não são tão utéis.

#### Análise de Colunas
Colunas com grandes números de erros nos registros e que não eram relevantes para a amostra, foram removidas. Essas colunas foram identificadas com base na análise da medidas de tedência central das mesmas

#### Conclusões

##### Resultados

##### Limitações 

##### Trabalhos futuros

##### Melhorias
