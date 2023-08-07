## Modelo de Banco de Dados - Sistema de Ordem de Serviço de uma Oficina Mecânica

Este é modelo que representa um sistema de ordem de serviço de uma oficina mecânica.

#### Tabelas

O modelo inclui as seguintes tabelas:

- `Cliente`: tabela que armazena informações sobre os clientes, como ID, nome, CPF, contato e endereço.
- `Veículo`: tabela que armazena informações sobre os veículos, como ID, tipo, modelo, marca, número da placa e ID do cliente associado.
- `Equipe_de_Mecânicos`: tabela que armazena informações sobre as equipes de mecânicos, como ID e nome.
- `Mecânico`: tabela que armazena informações sobre os mecânicos, como ID, código, nome, endereço, especialidade e ID da equipe de mecânicos associada.
- `Serviço`: tabela que armazena informações sobre os serviços, como ID, descrição, valor das peças e ID da equipe de mecânicos associada.
- `Ordem_de_Serviço`: tabela que armazena informações sobre as ordens de serviço, como ID, data de emissão, status, data de conclusão, ID do veículo associado, ID do serviço associado e ID da equipe de mecânicos associada.
- `Peça`: tabela que armazena informações sobre as peças, como ID, nome, descrição e valor.
- `Serviço_usa_Peça`: tabela de relacionamento entre os serviços e as peças que são utilizadas nos mesmos. Armazena o ID do serviço, o ID da peça e a quantidade utilizada.

#### Configurações

O modelo foi gerado usando o MySQL Workbench. 

#### Como usar

Você pode utilizar esse modelo de banco de dados como ponto de partida para o desenvolvimento do sistema de ordem de serviço da sua oficina mecânica. Basta abrir o projeto no MySQL Workbench gerar o script e executar o script SQL em um servidor MySQL e adaptar as queries.
