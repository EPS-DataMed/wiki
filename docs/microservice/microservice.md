<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/ARQ01.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

## Histórico de versões

| Versão |    Data    |              Descrição               |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :----------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 24/04/2024 | Criando documento de Microserviços | Todos do grupo|      -      |

## 1. Introdução

A arquitetura de microserviços é uma abordagem moderna para o desenvolvimento de sistemas complexos e escaláveis. Diferente do modelo monolítico, onde todas as funcionalidades são desenvolvidas e implantadas como uma única aplicação, os microserviços dividem o sistema em serviços menores e independentes. Cada microserviço é responsável por uma funcionalidade específica e comunica-se com outros serviços através de APIs bem definidas.

Essa abordagem oferece várias vantagens, incluindo maior flexibilidade na escolha de tecnologias, pois cada microserviço pode ser desenvolvido com a linguagem e o framework mais adequados para a sua função. Além disso, facilita a escalabilidade, permitindo que serviços específicos sejam escalados independentemente conforme a demanda. Outro benefício significativo é a melhoria na manutenção e na velocidade de desenvolvimento, já que equipes diferentes podem trabalhar simultaneamente em serviços distintos sem interferir umas nas outras.

No entanto, a arquitetura de microserviços também traz desafios, como a necessidade de um gerenciamento eficiente da comunicação entre serviços, a orquestração de deploys e a complexidade na monitoração e debug do sistema como um todo. Esses desafios podem ser mitigados com o uso de ferramentas e práticas adequadas, tornando a abordagem de microserviços uma escolha poderosa para muitos tipos de aplicações.

## 2. Arquitetura do Projeto

O projeto está estruturado em diversos componentes, cada um representando um microserviço ou uma funcionalidade específica. Essa organização modular permite uma maior flexibilidade e escalabilidade, facilitando o desenvolvimento, a manutenção e a implantação dos serviços.

No centro da arquitetura está o gateway, que atua como um ponto de entrada único para todas as requisições, direcionando-as para os microserviços apropriados. Essa camada de gateway não só simplifica a comunicação entre o front-end e os back-end services, mas também oferece funcionalidades adicionais como autenticação, roteamento e agregação de dados.

Os microserviços estão divididos em diferentes categorias, como microserviços consumidos, microserviços consumíveis e os próprios microserviços principais. Cada um destes desempenha um papel crucial na arquitetura geral, garantindo que as funcionalidades sejam bem distribuídas e gerenciáveis. A imagem a seguir detalha visualmente essa arquitetura, mostrando como cada componente se interliga.

## 3. Componentes de Arquitetura

O frame abaixo representa a arquitetura do projeto Datamed, que utiliza uma abordagem baseada em microserviços. Cada componente é responsável por uma funcionalidade específica, facilitando a manutenção, escalabilidade e deploy independente.


<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fdesign%2Fyu7o6OMcKcWTIKbzNSR75f%2FArquitetura-%25E2%2580%25A2-Datamed%3Fnode-id%3D0-1%26t%3DOCcQ73BFiPBZptqM-1" allowfullscreen></iframe>

<h3>3.1 Front-end</h3>
<div>
    <strong>✓ datamed:</strong> Representado na cor verde, o <code>datamed</code> é a interface do usuário, responsável por interagir com os serviços backend através do gateway.
</div>

<h3>3.2 Gateway</h3>
<div>
    <strong>✓ gateway:</strong> Representado na cor ciano, o <code>gateway</code> atua como um ponto de entrada único para as requisições do front-end, encaminhando as chamadas para os microserviços apropriados.
</div>

<h3>3.3 Microserviços Consumidos</h3>
<div>
    <strong>✓ privacy:</strong> Representado na cor cinza, o microserviço <code>privacy</code> é responsável pelo gerenciamento e aplicação das políticas de privacidade dos dados.
</div>
<br/>
<div>
    <strong>✓ encryption:</strong> Também representado na cor cinza, o microserviço <code>encryption</code> cuida da criptografia e segurança de senhas, assegurando que todas as informações armazenadas e transmitidas estejam protegidas.
