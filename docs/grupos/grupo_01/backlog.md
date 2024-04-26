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


## Requisitos Funcionais
Neste tópico, apresentam-se as histórias de usuários organizadas de acordo com seus respectivos épicos e derivam dos requisitos funcionais coletados durante a fase de coleta e refinamento dos requisitos. Cada um destes épicos, juntamente com suas histórias de usuários correspondentes, é descrito em detalhes nas subseções seguintes.

### Envio de Exames
Permite anexar exames de um paciente e extrair informações relevantes através do processamento avançado de dados.

### Cartão
Permite o usuário gerar e personalizar um cartão de informações.


<br />
A seguir, são apresentadas as histórias de usuário dos épicos em questão.

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FGrKcl3XqGJAJjkbnnWKexq%2FBacklog---Grupo-1%3Ftype%3Ddesign%26mode%3Ddesign%26t%3DfuW2qKRRQfiGTXkE-1" allowfullscreen></iframe>
    <figure style="font-style: italic;">
    Aguarde o carregamento da visualização, ou se preferir vá direto ao link<a href="https://www.figma.com/file/GrKcl3XqGJAJjkbnnWKexq/Backlog---Grupo-1?type=design&mode=design&t=fuW2qKRRQfiGTXkE-1"><u>aqui</u></a>.
</figure>
</div>


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

## Referências
 
 * COHN, M. Agile Estimating and Planning. Prentice Hall, 2005.
 * COHN, M. User Stories Applied. Addison-Wesley Professional, 2004.
 * SOMMERVILLE, I. Software Engineering. 9ª. ed. Pearson Education India, 2011.
