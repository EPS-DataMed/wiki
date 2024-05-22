# Relatório: Desenvolvimento de um Sistema para Processamento de Dados Médicos a partir de Arquivos PDF e Integração com Formulário React

## Objetivo
O objetivo deste relatório é apresentar as ideias iniciais do estudo e pesquisa que vão nos permitir desenvolver um sistema que permita aos usuários enviar arquivos PDF contendo informações médicas de pacientes, extrair esses dados dos arquivos PDF, armazená-los em um banco de dados PostgreSQL e, em seguida, exibi-los dinamicamente em um formulário desenvolvido com React. Este relatório detalha as ideias, possibilidades e passos para alcançar esse objetivo. Ele se estrutura em ideias de uma pesquisa inicial, tudo aqui será debatido e avaliado em reuniões em grupo documentadas no projeto, a fim de encontrar o melhor caminho para o desenvolvimento desta ação.

## Visão Geral
O sistema é mais complexo do que o relatado aqui, mas de maneira geral e para simplificar para esta parte do estudo e do desenvolvimento, vamos ter a visão que o sistema será composto por duas partes principais: uma API em Python para processamento de dados e integração com o banco de dados, e um frontend desenvolvido com React para exibir os dados em um formulário amigável para o usuário.

## Detalhes Técnicos

### API em Python
- Possibilidades de frameworks utilizados para desenvolvimento da API, são o: FastAPI, Flask e Django para desenvolver a API. Estes em um primeiro momento de estudo e pesquisa parecem possuir mais recursos e o desempenho necessário, para que possamos processar dados, além de serem mais flexíveis para a integração geral do projeto.
- A API será responsável por receber os arquivos PDF dos usuários, processá-los para extrair informações médicas relevantes e armazená-los no banco de dados PostgreSQL.
- Existem algumas bibliotecas como pdfplumber que podem ser usadas para processar os arquivos PDF (PyPDF2, pdfminer, Tabula-py), exigindo um estudo mais aprofundado dessa parte, para definir em grupo o caminho a ser tomado, referente a integração com o banco de dados PostgreSQL a psycopg2 parece ser a mais viável.
- A API deve ser projetada como uma API RESTful, fornecendo endpoints para receber arquivos PDF, extrair dados e fornecer esses dados em um formato JSON.

### Frontend com React
- Desenvolver um formulário usando React para exibir os dados médicos dos pacientes.
- O formulário permitirá aos usuários visualizar e interagir com os dados médicos, como nome do paciente, idade, diagnósticos, etc.
- Fazer uso de componentes controlados no React para vincular os dados recebidos da API aos campos de entrada do formulário.
- Usar requisições HTTP para se comunicar com a API em Python e obter os dados dos pacientes.

## Passos para Implementação
1. **Análise de Requisitos:** ✅
   - Identificar os requisitos detalhados do sistema, incluindo os tipos de informações médicas a serem extraídas dos arquivos PDF e os campos do formulário React.
2. **Desenvolvimento da API em Python:** 💻⏳
   - Configurar o ambiente de desenvolvimento Python com as bibliotecas necessárias.
   - Implementar os endpoints da API para receber arquivos PDF, extrair dados e interagir com o banco de dados PostgreSQL.
3. **Configuração do Banco de Dados:** 💻⏳
   - Criar o esquema do banco de dados PostgreSQL para armazenar os dados médicos dos pacientes.
4. **Desenvolvimento do Frontend com React:** 💻⏳
   - Configurar o ambiente de desenvolvimento React.
   - Criar os componentes de formulário React para exibir os dados médicos dos pacientes.
   - Implementar a lógica para fazer requisições à API e exibir os dados no formulário.
5. **Testes e Depuração:** ⏳
   - Realizar testes unitários e de integração para garantir a funcionalidade adequada do sistema.
   - Depurar quaisquer problemas encontrados durante o teste.
6. **Implantação:** ⏳
   - Implantação da aplicação em um ambiente de produção, garantindo escalabilidade e segurança.

## Considerações Finais
Este relatório detalha uma das possíveis abordagens para desenvolver um sistema para processamento de dados médicos a partir de arquivos PDF e integração com um formulário React. A combinação de uma API em Python para processamento de dados e um frontend React para interação com o usuário fornecerá uma solução eficaz e amigável para o gerenciamento de informações médicas dos pacientes. Mas ainda existem alguns detalhes importantes que precisam ser levados em consideração, como a robustez do sistema, a escalabilidade e a segurança. Além desta não ser a única opção viável, podendo e possivelmente sendo implementado em conjunto com outras opções, técnicas (OCR (Reconhecimento Óptico de Caracteres), Processamento de Linguagem Natural (NLP), Aprendizado de Máquina, Serviços de Processamento de Documentos em Nuvem). Todos os dados e informações aqui não são uma definição, mas ideias que serão levantadas e documentadas em discussões em grupo.

## Fontes
- Klippa Blog. "Extraindo dados de documentos PDF." Disponível em: [https://www.klippa.com/pt/blog/informacao/extrair-dados-documentos-pdf/](https://www.klippa.com/pt/blog/informacao/extrair-dados-documentos-pdf/)
- YouTube. "Extraindo dados de PDF com Python." Disponível em: [https://www.youtube.com/watch?v=x9IDL8eruAw](https://www.youtube.com/watch?v=x9IDL8eruAw)
