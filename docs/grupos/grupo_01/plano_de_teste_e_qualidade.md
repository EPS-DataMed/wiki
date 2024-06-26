
<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

Neste documento, estão delineadas a estratégia de testes que será utilizada pelo [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo), a fim de garantir a qualidade do produto de software.

## Histórico de versões

| Versão |    Data    |              Descrição               |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :----------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 16/04/2024 | Criando documento de Plano de Teste e Qualidade | [Grupo 01](/grupos/grupo_01?id=integrantes-do-grupo) |      -      |

O projeto será conduzido utilizando a metodologia de **_Desenvolvimento Orientado a Testes (TDD)_**, que é uma abordagem de desenvolvimento de software onde os testes são escritos antes do código de produção. Isso garante que o código seja desenvolvido de forma mais robusta e confiável, pois cada funcionalidade é validada por testes automatizados.

No frontend, a tecnologia escolhida é **_React com TypeScript (TS)_**. **_React_** é uma biblioteca JavaScript amplamente utilizada para construir interfaces de usuário, enquanto **_TypeScript_** adiciona tipagem estática ao JavaScript, proporcionando mais segurança e robustez ao código.

Para os testes unitários no frontend, serão utilizadas ferramentas e bibliotecas adequadas para o ambiente React, como **_Jest_** e **_React Testing Library_**. Estas ferramentas permitem escrever e executar testes de forma eficiente e abrangente, garantindo a qualidade do código produzido.

Por outro lado, o **_Jest_** é uma estrutura de teste de código aberto mantida pelo Facebook. Ele é amplamente utilizado para testes unitários. O **_Jest_** é conhecido por sua simplicidade de uso, velocidade de execução e integração perfeita com outras ferramentas populares, como Babel e Webpack. Ele oferece uma variedade de funcionalidades poderosas, como mocks automáticos, snapshots de componentes e suporte a testes assíncronos, tornando-o uma escolha ideal para desenvolvedores que desejam garantir a qualidade do código front-end por meio de testes abrangentes e confiáveis.

Os repositórios de microserviços estão utilizando **_Python_** e **_pytest_** para desenvolvimento e testes. **_pytest_** é uma estrutura de teste poderosa e fácil de usar, que permite escrever testes simples e escaláveis para aplicações Python. Essa escolha garante que os microserviços sejam testados de forma eficiente, aumentando a confiabilidade e qualidade do software entregue.

## Referências

- React: Uma biblioteca JavaScript para construir interfaces de usuário. Disponível em: https://reactjs.org/
- TypeScript: Um superconjunto de JavaScript que adiciona tipagem estática. Disponível em: https://www.typescriptlang.org/
- Jest: Uma estrutura de teste de código aberto mantida pelo Facebook. Disponível em: https://jestjs.io/
- pytest: Uma estrutura de teste poderosa e fácil de usar para aplicações Python. Disponível em: https://docs.pytest.org/en/stable/
