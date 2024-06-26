<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);"ss />
</div>

<br/>

Neste documento, são delineados os passos envolvidos na elaboração do <i>Product Backlog</i>, destacando cada fase do processo e documentando os artefatos gerados ao longo do percurso.

## Histórico de versões

| Versão |    Data    |                    Descrição                    |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :---------------------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento do Backlog do Produto | [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo) |      -      |
| `1.1`  | 19/04/2024 | Ajustando épico | [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo) |      -      |

## Introdução
O *Product Backlog*, ou *Backlog* do produto, é um conceito fundamental na metodologia ágil, especialmente no framework *Scrum*. Trata-se de uma lista dinâmica e priorizada de funcionalidades, melhorias e requisitos que compõem o produto a ser desenvolvido. Os itens no *Product Backlog* podem variar em termos de complexidade, esforço necessário para implementação e valor para o usuário final. Eles são frequentemente descritos em termos de histórias de usuário, que são pequenas narrativas centradas no usuário que descrevem uma funcionalidade desejada (Schwaber; Sutherland, 2017).

O <i>Backlog</i> do produto, deste projeto, foi construído combinando os requisitos, funcionais e não funcionais, coletados em cada etapa do processo de elaboração do *Lean Inception*. Os requisitos funcionais são aqueles que delineiam as necessidades, características e funcionalidades essenciais do produto de software, já os requisitos não funcionais focam nas qualidades e restrições que o produto deve cumprir, abrangendo aspectos como desempenho, segurança e usabilidade (Sommerville, 2011.). 

As histórias de usuários são agrupadas e organizadas de acordo com seus épicos correspondentes, proporcionando uma estrutura que visa simplificar a gestão de requisitos em uma escala mais abrangente (Cohn, 2004). Os épicos estabelecidos nesta fase são: "Navegação Inicial", "Gerência de Pacientes", "Formulário", "Resultados" e "Comercialização". Cada épico será explicado individualmente nas Seções a seguir.

E por fim, para calcular a pontuação de cada história, foi utilizada a sequência de Fibonacci. Este método reconhece a importância de atribuir valores que representem com precisão a complexidade relativa de cada tarefa. A sequência de Fibonacci, conhecida por seu crescimento exponencial, foi usada para criar um sistema que efetivamente abrange as variações de esforço e complexidade. As pontuações, que variam de 0 a 13, foram organizadas de maneira a facilitar a priorização de histórias, otimizar o uso de recursos e tornar o desenvolvimento o mais eficiente possível (Conh, 2005). 

## Requisitos não funcionais
Neste tópico, são apresentados os requisitos não funcionais, os quais foram organizados em 5 categorias distintas: usabilidade, portabilidade, confiabilidade, eficiência e segurança. Os detalhes específicos de cada categoria serão abordados a seguir.

### Usabilidade
Neste tópico são apresentados requisitos não funcionais relacionados à usabilidade da interface de autenticação. A ênfase está na criação de uma experiência do usuário intuitiva, em conformidade com as diretrizes de design. A Tabela 1 fornece detalhes sobre os requisitos não funcionais específicos para usabilidade.

| Item   | Requisito não funcional                                                                                                        |
| ------ | ------------------------------------------------------------------------------------------------------------------------------ |
| RQNF01 | A interface de autenticação deve ser projetada de forma intuitiva, seguindo as diretrizes de design de experiência do usuário. |
| RQNF02 | Os avisos sobre o uso de *cookies* devem ser apresentados de forma clara e fácil de entender para os usuários.                 |

<p style="text-align: center;">Tabela 1: Requisitos Não Funcionais de Usabilidade.</p>

### Portabilidade
Este tópico aborda um requisito não funcional de portabilidade do sistema. O objetivo é garantir que o sistema seja acessível de maneira consistente em uma variedade de navegadores populares. Consulte a Tabela 2 para obter detalhes sobre o requisito relacionado à portabilidade.

| Item   | Requisito não funcional                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------ |
| RQNF03 | O sistema de autenticação deve ser compatível com os principais navegadores da web, como Chrome, Firefox, Safari e Edge. |

<p style="text-align: center;">Tabela 2: Requisito Não Funcional de Portabilidade.</p>

### Confiabilidade
Nesta seção, é apresentado um requisito não funcional relacionado à confiabilidade. É crucial que os cookies mantenham uma vida útil adequada e não expirem prematuramente, a menos que o usuário escolha sair ou retirar seu consentimento. A Tabela 3 apresenta uma visão geral do requisito não funcional que garante a confiabilidade.

| Item   | Requisito não funcional                                                                                                                           |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| RQNF04 | Os *cookies* devem ter uma vida útil adequada e não expirar de forma prematura, a menos que o usuário opte por sair ou revogar seu consentimento. |

<p style="text-align: center;">Tabela 3: Requisito Não Funcional de Confiabilidade.</p>


### Eficiência
Aqui, é explorado um requisito não funcional relacionado à eficiência do sistema. Isso implica que o sistema deve ser capaz de fornecer respostas em tempo real de maneira ágil e eficaz. Detalhes específicos sobre o requisito de eficiência podem ser encontrados na Tabela 4.