</div>

<h3>3.4 Microserviços</h3>
<div>
    <strong>✓ authentication:</strong> Representado na cor laranja, o microserviço <code>authentication</code> lida com a autenticação de usuários, incluindo login, registro e gerenciamento de sessões.
</div>
<br/>
<div>
    <strong>✓ user-service:</strong> Também na cor laranja, o <code>user-service</code> é responsável pela gestão de usuários, incluindo perfis, permissões e informações pessoais.
</div>
<br/>
<div>
    <strong>✓ data-processing:</strong> Este microserviço, na cor laranja, processa os dados provindos de exames médicos recebidos, realizando transformações, validações e armazenamento conforme necessário.
</div>
<br/>
<div>
    <strong>✓ file-manager:</strong> Representado na cor laranja, o <code>file-manager</code> gerencia o armazenamento, recuperação e manipulação de arquivos dentro do sistema. Este serviço utiliza a AWS para salvar os arquivos dos usuários.
</div>

<h3>3.5 Microserviços Consumíveis</h3>
<div>
    <strong>✓ terms:</strong> Na cor rosa, o microserviço <code>terms</code> gerencia os termos e condições que os usuários devem aceitar para utilizar o serviço.
</div>
<br/>
<div>
    <strong>✓ extract-info-pdf:</strong> Também na cor rosa, o <code>extract-info-pdf</code> é responsável por extrair informações de documentos PDF, processando-os para uso interno ou apresentação ao usuário.
</div>

<h3>3.6 Banco de Dados</h3>
<div>
    <strong>✓ database:</strong> Representado na cor amarela, o <code>database</code> armazena todos os dados estruturados necessários para o funcionamento dos microserviços.
</div>

<h3>3.7 Serviços de Computação em Nuvem</h3>
<div>
    <strong>✓ AWS:</strong> Representado na cor cinza, o serviço <code>AWS</code> fornece infraestrutura e serviços em nuvem para armazenamento, processamento e outras funcionalidades escaláveis.
</div>
<br />
<div>
    Essa estrutura modular facilita a escalabilidade e manutenção do sistema, permitindo que cada microserviço seja desenvolvido, implantado e escalado independentemente.
</div>

## 4. CI/CD

