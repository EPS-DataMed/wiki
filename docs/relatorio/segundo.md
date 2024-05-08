<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/ANALISE.png" width="200" height="200" style="filter: brightness(0%);"ss />
</div>

<br/>

Neste documento, é apresentado o relatório referente ao segundo periodo do projeto.

## Histórico de versões

| Versão |    Data    |           Descrição            |  Autor(es)   |  Revisor(es)  |
| :----: | :--------: | :----------------------------: | :----------: | :-----------: |
| `1.0`  | 05/04/2024 | Criando documento de Relatório | Daniel Veras | Lucas Gabriel |
| `2.0`  | 07/05/2024 | Criando documento de Relatório | Daniel Veras, Victor Amaral Cerqueira, Luiz Gustavo Dias, Vítor Diniz Pagani, Antônio Rangel Chaves, Arthur de Melo Garcia| Luiz Gustavo Dias |
## Segundo Relatório EPS - DataMed (Healthtech)

**Equipe:**  DataMed

**Cliente:** Fernando Viana  

**Produzido por:** Luiz Gustavo, Daniel Veras, Victor Amaral Cerqueira, Vítor Diniz Pagani, Antônio Rangel Chaves, Arthur de Melo Garcia

**Revisado por:** Luiz Gustavo, Daniel Veras, Victor Amaral Cerqueira, Vítor Diniz Pagani, Antônio Rangel Chaves, Arthur de Melo Garcia

**Data coberta pelo relatório:** 07/04 a 08/05

## Integrantes

Abaixo estão os integrantes e seus respectivos cargos, conforme a Tabela 1, abaixo.

| Nome                                | Cargo          |
| ----------------------------------- | -------------- |
| Victor Amaral Cerqueira             | Desenvolvedor  |
| Luiz Gustavo Dias                   | Desenvolvedor  |
| Sávio Cunha de Carvalho             | Desenvolvedor  |
| Elias Yousef Santana                | Desenvolvedor  |
| Vítor Diniz Pagani                  | Desenvolvedor  |
| Antônio Rangel Chaves               | Desenvolvedor  |
| Arthur de Melo Garcia               | Desenvolvedor  |
| Kess Jhones Gomes                   | Desenvolvedor  |
| Daniel de Sousa Oliveira Melo Veras | Desenvolvedor  |
| Lucas Gabriel Sousa Camargo Paiva   | Desenvolvedor  |

<div style="text-align: center">
<p> Tabela 1: Definição de funções dos membros (Fonte: autor, 2024). </p>
</div>

## Visão Geral

Este relatório abrange o segundo período de planejamento e desenvolvimento do projeto, durante o qual foram realizadas diversas reuniões e atividades voltadas ao desenvolvimento do projeto, artefatos, levantamento da documentação necessária, definições técnicas a respeito das tecnologias,
, projeto do banco de dados, estrutura do repositório, validação de prótotipo com o cliente, criação do ambiente de desenvolvimento
e inicio do desenvolvimento do código própriamente dito.

Durante este período, foram realizadas 9 reuniões, entre subgrupos, grupo geral e incluindo quatro com a presença do cliente, com o objetivo de compreender melhor a visão do produto e validar o projeto desenvolvido até o presente momento.
Para o próximo período de desenvolvimento, planejamos focar no desenvolvimento do software.

## Cronograma
Um cronograma foi criado com base nas datas das disciplinas. As histórias de usuário definidas no backlog foram distribuídas em sprints de duas semanas. A primeira sprint começou em 29/04. Ele foi criado em forma de
roadmap no GitHub Projects e pode ser encontrado no link: https://github.com/orgs/EPS-DataMed/projects/1/views/2?groupedBy%5BcolumnId%5D=98914740

## Plano de Iteração

Considerando as sprints de duas semanas, e a última de 4 dias (por conta do calendário da UnB) nós iremos seguir 5 iterações. Essas iterações estão no roadmap e podem ser
encontradas no link: https://github.com/orgs/EPS-DataMed/projects/1/views/2?groupedBy%5BcolumnId%5D=98914740

