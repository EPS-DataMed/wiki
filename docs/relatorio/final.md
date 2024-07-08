<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

Neste documento, é apresentada a versão final do trabalho para a disciplina de Engenharia de Produto de Software.

## Histórico de versões

| Versão |    Data    |                    Descrição                    |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :---------------------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 26/06/2024 | Criando documento do Backlog do Produto | Todos do grupo |      -      |

## Introdução

Este documento apresenta a versão final do projeto desenvolvido para a disciplina de Engenharia de Produto de Software. O objetivo principal deste projeto foi aplicar os conceitos de engenharia de software na elaboração de um backlog de produto, incluindo a definição de requisitos, priorização e estimativa de esforço.

Durante o desenvolvimento do projeto, a equipe utilizou práticas ágeis para garantir a entrega de valor contínua e incremental. O backlog de produto foi desenvolvido com base em user stories, permitindo uma compreensão clara e compartilhada dos requisitos pelos membros da equipe e stakeholders.

<iframe src="https://eps-datamed.github.io/wiki/assets/final.pdf" width="100%" height="600px"></iframe>

## Funcionalidades Desenvolvidas

### Autenticação
Implementamos um **sistema robusto de autenticação** que permite a **criação de contas de usuários**, **login seguro** e **recuperação de senha**. Utilizamos um **serviço de criptografia** para assegurar que todas as senhas sejam armazenadas e transmitidas de forma segura. Esse sistema inclui a **verificação de tokens** de autenticação para proteger as sessões dos usuários contra acessos não autorizados.

### Termos de Uso
Desenvolvemos uma funcionalidade que gera e gerencia os **termos de uso** da aplicação. Os usuários são obrigados a aceitar os termos de uso ao se registrarem, garantindo que estejam cientes e concordem com as políticas e condições estabelecidas pela aplicação. As mudanças nos termos de uso são refletidas dinamicamente, e os usuários são **notificados para revisar e aceitar novamente** os novos termos.

### Usuário
Criamos um módulo de **gerenciamento de usuários** que inclui funcionalidades como **cadastro, edição de perfil, e exclusão de contas**. Este módulo também integra o serviço de criptografia para assegurar que as informações sensíveis dos usuários, como senhas, sejam protegidas. Além disso, o sistema permite que os administradores visualizem e gerenciem os perfis dos usuários.

### Processamento de Exames
Implementamos um **sistema para o processamento de exames médicos**. Esse sistema permite que os **resultados dos exames sejam carregados, processados e armazenados** na aplicação. Os usuários podem **visualizar seus resultados de exames de forma segura e confidencial**, com suporte para a interpretação e análise dos dados fornecidos.

### Gerenciador de Arquivos
Desenvolvemos um **gerenciador de arquivos** que permite aos usuários fazer o **gerenciamento de seus documentos de forma segura**. Este gerenciador de arquivos suporta vários formatos de documentos, porém na aplicação se limita a arquivos para garantir o correto processamento em etapas futuras, e garante que todos os arquivos sejam armazenados e acessados de maneira segura, utilizando **protocolos de segurança avançados**.

### Extração de PDF
Criamos uma funcionalidade de **extração de PDF** que permite a **extração de dados estruturados** a partir de documentos PDF. Esta funcionalidade é essencial para **automatizar a coleta de informações relevantes** dos PDFs e integrá-las nos processos da aplicação. Os dados extraídos são então **armazenados de forma organizada**, facilitando a consulta e posterior análise.

## Funcionalidades Consumidas e Grupo

### Privacy (Gama Budget)
O microsserviço **privacy** é responsável pelo **gerenciamento e aplicação das políticas de privacidade dos dados**. Ele gera os **termos de privacidade** que devem ser aceitos pelos usuários ao utilizar a aplicação. Isso garante que todas as interações e manipulações de dados sejam realizadas de acordo com as normas de privacidade estabelecidas, protegendo os direitos dos usuários e assegurando a conformidade com regulamentações. Além disso, o microsserviço permite **atualizações dinâmicas das políticas de privacidade**, refletindo rapidamente quaisquer mudanças nas regulamentações ou práticas de gerenciamento de dados. Dessa forma, os usuários estão sempre informados sobre como seus dados estão sendo utilizados e protegidos.

### Encryption (Cryptobot)
O microsserviço **encryption** cuida da **criptografia e segurança de senhas**, assegurando que todas as informações armazenadas e transmitidas estejam protegidas. Esse serviço é responsável por lidar com a **criptografia de senhas** durante a criação do usuário, garantindo que as senhas sejam armazenadas de maneira segura e que apenas versões criptografadas sejam mantidas nos bancos de dados. Além disso, o microsserviço também realiza a **descriptografia de senhas** durante o processo de login e troca de senha do usuário. Isso garante que a **verificação das credenciais** seja feita de maneira segura e confiável, protegendo as informações sensíveis contra acessos não autorizados e possíveis vazamentos de dados.

## Experiência de Consumo das Funcionalidades

### Experiência com Privacy (Gama Budget)
O maior desafio foi a **adaptação da interface do usuário** para aceitar os termos de privacidade de forma intuitiva. Garantir que todos os usuários visualizassem e aceitassem as atualizações dos termos sem causar uma interrupção significativa na experiência do usuário foi complicado. Tivemos que implementar **notificações e lembretes persistentes**, além de garantir que as mudanças nos termos fossem refletidas de forma imediata. A documentação fornecida pelo grupo Gama Budget estava **clara e detalhada**, o que facilitou a integração desse microsserviço. Embora complexa, a integração foi essencial para manter a **conformidade com as regulamentações de privacidade de dados**.

### Experiência com Encryption (Cryptobot)
A integração do microsserviço **encryption**, desenvolvido pelo grupo Cryptobot, apresentou vários **desafios técnicos**. Uma das principais dificuldades foi lidar com a **criptografia e descriptografia de senhas em tempo real** durante os processos de criação de usuário, login e troca de senha. A performance do sistema foi impactada inicialmente, e tivemos que **otimizar o fluxo de autenticação** para garantir uma experiência de usuário fluida. Houve também a necessidade de ajustar nossos **testes unitários** para cobrir as novas funcionalidades de segurança, o que aumentou a complexidade do nosso ambiente de testes. Além disso, encontramos **problemas na interoperabilidade** entre o microsserviço de criptografia e o restante da nossa aplicação. Algumas das chamadas de API para a descriptografia das senhas não estavam funcionando conforme esperado, resultando em falhas de autenticação para alguns usuários. Isso nos forçou a **revisar e corrigir a lógica de comunicação** entre os serviços, além de implementar **mecanismos de fallback** para garantir a segurança e a continuidade do serviço. Apesar desses desafios, a integração desse microsserviço **fortaleceu significativamente a segurança** da nossa aplicação, proporcionando uma **camada adicional de proteção** para os dados dos usuários.


## Referências

* COHN, M. Agile Estimating and Planning. Prentice Hall, 2005.
* COHN, M. User Stories Applied. Addison-Wesley Professional, 2004.
* SOMMERVILLE, I. Software Engineering. 9ª. ed. Pearson Education India, 2011.