# **Controle de Apontamento de Horas - Java the Hutt**

Projeto desenvolvido pela equipe Java the Hutt do 3º semestre de Desenvolvimento de Software Multiplataforma da FATEC de São José dos Campos, no contexto da metodologia de ensino Aprendizagem por Projetos Integrados (API), em parceria com a GSW.

---
<div align="center">

[O Desafio](#o-desafio) | 
[Backlog de Produto](#backlog-de-produto) | 
[DoR e DoD](#dor-e-dod) | 
[Cronograma de Evolução do Projeto](assets/sprint-1/cronograma-evolucao.jpg) | 
[Sprints](#sprints) | 
[Tecnologias Utilizadas](#tecnologias-utilizadas) |
[Estratégia de Branchs e Padrão de Commits](#padrao-de-commits) |
[Estrutura do Projeto](#estrutura-do-projeto) | 
[Manual do Usuário](#manual-do-usuario) | 
[Manual de Instalação](#manual-de-instalacao) | 
[Documentação](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?usp=sharing) | 
[Equipe](#autores) |

</div>

---
<a id="o-desafio"></a>
## 🧩 O Desafio
O sistema de Controle de Apontamento de Horas tem como objetivo centralizar e organizar o registro de horas trabalhadas em projetos, substituindo planilhas e controles dispersos que geram inconsistências e retrabalho. A proposta é oferecer maior visibilidade sobre esforço, custos e base de cobrança, garantindo informações confiáveis para tomada de decisão.

A solução será uma aplicação web com back-end em microserviços e APIs REST e front-end em single-page application, permitindo apontamentos por atividade, com diferentes regras de custo e faturamento por projeto, profissional ou tipo de atividade. O foco é unir flexibilidade nas regras com simplicidade no uso e relatórios claros.

---
<a id="backlog-de-produto"></a>
## 📋 Backlog de Produto

🚧 Em elaboração  
O backlog do produto encontra-se atualmente em fase de definição e priorização das funcionalidades.

| Rank	| Prioridade | User Stories | Estimativa (Pontos) | Sprint |
| --- | --- | --- | --- | --- |
| 01 | Alta | Como gestor, quero inserir as informações dos profissionais para poder alocá-los em projetos futuros e calcular o custo interno | 5 | 1 |
| 02 | Alta | Como gestor, quero criar novos projetos para que as frentes de trabalho sejam centralizadas e fiquem disponíveis para o lançamento de horas dos profissionais | 3 | 1 |
| 03 | Alta | Como gestor, quero alocar profissionais aos projetos para que eles possam visualizar suas atividades e itens e o sistema calcule a rentabilidade do projeto | 3 | 1 |
| 04 | Alta | Como gestor, quero criar/inserir um item e atividade que será utilizada em um projeto para descrever a tarefa que o profissional realizará e poder atribuir um responsável | 3 | 1 |
| 05 | Alta | Como gestor, quero atribuir um item e atividade ao profissional alocado em um projeto para que ele visualize suas atividades e possa realizar o apontamento de horas | 3 | 1 |
| 06 | Alta | Como profissional, quero realizar o apontamento de horas diário/semanal selecionando os itens e atividades em que trabalhei para registrar meu esforço com precisão | 8 | 1 |
| 07 | Alta | Como gestor, quero cadastrar e gerenciar clientes para poder vincular futuros projetos e garantir que as informações de faturamento estejam corretas | 3 | 1 |
| 08 | Alta | Como gestor, quero visualizar os clientes ativos para poder vinculá-los a novos projetos e garantir a integridade dos relatórios | 2 | 1 |
| 09 | Alta | Como gestor, quero visualizar a lista de profissionais existentes para saber em quais projetos participam e poder alocá-los de forma estratégica (ex.: especialidade) | 5 | 2 |
| 10 | Alta | Como gestor, quero visualizar os projetos existentes para acompanhar o consumo de horas, esforço e o andamento das atividades em tempo real | 3 | 2 |
| 11 | Alta | Como gestor, quero visualizar as atividades e itens realizados em um projeto para acompanhar o progresso comparando esforço planejado vs realizado | 5 | 2 |
| 12 | Alta | Como gestor, quero visualizar a relação entre itens entregues e horas apontadas para analisar a capacidade produtiva e ajustar estratégias | 5 | 2 |
| 13 | Alta | Como administrador, quero acessar o histórico de alterações dos lançamentos para garantir rastreabilidade e transparência dos dados | 5 | 2 |
| 14 | Alta | Como gestor, quero visualizar o relatório de rentabilidade por projeto para identificar contratos lucrativos ou com excesso de custo | 5 | 3 |
| 15 | Alta | Como financeiro, quero acompanhar o custo real acumulado dos profissionais por projeto para comparar com o orçamento previsto | 5 | 3 |
| 16 | Média | Como financeiro, quero visualizar o comparativo entre custo acumulado dos profissionais e valor a ser faturado por projeto para monitorar a rentabilidade | 5 | 3 |
| 17 | Média | Como gestor, quero alterar projetos para garantir que as regras de cobrança e custo estejam sempre atualizadas | 3 | 3 |
| 18 | Média | Como gestor, quero alterar os dados dos profissionais para manter informações e valores atualizados | 3 | 3 |
| 19 | Média | Como administrativo, quero alterar as informações dos clientes para manter os dados atualizados e garantir comunicação efetiva | 3 | 3 |
---

<a id="dor-e-dod"></a>
## 📍 DoR (Definition of Ready) and DoD (Definition of Done)
**:link: Clique no link abaixo para visualizar o DoR e DoD do projeto:**  
> [Definition of Ready and Done](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?tab=t.0)

---
<a id="sprints"></a>
## 👟 Sprints
| Sprint | Período | Documentação | Vídeo do Incremento | Status |
|---|---|---|---|---|
| 1 | 16/03/2026 - 05/04/2026 | [Ver Documentação](/documents/sprint-1/README.md) | <div align="center">[Ver Vídeo]()</div> | ⏳ Pendente |
| 2 | 13/04/2026 - 03/05/2026 | [Ver Documentação](/documents/sprint-2/README.md) | <div align="center">[Ver Vídeo]()</div> | ⏳ Pendente |
| 3 | 11/05/2026 - 31/05/2026 | [Ver Documentação](/documents/sprint-3/README.md) | <div align="center">[Ver Vídeo]()</div> | ⏳ Pendente |

---
<a id="tecnologias-utilizadas"></a>
## 💻 Tecnologias Utilizadas
⚠️ *Nota: Algumas tecnologias estão em fase de validação arquitetural e podem sofrer alterações.*

### 🎨 Frontend
<p>
<img src="https://cdn.simpleicons.org/html5/E34F26" height="32"/>
<img src="https://cdn.simpleicons.org/css/1572B6" height="32"/>
<img src="https://cdn.simpleicons.org/javascript/F7DF1E" height="32"/>
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="32"/>
<img src="https://cdn.simpleicons.org/react/61DAFB" height="32"/>
<img src="https://cdn.simpleicons.org/tailwindcss/06B6D4" height="32"/>
<img src="https://cdn.simpleicons.org/daisyui/5A0EF8" height="32"/>
</p>

### ⚙️ Backend & Dados
<p>
<img src="https://cdn.simpleicons.org/openjdk/ED8B00" height="32"/>
<img src="https://cdn.simpleicons.org/spring/6DB33F" height="31"/>
<img src="https://cdn.simpleicons.org/nodedotjs/339933" height="32"/>
<img src="https://cdn.simpleicons.org/mysql/4479A1" height="31"/>
<img src="https://cdn.simpleicons.org/mongodb/47A248" height="33"/>
<!-- Este é um comentário em Markdown -->
</p>

### 🛠️ Ferramentas & DevOps
<p>
<img src="https://cdn.simpleicons.org/git/F05032" height="32"/>
<img src="https://cdn.simpleicons.org/jira/0052CC" height="32"/>
<img src="https://cdn.simpleicons.org/excalidraw/6965DB" height="32"/>
<img src="https://cdn.simpleicons.org/swagger/85EA2D" height="32"/>
</p>

---
<a id="padrao-de-commits"></a>
## 🌿 Estratégia de Branch e 📝 Padrão de Commits

O projeto adota uma estratégia de versionamento inspirada no **Git Flow**, utilizando o sistema de controle de versão **Git**. 

Além disso, seguimos um padrão de commits para garantir maior rastreabilidade das atividades, facilitar a colaboração entre os membros da equipe e manter o histórico do projeto organizado ao longo do desenvolvimento.

**🔗 Clique no link abaixo para visualizar o guia completo de Padrão de Commits e Estratégia de Branch:** 
> [Padronização de Branches e Commits](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?tab=t.qq5zpzvc7izx0)

---
<a id="estrutura-do-projeto"></a>
## 🗂️ Estrutura do Projeto

🚧 **Pendente – Em definição**

A estrutura de pastas do projeto (backend e frontend) ainda será definida conforme a evolução da arquitetura da aplicação e a organização dos módulos durante a primeira sprint.
```
│
├── 📁 backend/
│
├── 📁 frontend/
│   └── 📁 src/
│       ├── 📁 assets/
│       ├── 📁 components/
│       ├── 📁 pages/
│       ├── 📁 features/
│       │   ├── 📁 Auth/
│       │   └── 📁 Dashboard/
│       ├── 📁 hooks/
│       ├── 📁 context/
│       ├── 📁 services/
│       ├── 📁 types/
│       ├── 📁 utils/
│       ├── 📁 styles/
│       ├── App.tsx
│       └── index.tsx
│
 ```

---
<a id="manual-do-usuario"></a>
## 📜 Manual do Usuário

🚧 **Pendente**
**:link: Clique no link abaixo para visualizar o Manual do Usuário:**  
> [Manual do Usuário](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?tab=t.16hfhaca36s0)

---

<a id="manual-de-instalacao"></a>
## 📖 Manual de Instalação

🚧 **Em definição – As instruções detalhadas serão atualizadas conforme a implementação do projeto.**

Abaixo está a estrutura prevista para execução local da aplicação.

### 🔧 Pré-requisitos

Antes de iniciar, será necessário ter instalado:

- Java (JDK 17 ou superior)
- Maven
- Node.js
- Banco de Dados relacional
- Git

### 🌀 Clonando o repositório

```bash
git clone https://github.com/fatec-api/java-the-hut.git
cd java-the-hut
```

---

## ⚙️ Configuração do Backend (Spring MVC)

🚧 **Pendente – Configuração será detalhada após definição final da estrutura do projeto.**

Passos previstos:

1. Acessar a pasta do backend
```bash
cd backend
```

2. Configurar variáveis de ambiente no arquivo:
```
application.properties
```
(credenciais do banco, porta do servidor, etc.)

3. Executar o projeto via Maven ou Gradle
```bash
mvn spring-boot:run
```
ou
```bash
./gradlew bootRun
```

A API deverá rodar em:
```
http://localhost:8080
```

---

## ⚙️ Configuração do Frontend (React + TypeScript)

🚧 **Pendente – Configuração será detalhada após definição final da estrutura do projeto.**

1. Acessar a pasta do frontend
```bash
cd frontend
```

2. Instalar dependências
```bash
npm install
```

3. Executar o projeto
```bash
npm run dev
```

A aplicação deverá rodar em:
```
http://localhost:5173
```

---

<a id="autores"></a>
## 👨‍💻 Autores

| Nome      | Função          | Redes Sociais |
|-----------|-----------------|---------------|
| Ana Elize Graciano | Product Owner | <a href="https://github.com/Ane-Graciano"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/ana-elize-graciano-107448359/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| João Vitor Silva Correa Siqueira | Scrum Master | <a href="https://github.com/kakashinho"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/joao-vitor-siqueira-a2a2a3227/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Gabriel Kodato Faria | Desenvolvedor | <a href="https://github.com/Kodatoo"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/gabriel-kodato-b745742b8/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Gustavo Ribeiro da Rosa | Desenvolvedor | <a href="https://github.com/gustasvos"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/gustavo-rosa-46a251180/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Kaique Henrique Silva Pinto | Desenvolvedor | <a href="https://github.com/kaiquehsp"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/kaiquehenrique"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Laís Zanardi Inocêncio | Desenvolvedora | <a href="https://github.com/lais-zanardi"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/lais-zanardi-inocencio/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Lucas Inácio de Carvalho | Desenvolvedor | <a href="https://github.com/Lukitta013"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/lucas-in%C3%A1cio-6aa3ba29a/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Maria Fernanda de Oliveira Laboissiere | Desenvolvedora | <a href="https://github.com/mariaflbss"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a> <a href="https://www.linkedin.com/in/maria-fernanda-laboissiere-25362b353/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
| Rebeca Lima Nunes | Desenvolvedora | <a href="https://github.com/rebeca-lima-ti"><img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub"></a>  <a href="[https://www.linkedin.com/in/maria-fernanda-laboissiere-25362b353/](https://www.linkedin.com/in/rebeca-lima-925611359/)"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a> |
