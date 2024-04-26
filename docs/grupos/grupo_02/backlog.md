<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);"ss />
</div>

<br/>

Neste documento, são delineados os passos envolvidos na elaboração do <i>Product Backlog</i>, destacando cada fase do processo e documentando os artefatos gerados ao longo do percurso.

## Histórico de versões

| Versão |    Data    |                    Descrição                    |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :---------------------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento do Backlog do Produto | [Grupo 02](/grupos/grupo_02?id=integrantes-do-grupo) |      -      |

## Introdução
O *Product Backlog*, ou *Backlog* do produto, é um conceito fundamental na metodologia ágil, especialmente no framework *Scrum*. Trata-se de uma lista dinâmica e priorizada de funcionalidades, melhorias e requisitos que compõem o produto a ser desenvolvido. Os itens no *Product Backlog* podem variar em termos de complexidade, esforço necessário para implementação e valor para o usuário final. Eles são frequentemente descritos em termos de histórias de usuário, que são pequenas narrativas centradas no usuário que descrevem uma funcionalidade desejada (Schwaber; Sutherland, 2017).

O <i>Backlog</i> do produto, deste projeto, foi construído combinando os requisitos, funcionais e não funcionais, coletados em cada etapa do processo de elaboração do *Lean Inception*. Os requisitos funcionais são aqueles que delineiam as necessidades, características e funcionalidades essenciais do produto de software, já os requisitos não funcionais focam nas qualidades e restrições que o produto deve cumprir, abrangendo aspectos como desempenho, segurança e usabilidade (Sommerville, 2011.). 

As histórias de usuários são agrupadas e organizadas de acordo com seus épicos correspondentes, proporcionando uma estrutura que visa simplificar a gestão de requisitos em uma escala mais abrangente (Cohn, 2004). Os épicos estabelecidos nesta fase são: "Autenticação e Autorização", "Gerenciamento de Instituições", "Gerenciamento de Especialidades", "Gerenciamento de Colaboradores" e "Gerenciamento de Agendamentos". Cada épico será explicado individualmente nas Seções a seguir.

E por fim, para calcular a pontuação de cada história, foi utilizada a sequência de Fibonacci. Este método reconhece a importância de atribuir valores que representem com precisão a complexidade relativa de cada tarefa. A sequência de Fibonacci, conhecida por seu crescimento exponencial, foi usada para criar um sistema que efetivamente abrange as variações de esforço e complexidade. As pontuações, que variam de 0 a 13, foram organizadas de maneira a facilitar a priorização de histórias, otimizar o uso de recursos e tornar o desenvolvimento o mais eficiente possível (Conh, 2005). 

### Épico 01 - Navegação Inicial
Permite ao usuário cadastrar-se, além de apresentar um guia geral sobre o uso da aplicação e a landing page. Também permite ao usuário realizar o login.

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                                          |
| ----- | ------------------------------------------------------------------------------------------------------------------------------ |
| RQF01 | A landing page deve permitir que os usuários criem uma nova conta. |
| RQF02 | O formulário de cadastro deve coletar e-mail, senha e confirmação de senha.|
| RQF03 | O sistema deve validar os dados de entrada do usuário durante o processo de cadastro.|
| RQF04 | O sistema deve oferecer a opção de visualizar a senha enquanto digitam para evitar erros de digitação.|
| RQF05 | Após o cadastro, o usuário deve receber um e-mail de confirmação para verificar sua conta.|
| RQF06 | A landing page deve permitir que os usuários entrem usando e-mail e senha.|
| RQF07 | O sistema deve oferecer a opção "Esqueceu a senha?" para recuperar a senha via e-mail.|
| RQF08 | Deve haver uma opção para manter o usuário conectado.|
| RQF09 | A landing page deve incluir um link ou seção para um guia de utilização que explique as principais funcionalidades do aplicativo.|
| RQF10 | O guia de utilização deve ser visual e interativo.|
| RQF11 | A página deve apresentar um design responsivo que se ajuste a dispositivos móveis e desktops.|
| RQF12 | Deve incluir uma seção "Sobre" que descreve o propósito e as principais características do aplicativo.|
| RQF13 | Deve conter links para as políticas de privacidade e termos de serviço.|

<p style="text-align: center;">Tabela 1: Requisitos Funcionais de Autenticação e Autorização.</p>

#### Requisitos Não Funcionais
| Item   | Requisito não funcional                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------ |
| RQNF01 | O tempo de carregamento da landing page não deve exceder 3 segundos. |
| RQNF02 | As respostas às ações de sign up e login devem ser processadas em menos de 2 segundos. |
| RQNF03 | Todos os dados do usuário, especialmente senhas e informações pessoais, devem ser criptografados. |
| RQNF04 | A landing page deve implementar HTTPS para garantir uma conexão segura. |
| RQNF05 | A interface do usuário deve ser intuitiva e fácil de navegar. |
| RQNF06 | Deve haver redundância no sistema para garantir a continuidade do serviço em caso de falha. |
| RQNF07 | O código deve ser bem documentado para facilitar futuras manutenções e atualizações. |