O deploy dos microserviços do projeto Datamed é realizado utilizando a plataforma [Render.com](https://render.com/). Essa plataforma facilita a implantação contínua e automatizada, oferecendo suporte robusto para serviços baseados em contêineres. 

<img width="1493" alt="image" src="https://github.com/EPS-DataMed/.github/assets/48137972/0ffc6a8b-be61-49d3-b52b-43584907f8d6">

### 4.1 Processo de Deploy

1. **Configuração do Ambiente**: Inicialmente, os ambientes de produção e desenvolvimento são configurados na plataforma Render.com. Isso inclui a definição das variáveis de ambiente necessárias para o funcionamento dos microserviços.

2. **Build e Deploy Automático**: A cada commit realizado no repositório principal do projeto, o Render.com automaticamente realiza o build e o deploy dos microserviços. Isso garante que as versões mais recentes do código estejam sempre em produção ou no ambiente de testes.

3. **Escalabilidade e Monitoramento**: A plataforma Render.com permite escalar automaticamente os microserviços de acordo com a demanda. Além disso, oferece ferramentas de monitoramento e logging que ajudam a identificar e resolver problemas rapidamente.

4. **Gerenciamento de Configurações**: Utilizando os recursos de configuração do Render.com, é possível gerenciar as diferentes versões dos serviços e aplicar alterações de configuração sem a necessidade de downtime.

### 4.2 Benefícios

- **Automação**: O deploy automatizado reduz erros humanos e acelera o processo de colocação de novas funcionalidades em produção.
- **Escalabilidade**: A capacidade de escalar os serviços conforme necessário garante que o sistema possa lidar com picos de tráfego sem degradação de desempenho.
- **Confiabilidade**: O monitoramento contínuo e os logs centralizados ajudam a manter o sistema estável e identificar problemas rapidamente.

### 4.3 Desafios e Considerações

- **Gerenciamento de Estado**: Como os microserviços são implantados de forma independente, é crucial gerenciar o estado e a consistência dos dados.
- **Compatibilidade de Versões**: Garantir que diferentes versões dos microserviços possam se comunicar corretamente é um desafio contínuo.

Ao utilizar Render.com, o projeto Datamed consegue uma implantação ágil e eficiente, suportando a arquitetura de microserviços de forma robusta e escalável.

## 5. Qualidade de Código com SonarCloud

Todos os repositórios do projeto Datamed utilizam o [SonarCloud](https://sonarcloud.io/) para garantir a qualidade do código. O SonarCloud é uma plataforma de análise de código que ajuda a identificar problemas de segurança, bugs e questões de manutenção em projetos de software.

<img width="927" alt="image" src="https://github.com/EPS-DataMed/client-side/assets/48137972/1fac163f-d735-44f2-ad2b-83a5dd6c88ff">

### 5.1 Integração com SonarCloud

1. **Configuração Inicial**: Cada repositório do projeto foi configurado para integração com o SonarCloud. Isso inclui a definição de projetos no SonarCloud e a adição dos tokens de autenticação necessários nos pipelines de CI/CD.

2. **Análise Contínua**: A cada commit e pull request, uma análise de código é executada automaticamente. O SonarCloud verifica o código contra um conjunto de regras pré-definidas, cobrindo aspectos como segurança, bugs, vulnerabilidades e manutenibilidade.

3. **Relatórios e Métricas**: Após cada análise, o SonarCloud gera relatórios detalhados que são disponibilizados diretamente na interface web da plataforma. Esses relatórios incluem métricas de cobertura de testes, dívida técnica, duplicação de código e muito mais.

### 5.2 Benefícios do SonarCloud

- **Detecção de Problemas Antecipada**: Com a análise contínua, problemas potenciais são identificados e resolvidos rapidamente, antes de chegarem à produção.
- **Melhoria Contínua**: O feedback constante ajuda os desenvolvedores a melhorar continuamente a qualidade do código, promovendo boas práticas de programação.
- **Transparência e Conformidade**: Relatórios detalhados e históricos de análise fornecem transparência sobre a qualidade do código e garantem conformidade com os padrões estabelecidos.

### 5.3 Qualidade e Conformidade

Todos os repositórios do projeto estão de acordo com os padrões de qualidade estabelecidos no SonarCloud. Isso inclui alta cobertura de testes, baixa dívida técnica e ausência de vulnerabilidades críticas. A utilização do SonarCloud assegura que o código é robusto, seguro e fácil de manter.

### 5.4 Desafios e Considerações

- **Configuração de Regras**: Personalizar as regras de análise para que se adequem às necessidades específicas do projeto pode ser um desafio inicial, mas é essencial para obter resultados precisos.
- **Acompanhamento Contínuo**: É importante que a equipe continue monitorando os relatórios do SonarCloud e tomando ações corretivas conforme necessário.

A integração com o SonarCloud fortalece a qualidade do projeto Datamed, promovendo um ciclo de desenvolvimento mais seguro e eficiente.

## 6. Referências

- NEWMAN, Sam. *Building Microservices: Designing Fine-Grained Systems*. 2. ed. Beijing: O'Reilly Media, 2021.
- WOLFF, Eberhard. *Microservices: Flexible Software Architecture*. Addison-Wesley Professional, 2016.
- RICHARDSON, Chris. *Microservices Patterns: With examples in Java*. Manning Publications, 2018.
- NADER, Kinsey. *Cloud Native Microservices with Spring and Kubernetes: A practical guide to building enterprise-grade microservices with Spring and Kubernetes*. Packt Publishing, 2021.
- VERNON, Vaughn. *Strategic Monoliths and Microservices: Driving Innovation Using Purposeful Architecture*. Addison-Wesley Professional, 2021.