| Item   | Requisito não funcional                                         |
| ------ | --------------------------------------------------------------- |
| RQNF05 | O sistema deve ser capaz de apresentar respostas em tempo real. |

<p style="text-align: center;">Tabela 4: Requisito Não Funcional de Eficiência.</p>

### Segurança
Nesta seção, são discutidos os requisitos não funcionais relacionados à segurança abrangente do sistema. Isso envolve a proteção da confidencialidade dos dados do usuário, a garantia da segurança geral dos dados e a preservação da integridade dos dados. Para obter informações mais detalhadas, consulte a Tabela 5.

| Item   | Requisito não funcional                                            |
| ------ | ------------------------------------------------------------------ |
| RQNF06 | O sistema deve preservar a confidencialidade dos dados do usuário. |
| RQNF07 | O sistema deve assegurar a segurança dos dados.                    |
| RQNF08 | O sistema deve proteger a integridade dos dados.                   |

<p style="text-align: center;">Tabela 5: Requisitos Não Funcionais de Segurança.</p>

### Épicos

Épicos no backlog do produto representam grandes iniciativas ou metas de alto nível que são desmembradas em tarefas menores. Eles são usados para agrupar um conjunto de funcionalidades ou requisitos que, juntos, contribuem significativamente para o desenvolvimento de um produto. Esses épicos são uma ferramenta fundamental para gerenciar projetos complexos e manter o foco nas metas estratégicas. À medida que a equipe avança, os épicos são decompostos em histórias de usuário mais detalhadas e viáveis.

#### Autenticação
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero fazer sign up                          | Must       |
| Eu como usuário quero fazer log in                           | Must       |
| Eu como usuário quero recuperar minha senha                  | Must       |

#### Termos de Uso
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero gerar um PDF com termos de uso         | Should     |
| Eu como usuário quero me descadastrar dos termos             | Should     |

#### Usuário
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero editar meu perfil                      | Must       |
| Eu como administrador quero listar informações de usuários   | Must       |
| Eu como administrador quero atribuir dependentes a um usuário| Should     |
| Eu como usuário quero confirmar dependência                  | Should     |
| Eu como administrador quero excluir um dependente            | Should     |

#### Processamento de Exames
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero enviar exames médicos para processamento| Must      |
| Eu como usuário quero extrair corretamente dados de saúde    | Must       |
| Eu como administrador quero criar formulários                | Should     |
| Eu como administrador quero editar formulários               | Should     |
| Eu como usuário quero listar formulários                     | Should     |

#### Gerenciador de Arquivos
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero submeter arquivos e salvar no repositório | Must    |
| Eu como usuário quero excluir arquivos                       | Must       |
| Eu como usuário quero mostrar todos os arquivos              | Must       |

#### Extração de PDF
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero submeter um PDF                        | Must       |
| Eu como usuário quero extrair informações do PDF por parâmetros | Should  |

#### Compartilhamento de Dados de Saúde
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como administrador quero visualizar logs de dados compartilhados | Should |
| Eu como administrador quero ferramentas de busca e filtragem de dados | Could |
| Eu como administrador quero notificações sobre novos compartilhamentos | Could |
| Eu como profissional quero mecanismos para feedback de dados | Could      |
| Eu como administrador quero opções para correção de dados    | Should     |
| Eu como administrador quero backup e recuperação de dados    | Must       |
| Eu como administrador quero histórico de versões de dados    | Could      |

#### Comercialização
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como administrador quero anonimização de dados            | Should     |
| Eu como administrador quero dashboard para gerenciar transações | Should  |
| Eu como administrador quero implementar medidas de segurança | Should     |
| Eu como administrador quero backup regular                   | Must       |

#### Cartão de Vacina
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero submeter cartão de vacina              | Must       |
| Eu como usuário quero alertar sobre vacinas que venceram     | Must       |
| Eu como administrador quero informar novas vacinas           | Could      |

#### Navegação Inicial
| User Story (História de Usuário)                              | MoSCoW |
|--------------------------------------------------------------|-----------------|
| Eu como usuário quero explicação sobre a aplicação           | Must       |
| Eu como usuário quero colocar demonstração de software       | Should     |
| Eu como usuário quero colocar contato na landing page        | Should     |


| Legenda MoSCoW | Descrição |
|:--------------:|:---------:|
| Must | Tarefas indispensáveis para a realização do projeto (Tenho que fazer) |
| Should | Tarefas importantes para a realização do projeto, mas não é fundamental (Deveria fazer) |
| Could| Tarefas interessantes e que poderiam ser feitas, mas não são tão importantes para o sucesso do produto (Poderia fazer) |
| Won't | Tarefas menos importantes e o time decide não fazer em um futuro próximo (Não vou fazer) |



## Referências
 
 * COHN, M. Agile Estimating and Planning. Prentice Hall, 2005.
 * COHN, M. User Stories Applied. Addison-Wesley Professional, 2004.
 * SOMMERVILLE, I. Software Engineering. 9ª. ed. Pearson Education India, 2011.
