
<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

Neste documento, estão delineadas a estratégia de testes que será utilizada pela equipe, a fim de garantir a qualidade do produto de software.

## Histórico de versões

| Versão |    Data    |              Descrição              |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :---------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento de Plano de Teste | [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo) |      -      |


## Objetivo dos testes

Os testes desse projeto visam a garantir a establidade e confiança do produto em desenvolvimento, assegurando que não haja _bugs_ em ambiente de produção. Assim, evitando que os usuário enfrente situações desagradáveis ou inseperadas durante o uso da aplicação. As funcionalidades que possuem maior impacto no codigo devem ser priorizadas nos testes e os testes tem como principal métrica de sucesso atingir a meta de uma cobertura de código de pelo menos 80%.

## Timeline das Sprints

As Sprints de desenvolvimento terão duração de 1 semana, visando o desenvolvimento das funcionalidades descritas em cada uma delas, os testes por sua vez visam comprovar a entrega dessas funcionalidades de forma eficaz e com qualidade. As principais releases serão a R1 e R2 marcadas para as datas de 29/05/2024 a 04/06/2024 e 03/07/2024 a 09/07/2024, respectivamente.

## Ciclo de Vida das Tarefas

Um item da Sprint pode ser considerado pronto assim que o código relacionado ao mesmo obtiver uma cobertura de testes de 80% ou mais.

## Identificação dos Tipos de Teste

Em primeiro momento o projeto terá como foco principal a realização de Testes Funcionais, sendo realizados por meio de Testes Unitários, os quais cumprirão com o objetivo incial de assegurar a qualidade do código em produção, evitando comportamentos inesperados. Em um segundo momento, serão implementados Testes de Segurança e Testes de Performance, os quais vissam dar completude a qualidade do software.

## Papeis de Teste na Equipe

O projeto será conduzido utilizando a metodologia de **_Desenvolvimento Orientado a Testes (TDD)_**, que é uma abordagem de desenvolvimento de software onde os testes são escritos antes do código de produção. Isso garante que o código seja desenvolvido de forma mais robusta e confiável, pois cada funcionalidade é validada por testes automatizados.

## Ferramentas de Testes

No frontend, a tecnologia escolhida é o **_React com TypeScript (TS)_**. **_React_** é uma biblioteca JavaScript amplamente utilizada para construir interfaces de usuário, enquanto **_TypeScript_** adiciona tipagem estática ao JavaScript, proporcionando mais segurança e robustez ao código.

Para os testes unitários no frontend, serão utilizadas ferramentas e bibliotecas adequadas para o ambiente React, como **_Jest_** e **_React Testing Library_**. Estas ferramentas permitem escrever e executar testes de forma eficiente e abrangente, garantindo a qualidade do código produzido.

Por outro lado, o **_Jest_** é uma estrutura de teste de código aberto mantida pelo Facebook. Ele é amplamente utilizado para testes unitários. O **_Jest_** é conhecido por sua simplicidade de uso, velocidade de execução e integração perfeita com outras ferramentas populares, como Babel e Webpack. Ele oferece uma variedade de funcionalidades poderosas, como mocks automáticos, snapshots de componentes e suporte a testes assíncronos, tornando-o uma escolha ideal para desenvolvedores que desejam garantir a qualidade do código front-end por meio de testes abrangentes e confiáveis.

Os repositórios de microserviços estão utilizando **_Python_** e **__Fast API__** para o desenvolvimento. O **__Fast API__**
é um **__framework__** muito utilizado para o desenvolvimento de APIs em Python, devido sua velocidade no desenvolmento e de execução. Para o desenvolvimento dos testes será utilizado o framework **_pytest_** em conjunto com as ferramentas de testes disponibilizadas pelo framework **__Fast API__** e a biblioteca **_unittest mock_** para permitir a realização de testes sem que esses afetem os ambientes de produção. O **_pytest_** é uma estrutura de teste poderosa e fácil de usar, que permite escrever testes simples e escaláveis para aplicações Python. Essa escolha garante que os microserviços sejam testados de forma eficiente, aumentando a confiabilidade e qualidade do software entregue.

## Ambiente de Testes

Os testes deverão ser executados localmente em ambiente de desenvolvimento após a realização do ciclo do TDD, em seguida com a realização de um __Pull Request__, os testes serão executados novamente pela pipeline de Integração Contínua do **__GitHub Actions__** integrada a ferramenta de análise estática de código: **__Sonar Cloud__**, a aqual indicará se os critérios de aceite foram satisfeitos para que o código passe para o ambiente de produção.

## Monitoramento de Testes

O monitoramento dos testes serão realizados pela ferramenta **__Sonar Cloud__**, a qual possibilitará a visualização da situação dos testes do projeto.

## Referências

* <div>TDD – Test Driven Development. Disponível em: <a href="https://example.com/tdd-introduction" target="_blank">https://example.com/tdd-introduction</a>. Acesso em: 16 abr. 2024.</div>
* <div>React. Disponível em: <a href="https://reactjs.org/" target="_blank">https://reactjs.org/</a>. Acesso em: 16 abr. 2024.</div>
* <div>TypeScript. Disponível em: <a href="https://www.typescriptlang.org/" target="_blank">https://www.typescriptlang.org/</a>. Acesso em: 16 abr. 2024.</div>
* <div>Jest. Disponível em: <a href="https://jestjs.io/" target="_blank">https://jestjs.io/</a>. Acesso em: 16 abr. 2024.</div>
* <div>React Testing Library. Disponível em: <a href="https://testing-library.com/docs/react-testing-library/intro/" target="_blank">https://testing-library.com/docs/react-testing-library/intro/</a>. Acesso em: 16 abr. 2024.</div>
* <div>Python. Disponível em: <a href="https://www.python.org/" target="_blank">https://www.python.org/</a>. Acesso em: 16 abr. 2024.</div>
* <div>pytest. Disponível em: <a href="https://docs.pytest.org/en/6.2.x/" target="_blank">https://docs.pytest.org/en/6.2.x/</a>. Acesso em: 16 abr. 2024.</div>
* <div>‌MERLIN, Team. Test Strategy in an Agile Scrum project - Government Digital Services, Singapore - Medium. Medium. Disponível em: <a href="https://medium.com/singapore-gds/test-strategy-in-an-agile-scrum-project-e2754a2cd634" target="_blank">https://medium.com/singapore-gds/test-strategy-in-an-agile-scrum-project-e2754a2cd634</a>. Acesso em: 16 abr. 2024.</div>

‌