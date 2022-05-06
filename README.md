Validation of tabular (CSV) data against a schema defined in YAML or JSON. See the schema.yml file in this repository for an example and instructions on creating a schema. It is possible to designate up to six main "rules":

  1. required columns (i.e. columns that must exist for all rows)
  2. allowed columns (i.e. *only* the specified columns can exist -- for strict control of data)
  3. populated columns (i.e. these columns must contain a non-null value)
  4. controlled values (specify a set of possible values as a list in the form: {'colname' : ['val1','val2','val3']}
  5. numeric data (cells in these columns may only contain digits)
  6. date data (values in these columns must be parsable as ISO-8601 dates)

VALIDAÇÃO DE ARQUIVOS CSV

Este conjunto de códigos, será capaz de reconhecer dentro de um arquivo CSV incongruências com um padrão pré-amostrado. 

VISÃO GERAL DO PROJETO
- Passo 1: desenvolvimento de estrutura de um projeto que comporte ferramentas capazes de identificar incongruência de entradas CSV.
- Passo 2: formulação da correlação de tratamento de arquivos CSV com uma base de dados pré-defida.
- Passo 3: compilação de ferramentas visualizadoras e de performance, instituir dentro de uma plataforma de visualização de resposta a cada entrada CSV, a ideia é ter uma interface programática de fácil acesso, com funcionalidade simples.
- Passo 4: definição das funcionalidades da ferramenta final, desde a aquisição de backup do dado inserido pelo cliente na entrada CSV até a resposta em tela, se o documento está ou não cumprindo os parâmetros solicitados pela normativa dos formatos CSV padrões da telemetria
- Passo 5: relação das entradas de arquivos tabulares, com a funcionalidade de sensores de aquisição de telemetria. Entender dentro da relação cliente aquisição de dados quais são as possíveis lacunas e desafios em manter uma estrutura padronizada na inserção de dados. 
- Passo 6: interface de acesso e aquisição automatizada. Após a padronização da aquisição de arquivos em formato CSV e a definição dos parâmetros oficiais, é preciso entender como a interface de acesso pode ser utilizada pelo cliente. 
- Passo 7: aquisição automática e software de alimentação de banco de dados, levando em conta que o software de validação de dados vai abranger uma gama de funcionalidades desde backup de informação até analise e informativo de erro e incongruências, poderemos relacionar dentro dessa funcionalidade algum tipo de ferramenta automática de aquisição de dados. 
- Passo 8: com uma API de integração de dados, poderemos ativar funcionalidades de aquisição automática entre sensores, levando em conta aquisição de dados por CLP e leitura de código fonte.
 
  

O titulares ou seus RT's devem verificar e corrigir eventuais erros de formatação, antes de enviarem os dados à ANM acompanhados do respectivo extrato de aprovação via plataforma SEI.    
Ferramenta faz a varredura dos dados, apontando eventuais erros de preenchimento quantas vezes forem necessárias à correta formatação do dado; 

Caso aprovado o dado, a ferramenta deve gerar o extrato de aprovação para impressão, contendo rash do arquivo analisado (saída), e deve alimentar uma base de dados (em ambiente seguro) com o conteúdo do dado aprovado;   
Ferramenta web para validação automática dos dados, conforme regras previstas na resolução 

Login e senha para acesso e uso da ferramenta deve ser os mesmos usados para acesso no sistema SEI 

Identificadores a serem exigidos para carga dos dados: 

CNPJ do titular 

Número do processo minerário 

Nome da Fonte
