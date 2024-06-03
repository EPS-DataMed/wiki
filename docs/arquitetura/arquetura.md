<br/>

<div style="display: flex; flex-direction: column; justify-content: center; align-items:center;">
    <img src="https://dansousamelo.github.io/RQ_ISP/assets/backlog/BACKLOG-ICON.png" width="200" height="200" style="filter: brightness(0%);" />
</div>

<br/>

## Histórico de versões

| Versão |    Data    |              Descrição               |                      Autor(es)                       | Revisor(es) |
| :----: | :--------: | :----------------------------------: | :--------------------------------------------------: | :---------: |
| `1.0`  | 24/04/2024 | Criando documento de Arquitetura | Todos do grupo|      -      |

## 1. Introdução

### 1.1 Objetivo do Documento
Este documento tem como objetivo detalhar a **arquitetura** do sistema **Datamed**, que viabiliza o **cadastro de usuários** (comuns e médicos), a **submissão de exames**, a gestão de **dependentes/pacientes** e a geração de **cartões com informações dos exames** para impressão.

### 1.2 Escopo do Sistema
O escopo do sistema **Datamed** abrange:
- **Front-end**: Desenvolvido com **React.js** e **TypeScript**.
- **Back-end**: Implementado com **FastAPI** e **Python**.
- **Banco de dados**: **PostgreSQL**.
- **Ambientes de produção**: **Vercel** e **Render**.

### 1.3 Visão Geral do Sistema
O **Datamed** se configura como uma aplicação web completa para gestão de exames médicos, possibilitando:
- **Submissão de exames**.
- **Processamento dos exames submetidos**.
- **Geração de cartões com informações dos exames** para impressão.

## 2. Visão Geral da Arquitetura

### 2.1 Descrição Geral da Arquitetura
O **Datamed** é estruturado em torno de um **front-end** baseado em **React.js** e um **back-end** robusto com **microsserviços** em **FastAPI**. A comunicação entre as interfaces se dá por meio de **API RESTful**, utilizando um **gateway** como ponto central de integração entre os diversos microsserviços. Para armazenamento das informações de usuários, exames e dependentes/pacientes, o sistema adota o banco de dados **PostgreSQL**, garantindo confiabilidade e escalabilidade.

### 2.2 Visão de Alto Nível dos Componentes
- **Front-end**:
  - Desenvolvido com **React.js**, **TypeScript** e **styled components**, proporcionando uma interface amigável e responsiva.
- **Back-end**:
  - Arquitetura em **microsserviços** com **FastAPI** e **Python**, oferecendo flexibilidade, modularidade e alta performance.
- **Gateway**:
  - Funciona como um ponto central de integração entre os microsserviços do **back-end**, otimizando a comunicação e o roteamento de requisições.
- **Banco de Dados**:
  - **PostgreSQL** garante armazenamento seguro e confiável das informações do sistema, incluindo usuários, exames e dependentes/pacientes.
- **Ambiente de Produção**:
  - **Vercel** (front-end) e **Render** (back-end) garantem alta disponibilidade e escalabilidade da aplicação em produção.

## 3. Visão de Componentes
**Descrição dos Principais Repositórios do Sistema**

Para o desenvolvimento do projeto visando a arquitetura de **microsserviços** foi realizada a construção de 5 repositórios.

### 3.1 - Client-side
Esse é o repositório responsável pela camada de **front-end** do projeto. Todo nosso código relacionado a parte visual do sistema está agregado nesta camada. O código do repositório está sendo desenvolvido em **React** para maior escalabilidade e compatibilidade com o que se pretende alcançar com o projeto.

### 3.2 - User-service
É o repositório responsável pelo gerenciamento de **usuários**. Essa camada atende a todos os serviços relacionados ao gerenciamento de **pacientes, médicos e dependentes**, incluindo sua criação, consulta, alterações e exclusão lógica.

### 3.3 - Authentication
É a camada de micro serviço responsável pela parte de **validação de usuários**, todas as operações que necessitam da validação de acesso do usuário passam por esta camada.

