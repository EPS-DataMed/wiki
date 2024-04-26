<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);"ss />
</div>

<br/>

Neste documento, são delineados os passos envolvidos na elaboração do <i>Product Backlog</i>, destacando cada fase do processo e documentando os artefatos gerados ao longo do percurso.

## Histórico de versões

| Versão |    Data    |                    Descrição                    |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :---------------------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 17/04/2024 | Criando documento do Backlog | Grupo 03 |      -      |

## Introdução
O *Product Backlog*, ou *Backlog* do produto, é um conceito fundamental na metodologia ágil, especialmente no framework *Scrum*. Trata-se de uma lista dinâmica e priorizada de funcionalidades, melhorias e requisitos que compõem o produto a ser desenvolvido. Os itens no *Product Backlog* podem variar em termos de complexidade, esforço necessário para implementação e valor para o usuário final. Eles são frequentemente descritos em termos de histórias de usuário, que são pequenas narrativas centradas no usuário que descrevem uma funcionalidade desejada (Schwaber; Sutherland, 2017).

O <i>Backlog</i> do produto, deste projeto, foi construído combinando os requisitos, funcionais e não funcionais, coletados em cada etapa do processo de elaboração do *Lean Inception*. Os requisitos funcionais são aqueles que delineiam as necessidades, características e funcionalidades essenciais do produto de software, já os requisitos não funcionais focam nas qualidades e restrições que o produto deve cumprir, abrangendo aspectos como desempenho, segurança e usabilidade (Sommerville, 2011.). 

As histórias de usuários são agrupadas e organizadas de acordo com seus épicos correspondentes, proporcionando uma estrutura que visa simplificar a gestão de requisitos em uma escala mais abrangente (Cohn, 2004). Os épicos estabelecidos nesta fase são: "Autenticação e Autorização", "Gerenciamento de Instituições", "Gerenciamento de Especialidades", "Gerenciamento de Colaboradores" e "Gerenciamento de Agendamentos". Cada épico será explicado individualmente nas Seções a seguir.

E por fim, para calcular a pontuação de cada história, foi utilizada a sequência de Fibonacci. Este método reconhece a importância de atribuir valores que representem com precisão a complexidade relativa de cada tarefa. A sequência de Fibonacci, conhecida por seu crescimento exponencial, foi usada para criar um sistema que efetivamente abrange as variações de esforço e complexidade. As pontuações, que variam de 0 a 13, foram organizadas de maneira a facilitar a priorização de histórias, otimizar o uso de recursos e tornar o desenvolvimento o mais eficiente possível (Conh, 2005). 

### Épico 01 - Autenticação e Autorização
Permite ao usuário cadastrar e gerenciar dados básicos de acesso a sua conta, além disso também tem como foco a segurança da informação, utilizando de criptografia e permitindo formas de redefinição de senha.

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                                          |
| ----- | ------------------------------------------------------------------------------------------------------------------------------ |
| RQF01 | Quero entrar com minha credencial de usuário e senha para acessar o sistema de forma segura para que eu possa geranciar as informações sem riscos de acessos não autorizados. |
| RQF02 | Quero poder redefinir minha senha usando meu e-mail para que eu possa recuperar o acesso ao sistema se eu esquecer minha senha.|

<p style="text-align: center;">Tabela 1: Requisitos Funcionais de Autenticação e Autorização.</p>

#### Requisitos Não Funcionais
| Item   | Requisito não funcional                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------ |
| RQNF01 | Como administrador, quero que minha senha seja criptografada para que não possa ser facilmente acessada ou descriptografada por terceiros. |

<p style="text-align: center;">Tabela 2: Requisitos Não Funcionais de Autenticação e Autorização.</p>

