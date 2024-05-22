<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);"ss />
</div>

<br/>

Neste documento, estão delineadas a estratégia de testes que será utilizada pelo [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo), a fim de garantir a qualidade do produto de software.

## Histórico de versões

| Versão |    Data    |              Descrição               |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :----------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento de Plano de Teste e Qualidade | [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo) |      -      |

O projeto será conduzido utilizando a metodologia de **_Desenvolvimento Orientado a Testes (TDD)_**, que é uma abordagem de desenvolvimento de software onde os testes são escritos antes do código de produção. Isso garante que o código seja desenvolvido de forma mais robusta e confiável, pois cada funcionalidade é validada por testes automatizados.

No frontend, a tecnologia escolhida é **_React com TypeScript (TS)_**. **_React_** é uma biblioteca JavaScript amplamente utilizada para construir interfaces de usuário, enquanto **_TypeScript_** adiciona tipagem estática ao JavaScript, proporcionando mais segurança e robustez ao código.

Para os testes unitários no frontend, serão utilizadas ferramentas e bibliotecas adequadas para o ambiente React, como **_Jest_** e **_React Testing Library_** e **_Cypress_**. Estas ferramentas permitem escrever e executar testes de forma eficiente e abrangente, garantindo a qualidade do código produzido.

O **_Cypress_** é uma ferramenta de teste end-to-end (E2E) que permite simular interações do usuário em um navegador web real. Ele é especialmente útil para testar fluxos de usuário complexos e garantir que a aplicação funcione conforme o esperado do ponto de vista do usuário final. Com o **_Cypress_**, os desenvolvedores podem escrever testes descritivos que interagem com o aplicativo da mesma forma que um usuário real, clicando em botões, preenchendo formulários e navegando entre páginas. Além disso, o **_Cypress_** oferece assertivas poderosas para verificar o comportamento esperado do aplicativo, proporcionando uma maneira confiável de garantir a qualidade e a integridade do código front-end.

Por outro lado, o **_Jest_** é uma estrutura de teste de código aberto mantida pelo Facebook. Ele é amplamente utilizado para testes unitários. O **_Jest_** é conhecido por sua simplicidade de uso, velocidade de execução e integração perfeita com outras ferramentas populares, como Babel e Webpack. Ele oferece uma variedade de funcionalidades poderosas, como mocks automáticos, snapshots de componentes e suporte a testes assíncronos, tornando-o uma escolha ideal para desenvolvedores que desejam garantir a qualidade do código front-end por meio de testes abrangentes e confiáveis.

No backend, a linguagem escolhida é **_Java_**, uma linguagem de programação popular e amplamente utilizada para desenvolvimento de aplicativos empresariais e sistemas distribuídos.

Para os testes serão utilizadas as bibliotecas **_JUnit_** e **_Mockito_**. O **_JUnit_** é um framework de teste de código aberto para Java, amplamente utilizado para escrever e executar testes unitários, e o **_Mockito_** é uma biblioteca de mocking para Java que facilita a criação de mocks e stubs de objetos em testes unitários.

Para garantir a qualidade do código Java e realizar testes estáticos, será utilizado o **_Quodana_**, uma ferramenta de análise estática de código que ajuda a identificar possíveis problemas e vulnerabilidades no código-fonte.

Com essa abordagem, espera-se desenvolver um software de alta qualidade, com testes abrangentes e uma arquitetura robusta tanto no frontend quanto no backend.


## Referências

- React: Uma biblioteca JavaScript para construir interfaces de usuário. Disponível em: https://reactjs.org/

- TypeScript: Um superconjunto de JavaScript que adiciona tipagem estática. Disponível em: https://www.typescriptlang.org/

- Jest: Uma estrutura de teste de código aberto mantida pelo Facebook. Disponível em: https://jestjs.io/

- Cypress: Uma ferramenta de teste end-to-end (E2E) para aplicativos web. Disponível em: https://www.cypress.io/

- JUnit: Um framework de teste de código aberto para Java. Disponível em: https://junit.org/junit5/

- Mockito: Uma biblioteca de mocking para Java que facilita a criação de mocks e stubs de objetos em testes unitários. Disponível em: https://site.mockito.org/

- Quodana: Uma ferramenta de análise estática de código para Java. Disponível em: https://www.quodana.com/