### 3.4 - Data-processing-service
É o repositório responsável pela parte de **captação e processamento de dados**. Ele contempla os serviços associados aos formulários que o sistema irá utilizar para receber os dados da parte dos clientes e os serviços de processamento desses dados.

### 3.5 - Database
Por fim temos nosso repositório responsável pelo armazenamento e dockerização da nossa **base de dados**, esse repositório em si não possui nenhum micro serviço e é encarregado de manter a estrutura da nossa base de dados.

<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/44be9a16-8277-4800-86ff-1f3e51c7aaf6" width="600" height="400" />

## 4. Visão de Módulos
**Estrutura de Módulos e Pacotes**

- **Front-end**:
  - src/
    - components/
    - pages/
    - services/
    - utils/

- **Back-end**:
  - services/
    - users/
    - exams/
    - dependents/
    - gateway/

**Interface e Interações entre Módulos**

As páginas do **front-end** interagem com os componentes e serviços para realizar operações, enquanto os serviços do **back-end** interagem com os modelos de dados para acessar o banco de dados através do gateway.

## 5. Visão de Camadas
**Descrição das Diferentes Camadas da Arquitetura**

- **Camada de Apresentação (Front-end)**: Responsável pela interface com o usuário.
- **Camada de Aplicação (Back-end)**: Contém a lógica de negócios e **APIs RESTful** distribuídas em microsserviços.
- **Camada de Dados (Banco de Dados)**: Armazena as informações dos usuários, exames e dependentes/pacientes.

**Responsabilidades de Cada Camada**

- **Front-end**: Capturar e exibir dados para os usuários.
- **Back-end**: Processar a lógica de negócios e responder às solicitações do **front-end** via gateway.
- **Banco de Dados**: Persistir dados de forma segura e eficiente.

## 6. Visão de Dados
**Estrutura de Dados do Sistema**

<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/641a7b17-0ec7-4781-9c79-e958954bcf87" width="600" height="400" />

## 7. Visão de Implantação
**Ambientes de Implantação**

- **Produção**:
  - **Front-end** hospedado na **Vercel**.
  - **Back-end** hospedado na **Render**.
- **Testes e Desenvolvimento**: Utilizam ambientes locais e staging conforme necessário.

**Diagrama de Implantação**:

<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/20ff8a9b-19fe-4e9a-9086-9eb68ed069da" width="600" height="400" />

## 8. Visão de Execução
**Fluxos de Trabalho Principais**

### 8.1 - Fluxo de cadastro e login
<br/>
<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/d8e604df-2251-4c2b-89fa-67fd9b96b856" width="600" height="400" />

### 8.2 - Fluxo de submissão de exame
<br/>
<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/4b9b6615-26a5-4155-8c9d-2912447bfa67" />

### 8.3 - Fluxo de adição de dependentes/pacientes
<br/>
<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/9e90bb64-6e61-44e4-a070-cd2481c2a04a" />

## 9. Cenários de Uso

### Cenário de Uso 1: Cadastro de Usuário
<br/>
<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/105eebd1-191c-42d8-baa5-356a5c9ad48e" width="600" height="400" />

### Cenário de Uso 2: Submissão de Exame
<br/>
<img src="https://github.com/EPS-DataMed/client-side/assets/48137972/0f11ce89-6931-4379-af26-d2fec3bbaaea" width="600" height="400" />

## 10. Visão de Infraestrutura
**Descrição da Infraestrutura de Hardware e Software**

- **Front-end** utiliza **React.js**, **TypeScript** e **styled components**.
- **Back-end** utiliza **FastAPI**, **Python** e **pytest**.
- **Banco de dados** **PostgreSQL**.
- **Ambiente de produção** utiliza **Vercel** e **Render**.

**Ferramentas e Frameworks Utilizados**

- **Front-end**: **React.js**, **TypeScript**, **styled components**, **jest**.
- **Back-end**: **FastAPI**, **Python**, **pytest**.
- **Banco de Dados**: **PostgreSQL**.
- **Plataforma de Produção**: **Vercel**, **Render**.

## 11. Padrões e Convenções
**Padrões Arquitetônicos Utilizados**

