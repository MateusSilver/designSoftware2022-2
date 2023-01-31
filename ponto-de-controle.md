## Análise Artigo Design de Software
_baseado em [Projetando um sistema de software complexo](https://betterprogramming.pub/designing-a-complex-software-system-720897671b6a)_

### Os fundamentos do design de software
#### Visão
O projeto GCC tem como finalidade criar um software que traga segurança, facilidade de uso para documentar as consultas e exames feitos em um hospital e que tenha facilidade de integração com o RNDS, plataforma nacional de integração de dados em saúde.
#### Limite
O software é limitado a:
* Preenchimento dos dados do paciente
* Preenchimento da consulta feita ao paciente
* Preenchimento do resultado do exame feito no paciente
* Envio e busca dos dados do paciente no RNDS
#### Contrato
1. Contratos de usuário: O usuário irá interagir com o sistema pela web
2. Contratos de Integração: a integração será feita pela web utilizando serviços de API pois possibilita a comunicação do software com outros sistemas e dever ter alto nível de segurança dado o tráfego de dados sensíveis
3. Contratos de API: será usado o swagger para documentação da api descrevendo os endpoints e parâmetros da aplicação
4. Contratos de Dados: o modelo de dados será orientado a objetos que são armazenados no banco relacional com restrições de formatação condizentes com as especificações do RNDS 
5. Contratos de equipe: os arquivos são organizados no padrão de arquitetura MVC e seguindo os padrões de design pattern

### Limites do Design de Software
O design do projeto foi limitado ao detalhamento dos containers principais do sistema sendo eles a api, o banco de dados e o worker pois foram definidos como prioridades por terem alta complexidade, sendo o detalhamento feito no padrão C4 model com modelagem dos diagramas necessários para documentar as decisões do projeto.

### Processo de Design
__Abordagem Top-Down__ realizada para o software em questão definindo estrutura básica de comunicação entre cada parte do sistema do GCC para realizar seus propósitos e após identificar necessidades adicionais de desmembramento em outros elementos.
### Ferramentas de design
#### Geral
Estas são as ferramentas de design que foram utilizadas para modelar o design do projeto:
* [Visual Paradigm - C4 Model](https://online.visual-paradigm.com/pt/diagrams/features/c4-model-tool/)
* [Diagram.net (draw.io)](diagram.net)
#### Visual
Não foi realizada ainda uma implementação do escopo geral do escopo do sistema e seu funcionamento fora o que é descrito no README deste repositório.
#### Interface do usuário - __Mockups__
Não foi realizada ainda uma implementação de telas visuais e páginas do sistema.
#### Interface do usuário - __Protótipos__
Não destinamos tempo para o desenvolvimento de protótipos pois causaria atrasos ao projeto.
#### Diagramas de negócios
Ainda não foram implementados diagramas de negócio no projeto.
#### Schemas
Schemas serão formatados de acordo com os dados e especificações recebidos da Rede Nacional de Dados da Saúde (RNDS).
#### Topologias
As topologias utilizadas para a compreensão da infraestrutura necessária para o funcionamento do sistema GCC foram o [Diagrama de Componentes](https://github.com/MateusSilver/designSoftware2022-2/blob/main/documentacao/componente.md) e o [Diagrama de Contêineres](https://github.com/MateusSilver/designSoftware2022-2/blob/main/documentacao/container.md).