<p style="text-align: center;">Tabela 2: Requisitos Não Funcionais de Autenticação e Autorização.</p>

### Épico 02 - Gerenciamento de pacientes
Permite o usuário a excluir pacientes, listar pacientes, cadastrar dependentes, cadastrar um novo exame para o cliente e realizar o logout da aplicação

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                                            |
| ----- | ------------------------------------------------------------------------------------------------------------------------------     |
| RQF01 | O sistema deve permitir o cadastro de dependentes, coletando dados como nome, idade, relação e condições de saúde específicas.    |
| RQF02 | O sistema deve permitir a listagem de todos os dependentes cadastrados pelo usuário.                                                |
| RQF03 | O sistema deve oferecer a funcionalidade de exclusão de dependentes cadastrados.                                                    |
| RQF04 | O sistema deve permitir o cadastro de exames para um dependente específico, incluindo tipo de exame, data e resultados.             |
| RQF05 | O sistema deve permitir que o usuário realize logout da aplicação.                                                                  |
| RQF06 | O sistema deve permitir que o usuário atualize as informações de um dependente cadastrado.                                          |
| RQF07 | O sistema deve fornecer uma funcionalidade de pesquisa para localizar rapidamente informações sobre um dependente específico.      |
| RQF08 | O sistema deve enviar notificações via email ou SMS para lembretes de exames agendados.                                             |
| RQF09 | O sistema deve permitir o upload de documentos médicos associados a um dependente, como resultados de exames em formato PDF.       |
| RQF10 | O sistema deve oferecer a opção de visualizar um histórico detalhado de todos os exames realizados por cada dependente.             |
| RQF11 | O sistema deve permitir a exportação de relatórios médicos de dependentes em formatos como PDF ou Excel.                            |
| RQF12 | O sistema deve permitir a configuração de permissões de acesso para diferentes níveis de usuários (por exemplo, admin, usuário).    |
| RQF13 | O sistema deve oferecer suporte para múltiplos idiomas na interface do usuário.                                                     |



### Requisitos Não Funcionais
| Item   | Requisito não funcional                                                                                                         |
| ------ | -----------------------------------------------------------------------------------------------------------------------------    |
| RQNF01 | O sistema deve garantir a segurança dos dados pessoais e médicos dos dependentes, utilizando criptografia para armazenamento.    |
| RQNF02 | O sistema deve ser acessível via HTTPS para garantir uma conexão segura.                                                         |
| RQNF03 | A interface do usuário deve ser intuitiva e adaptada para facilitar o gerenciamento dos dependentes e exames.                    |
| RQNF04 | O sistema deve ser capaz de suportar um alto volume de usuários e operações simultâneas sem perda de performance.                 |
| RQNF05 | O sistema deve garantir alta disponibilidade e redundância para evitar interrupções no serviço.                                  |
| RQNF06 | O tempo de resposta para as operações de cadastro, listagem e exclusão de dependentes não deve exceder 2 segundos.                |
| RQNF07 | As atualizações do sistema devem ser possíveis sem tempo de inatividade significativo ou impacto no usuário final.                |
| RQNF08 | O sistema deve ser projetado para ser compatível com os principais navegadores e versões de dispositivos móveis.                   |
| RQNF09 | O sistema deve implementar logs de auditoria detalhados para monitorar e registrar todas as ações críticas realizadas pelos usuários.|
| RQNF10 | O sistema deve garantir a privacidade dos dados do usuário, cumprindo com regulamentações como GDPR ou HIPAA, conforme aplicável.   |
| RQNF11 | O sistema deve oferecer um tempo de recuperação após desastre (RTO) de no máximo 4 horas e um ponto de recuperação (RPO) de 1 hora.  |
| RQNF12 | O sistema deve fornecer uma API para integração com outros sistemas de saúde eletrônicos e plataformas de dados.                   |
| RQNF13 | O sistema deve ter uma capacidade de escalabilidade horizontal para lidar com o aumento de carga durante picos de uso.             |
| RQNF14 | O sistema deve ter uma interface responsiva, com um tempo de carregamento de tela não superior a 3 segundos.                        |
| RQNF15 | O sistema deve fornecer suporte técnico 24/7 para usuários e manutenção do sistema.                                                 |



<p style="text-align: center;">Tabela 3: Requisitos Funcionais de Gerenciamento de instituições.</p>


## Referências
 
 * COHN, M. Agile Estimating and Planning. Prentice Hall, 2005.
 * COHN, M. User Stories Applied. Addison-Wesley Professional, 2004.
 * SOMMERVILLE, I. Software Engineering. 9ª. ed. Pearson Education India, 2011.