- Arquitetura de **microsserviços** para o **back-end**.
- Componentização no **front-end** com **React**.

**Convenções de Codificação**

- Seguir padrões de codificação do **PEP 8** para **Python**.
- Utilizar **ESLint** e **Prettier** para manter a consistência do código no **front-end**.

## 12. Decisões Arquitetônicas
**Principais Decisões e Justificativas**

- Escolha de **React.js** e **TypeScript** para robustez e escalabilidade do **front-end**.
- Utilização de **FastAPI** e **Python** no **back-end** pela facilidade de desenvolvimento rápido e integração com bibliotecas de machine learning.
- Uso de **PostgreSQL** devido à sua robustez e suporte a transações complexas.
- Adoção de uma arquitetura de **microsserviços** para facilitar a escalabilidade e manutenção do sistema.

**Trade-offs Considerados**

- Escolha entre **FastAPI** e **Django**, optando por **FastAPI** pela performance e simplicidade.
- Escolha entre **PostgreSQL** e **MySQL**, optando por **PostgreSQL** pela melhor conformidade com **ACID**.

## 13. Segurança
**Mecanismos de Segurança Implementados**

- Autenticação baseada em **JWT**.
- Criptografia de senhas.
- Conexões **HTTPS** para comunicação segura.

**Políticas de Segurança**

- Políticas de controle de acesso baseadas em papéis (**RBAC**).
- Auditoria e logs de atividades.

## 14. Gerenciamento de Configuração

### 14.1 - Controle de Versão
O uso do **Git** como ferramenta de controle de versão para projetos de software, oferece simplicidade e flexibilidade no versionamento. Sua utilização estratégica aprimora o processo de desenvolvimento, garantindo qualidade e colaboração eficientes dentro da organização.

### 14.2 - Branching strategy com feature branches e pull requests
As **feature branches** servem como base para um desenvolvimento modular, permitindo que cada desenvolvedor trabalhe em funcionalidades ou correções de bugs de forma isolada, sem afetar a linha principal (**main branch**). Isso minimiza conflitos de código e garante a estabilidade do código principal.

As **pull requests** facilitam a revisão e integração das alterações na linha principal. Ao concluir o trabalho em sua ramificação de recurso, crie uma **pull request**. Isso notifica sua equipe sobre as alterações, permitindo a revisão do código antes da mesclagem.

### 14.3 - Revisões de código para todas as mudanças
Todas as alterações no código devem passar por revisões rigorosas por outros desenvolvedores antes da mesclagem na **main branch**. Isso ajuda a identificar e corrigir erros, detectar problemas de design e garantir a conformidade com os padrões de codificação. Esse processo robusto de gerenciamento de mudanças é crucial para garantir a qualidade e a estabilidade do código.

### 14.4- Testes automatizados para validação de alterações
São feitas a Implementação de testes automatizados abrangentes para validar as alterações no código. Isso garante que novas funcionalidades funcionem como esperado e que as correções de bugs resolvam os problemas sem introduzir novos.

## 15. Glossário
**Termos e Definições Relevantes**

- **JWT**: JSON Web Token, utilizado para autenticação.
- **RBAC**: Role-Based Access Control, controle de acesso baseado em papéis.
- **CRUD**: Create, Read, Update, Delete, operações básicas de banco de dados.
- **feature branches, pull requests**.

## Referências
- FOWLER, Martin. Patterns of Enterprise Application Architecture. Addison-Wesley, 2002. ISBN 978-0321127426.
- BASS, Len; CLEMENTS, Paul; KAZMAN, Rick. Software Architecture in Practice. Addison-Wesley, 2012. ISBN 978-0321815736.
- CLEMENTS, Paul et al. Documenting Software Architectures: Views and Beyond. Addison-Wesley, 2010. ISBN 978-0321552686.
- ROZANSKI, Nick; WOODS, Eóin. Software Systems Architecture: Working With Stakeholders Using Viewpoints and Perspectives. Addison-Wesley, 2011. ISBN 978-0321718334.
- ALBIN, Stephen T. The Art of Software Architecture: Design Methods and Techniques. Wiley, 2003. ISBN 978-0471267734.