## Configuração do Repositório / Configuração do Ambiente
O ambiente e repositório foi configurado no github e pode ser encontrado em: https://github.com/EPS-DataMed

## Backlog

A partir do Lean Inception chegamos na definição de dois épicos: Gerência de Pacientes e Dados de Saúde. E com base nos épicos foram montadas 17 história
de usuário que descrevem o que o DataMed deve fazer. O backlog completo pode ser encontrado no link: https://healthtech-doc-fga-eps-rmc-healthtech-5e4df58c4b433446d7c8f4f18.gitlab.io/#/reunioes/backlogGeral

## Kanban

A equipe está utilizando o quadro Kanban do próprio GitHub, para controle das tarefas definidas nas issues, para facilitar a observação das tarefas a serem realizadas, em progresso e finalizadas

#Protótipo de Alta Fidelidade 

Dividimos o grupo em 3 subgrupos, cada grupo ficou responsável por um épico, são eles Gerência de Pacientes, Envio de Exames e Compartilhamento de dados. Abaixo está o link de acesso para visualização do protótipo:
https://www.figma.com/file/1dpqTkNRHpdYYgkIXuLG39/Envio-de-Exames?type=design&node-id=190-619&mode=design
A validação do protótipo não foi concluída totalmente devido a dificuldade de conversarmos com o cliente, ainda estamos caminhando para uma validação completa. Abaixo temos um link de uma primeira validação com o cliente:
https://www.youtube.com/watch?v=Eynu7nJD178&list=PLE4Al1kGMC3K0fqa3RJZrf87ByLi0L6Ro&index=2

## Épicos
Os épicos são: Gerência de Pacientes, Envio de Exames e Compartilhamento de dados. Cada subgrupo ficou responsável por um épico.

## Scrum
Adotamos o framework SCRUM para o desenvolvimento do produto. Com o backlog montado do produto e validado pelo usuário, dividimos as tarefas entre os subgrupos por épicos como descrito anteriormente.
Nosso planejamento inicial era de termos sprints de 15 dias, porém, devido a alteração relacionada às datas de entrega, tivemos que optar por fazer sprints menores, cada uma contendo 7 dias. Quanto às cerimônias, cada subgrupo está mantendo o contato via Telegram pelo tópico de sua equipe, não estamos realizando mais do que a daily de cerimônias até o momento, devido a divisão do projeto na matéria, e também pelo desenvolvimento atual do software não ter exigido uma reunião de revisão.

## Pipeline CI/CD
O pipeline de front-end iremos utilizar a Vercel, para o back-end utilizaremos a plataforma Render. Ambas as ferramentas são ativadas automaticamente ao commitar na branch principal do código. E para o banco de dados a gente ainda está pesquisando um local para hospedar. 

## Testes
Para o front-end iremos usar o react-testing-library e no back-end pytest além de junit.

## Sonar
Estamos estudando a implementação.

## Microserviços
Já possuímos uma arquitetura definida. Cada grupo já está trabalhando em um micro serviço, no épico de Gerência de Pacientes utilizaremos um micro serviço, no Épico de Envio de exames utilizaremos três, e no compartilhamento de dados utilizaremos apenas um. Todos os serviços serão intermediados por um gateway.

## Plano de gestão de riscos
Também desenvolvemos um plano de gestão de riscos, que pode ser encontrado no link: https://eps-datamed.github.io/wiki/#/sprint/plano_gerenciamento_riscos

Este relatório reflete o progresso e as atividades realizadas pela equipe DataMed durante o período mencionado. O próximo passo é seguir com o plano de desenvolvimento estabelecido para o projeto.

---
Este relatório foi produzido por Daniel Veras, Victor Amaral Cerqueira, Luiz Gustavo Dias, Vítor Diniz Pagani, Antônio Rangel Chaves, Arthur de Melo Garcia
e revisado por Luiz Gustavo Dias.