### Épico 02 - Gerenciamento de instituições
Permite ao usuário fazer o cadastro e gerência de instituições, possibilitando adição de especialidades e gestão completa dos dados para que estejam constantemente atualizados.

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                                                                                            |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RQF03 | Quero cadastrar novas instituições fornecendo nome, tipo, endereço e contato para expandir a rede de atendimento disponível no sistema.                                          |
| RQF04 | Quero adicionar especialidades disponíveis em cada instituição durante o cadastro para que os pacientes possam escolher corretamente onde querem ser atendidos                   |
| RQF05 | Quero atualizar ou remover instituições já cadastradas para garantir que a informação no sistema esteja sempre atualizada e correta                                              |
| RQF06 | Quero visualizar todas as informações de uma instituição, incluindo detalhes como especialidades oferecidas e médicos disponíveis, para gerenciar eficientemente as instituições.|

<p style="text-align: center;">Tabela 3: Requisitos Funcionais de Gerenciamento de instituições.</p>

### Épico 03 - Gerenciamento de Especialidades
Permite ao usuário cadastrar novas especialidades na lista de serviços ofertados e fazer o gerenciamento dessas especialidades.

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                             |
| ----- | ----------------------------------------------------------------------------------------------------------------- |
| RQF07 | Quero adicionar novas especialidades ao sistema para manter a lista de serviços oferecidos atualizada.    |
| RQF08 | Quero editar os detalhes das especialidades para corrigir erros ou atualizar informações.                 |
| RQF09 | Quero remover especialidades que não são mais oferecidas para evitar confusões no agendamento de consultas .      |

<p style="text-align: center;">Tabela 4: Requisitos Funcionais de Gerenciamento de Especialidades.</p>

### Épico 04 - Gerenciamento de Colaboradores
Permite ao usuário cadastrar colaboradores na lista de serviços ofertados e fazer o gerenciamento dessas especialidades.

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                             |
| ----- | ----------------------------------------------------------------------------------------------------------------- |
| RQF10 | Quero cadastrar colaboradores no sistema, incluindo informações como nome, CPF e e-mail, para que eles possam ser associados a consultas e especialidades.|
| RQF11 | Quero associar colaboradores às instituições em que trabalham para que os pacientes possam agendar consultas corretamente.|
| RQF12 | Quero atualizar as informações dos colaboradores ou remover colaboradores do sistema quando necessário|

<p style="text-align: center;">Tabela 5: Requisitos Funcionais de Gerenciamento de Colaboradores.</p>

### Épico 05 - Gerenciamento de Agendamentos
Permite ao usuário gerenciar seus agendamentos, desde o agendamento até a edição em casos onde seja necessário.

#### Requisitos Funcionais
| Item  | Requisitos Funcionais                                                                                             |
| ----- | ----------------------------------------------------------------------------------------------------------------- |
| RQF13 | Quero ter a opção de realizar um agendamento diretamente pelo sistema, facilitando a gestão do meu tempo e evitando deslocamentos desnecessários.|
| RQF14 | Quero ter a opção de cancelar ou fazer um reagendamento diretamente pelo sistema, facilitando a gestão do meu tempo e evitando deslocamentos desnecessários.|
| RQF15 | Quero poder modificar os detalhes de um agendamento em caso de necessidade, como alterações no horário ou no médico designado, para acomodar.|
| RQF16 | Quero poder confirmar ou recusar pedidos de reagendamento ou cancelamento para manter a ordem e eficiência dos agendamentos|
| RQF17 | Quero visualizar todas as minhas consultas agendadas, incluindo datas, horários, colaboradores e instituições, para que eu possa gerenciar meu tempo e compromissos de saúde eficientemente.|

<p style="text-align: center;">Tabela 6: Requisitos Funcionais de Gerenciamento de Agendamentos.</p>

## Referências
 
 * COHN, M. Agile Estimating and Planning. Prentice Hall, 2005.
 * COHN, M. User Stories Applied. Addison-Wesley Professional, 2004.
 * SOMMERVILLE, I. Software Engineering. 9ª. ed. Pearson Education India, 2011.
