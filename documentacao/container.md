## Diagrama de contêineres

O diagrama a seguir, ilustra os contêineres da aplicação.


![](diagramas/c4_container.png)

As interfaces de usuário, sejam elas destinadas aos Pacientes, Médicos, ou Secretárias, necessitam buscar e retornar informações. 

Para tanto, a interface se comunica com a API, fazendo as requisições. A API por sua vez, busca essas informações no Banco de dados (Database).

O Banco de dados pode ser alimentado pelo RNDS (Rede Nacional de Dados em Saúde), e por se tratar de dados sensíveis, existe um Worker que controla esse fluxo.
