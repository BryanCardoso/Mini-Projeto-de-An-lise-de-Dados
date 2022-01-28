# Mini Projeto de Análise de Dados

Vamos fazer um exercício completo de pandas para um miniprojeto de análise de dados.

### O que temos?

Temos os dados de 2019 de uma empresa de prestação de serviços. 

- CadastroFuncionarios
- CadastroClientes
- BaseServiçosPrestados

Obs1: Para ler arquivos csv, temos o read_csv<br>
Obs2: Para ler arquivos xlsx (arquivos em excel normais, que não são padrão csv), temos o read_excel

### O que queremos saber/fazer?

1. Valor Total da Folha Salarial -> Qual foi o gasto total com salários de funcionários pela empresa? <br>
    Sugestão: calcule o salário total de cada funcionário, salário + benefícios + impostos, depois some todos os salários
    
    
2. Qual foi o faturamento da empresa?<br>
    Sugestão: calcule o faturamento total de cada serviço e depois some o faturamento de todos
    
    
3. Qual o % de funcionários que já fechou algum contrato?<br>
    Sugestão: na base de serviços temos o funcionário que fechou cada serviço. Mas nem todos os funcionários que a empresa tem já fecharam algum serviço.<br>
    . Na base de funcionários temos uma lista com todos os funcionários<br>
    . Queremos calcular Qtde_Funcionarios_Fecharam_Serviço / Qtde_Funcionários_Totais<br>
    . Para calcular a qtde de funcionários que fecharam algum serviço, use a base de serviços e conte quantos funcionários tem ali. Mas lembre-se, cada funcionário só pode ser contado uma única vez.<br><br>
    Dica: se você aplicar o método .unique() em uma variável que é apenas 1 coluna de um dataframe, ele vai excluir todos os valores duplicados daquela coluna.<br>
    Ex: unicos_colunaA = dataframe['colunaA'].unique() te dá como resposta uma lista com todos os itens da colunaA aparecendo uma única vez. Todos os valores repetidos da colunaA são excluidos da variável unicos_colunaA 
    
    
4. Calcule o total de contratos que cada área da empresa já fechou


5. Calcule o total de funcionários por área


6. Qual o ticket médio mensal (faturamento médio mensal) dos contratos?<br>
    Dica: .mean() calcula a média -> exemplo: media_colunaA = dataframe['colunaA'].mean()

Obs: Lembrando as opções mais usuais de encoding:<br>
encoding='latin1', encoding='ISO-8859-1', encoding='utf-8' ou então encoding='cp1252'

Observação Importante: Se o seu código der um erro na hora de importar os arquivos:<br>
- CadastroClientes.csv
- CadastroFuncionarios.csv

Use separador ";" (ponto e vírgula) para resolver

## English version
Let's do a full panda exercise for a mini-data analysis project.

### What have we got?
We have 2019 data from a service provider.

- CadastroFuncionarios
- CadastroClientes
- BaseServiçosPrestados

Note1: To read csv files, we have the read_csv
Obs2: To read xlsx files (normal excel files, which are not csv standard), we have the read_excel

### What do we want to know/do?

1. Total Salary Amount -> was the total expenditure on employee salaries by the company?
    Tip: Calculate each employee's total salary, salary + benefits + taxes, then add up all salaries


2. What was the company's revenue?
    Tip: Calculate the total billing for each service and then add up the billing for all
    
    
3. What is the % of employees who have already signed a contract?
     Tip: On the service basis we have the employee who closed each service. But not all employees that the company has have already closed some service.
       . At the employee base we have a list of all employees
       . We want to calculate Qtde_Funcionarios_Fecharam_Serviço / Qtde_Funcionários_Totais
       . To calculate the number of employees who closed a service, use the service base and count how many employees there are. But remember, each employee can only be counted once.
       Tip: if you apply the .unique() method on a variable that is only 1 column of a dataframe, it will delete all duplicate values from that column. 
       Ex: unicos_colunaA = dataframe['colunaA'].unique() gives you as a response a list with all items in columnA appearing only once. All repeated values of columnA are excluded from the unicos_columnA variable
       
       
4. Calculate the total number of contracts that each area of the company has already closed


5. Calculate total employees per area



6. What is the average monthly ticket (average monthly revenue) of the contracts?
    Hint: .mean() calculates the average -> example: average_columnA = dataframe['columnA'].mean()

Note: Remembering the most common encoding options:
encoding='latin1', encoding='ISO-8859-1', encoding='utf-8' or else encoding='cp1252'

Important Note: If your code has an error when importing files:
- CadastroFuncionarios
- CadastroClientes
- BaseServiçosPrestados
Use separator ";" (semicolon) to resolve
