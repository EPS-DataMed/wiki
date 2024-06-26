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

<!-- | ID | Épico | Grupo responsável |
|:--:|:-----:|:-----------------:|
| EP 01 | Gerência de Pacientes | Grupo 2 |
| EP 02 | Dados de Saúde | Grupo 1 e 2 |
| EP 03 | Agendamento de consultas | Grupo 3 | -->


### Histórias de Usuário

Histórias de usuário são uma técnica de documentação amplamente utilizada no desenvolvimento de software ágil. Elas são pequenas descrições de funcionalidades ou requisitos do ponto de vista do usuário. Cada história de usuário é uma narrativa concisa que descreve o que um usuário deseja alcançar ao interagir com um sistema ou software. Essas histórias são fundamentais para entender as necessidades do cliente e guiar o desenvolvimento de software centrado no usuário. Elas geralmente seguem um formato simples e são uma parte essencial do backlog do produto.

| Épico | ID | História de Usuário | Prioridade |
|:-----:|:--:|:-------------------:|:----------:|
| EP 01 | US 01 | Eu, como Usuário, desejo fazer login no DataMed | Must |
| EP 01 | US 02 | Eu, como Usuário, desejo fazer logout no DataMed | Must |
| EP 01 | US 03 | Eu, como Usuário, desejo me cadastrar no DataMed | Must |
| EP 01 | US 04 | Eu, como Usuário, desejo editar meus dados cadastrados | Must |
| EP 01 | US 05 | Eu, como Usuário, desejo excluir minha conta doo DataMed | Must |
| EP 01 | US 06 | Eu, como Usuário, desejo cadastrar meus dependentes no DataMed | Must |
| EP 01 | US 07 | Eu, como Usuário, desejo editar os dados dos meus dependentes no DataMed | Must |
| EP 01 | US 08 | Eu, como Usuário, desejo excluir as contas dos meus dependentes no DataMed | Must |
| EP 02 | US 31 | Eu, como usuário, desejo cadastrar meus dados de saúde | Must |
| EP 02 | US 09 | Eu, como Usuário, gostaria de visualizar um histórico detalhado de todos os exames realizados meus ou de meus dependentes. | Should |
| EP 02 | US 10 | Eu, como Usuário, gostaria de realizar upload de exames no formato PDF | Must |
| EP 02 | US 11 | Eu, como Usuário, gostaria que o sistema me guiasse no processo de preencher os dados de saúde | Could |
| EP 02 | US 12 | Eu, como Usuário, gostaria que o sistema enviasse o cartão por E-mail | Could |
| EP 02 | US 13 | Eu, como Usuário, gostaria de que os dados contidos nos exames enviados por PDF fossem processados automaticamente | Should |
| EP 02 | US 14 | Eu, como Usuário, gostaria de preencher um formulário manualmente para o envio de exames | Must |
| EP 02 | US 15 | Eu, como Usuário, gostaria de gerar um cartão contendo resumo dos meus dados médicos ou de meus dependentes | Must |
| EP 02 | US 16 | Eu, como Usuário, gostaria de imprimir um cartão contendo resumo dos meus dados médicos ou de meus dependentes | Must |
| EP 02 | US 32 | Eu, como Usuário, gostaria de adicionar documentos pdf e imagens em um campo "Informações adicionais", no momento de preencher os dados de saúde | Must |
| EP 03 | US 17 | Eu, como Administrador, gostaria de cadastrar novas instituições fornecendo nome, tipo, endereço e contato para expandir a rede de atendimento disponível no sistema. | Must |
| EP 03 | US 18 | Eu, como Administrador, gostaria de adicionar especialidades disponíveis em cada instituição durante o cadastro para que os pacientes possam escolher corretamente onde querem ser atendidos | Must |
| EP 03 | US 19 | Eu, como Administrador, gostaria de atualizar ou remover instituições já cadastradas para garantir que a informação no sistema esteja sempre atualizada e correta | Must |
| EP 03 | US 20 | Eu, como Administrador, gostaria de visualizar todas as informações de uma instituição, incluindo detalhes como especialidades oferecidas e médicos disponíveis, para gerenciar eficientemente as instituições. | Must |
| EP 03 | US 21 | Eu, como Administrador, gostaria de editar os detalhes das especialidades para corrigir erros ou atualizar informações. | Must |
| EP 03 | US 22 | Eu, como Administrador, gostaria de remover especialidades que não são mais oferecidas para evitar confusões no agendamento de consultas. | Must |
| EP 03 | US 23 | Eu, como Administrador, gostaria de cadastrar colaboradores no sistema, incluindo informações como nome, CPF e e-mail, para que eles possam ser associados a consultas e especialidades. | Must |
| EP 03 | US 24 | Eu, como Administrador, gostaria de associar colaboradores às instituições em que trabalham para que os pacientes possam agendar consultas corretamente. | Must |
| EP 03 | US 25 | Eu, como Administrador, gostaria de atualizar as informações dos colaboradores ou remover colaboradores do sistema quando necessário | Must |
| EP 03 | US 26 | Eu, como Usuário, gostaria de ter a opção de realizar um agendamento diretamente pelo sistema, facilitando a gestão do meu tempo e evitando deslocamentos desnecessários. | Must |
| EP 03 | US 27 | Eu, como Usuário, gostaria de ter a opção de cancelar ou fazer um reagendamento diretamente pelo sistema, facilitando a gestão do meu tempo e evitando deslocamentos desnecessários. | Must |
| EP 03 | US 28 | Eu, como Usuário, gostaria de poder modificar os detalhes de um agendamento em caso de necessidade, como alterações no horário ou no médico designado, para acomodar. | Should |
| EP 03 | US 29 | Eu, como Usuário, gostaria de poder confirmar ou recusar pedidos de reagendamento ou cancelamento para manter a ordem e eficiência dos agendamentos | Must |
| EP 03 | US 30 | Eu, como Usuário, gostaria de visualizar todas as minhas consultas agendadas, incluindo datas, horários, colaboradores e instituições, para que eu possa gerenciar meu tempo e compromissos de saúde eficientemente. | Must |

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
