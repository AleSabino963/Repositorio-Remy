### UML da Lista de Insumos. 
```mermaid
sequenceDiagram
 actor U as Usuário
 participant A as FrontEnd
 participant B as BackEnd
 participant D as Banco de dados

U->>A:Aperta o botão "Insumos"
A->>B:Solicita a lista de Insumos
B->>D:Consulta os insumos cadastrados
D-->>B:Retorna uma lista com insumos cadastrados
Note over B:Organiza a lista em ordem alfabética.
B-->>A:Retorna a lista de insumos de forma organizada
A-->>U:Exibe a lista de insumos em ordem alfabética
