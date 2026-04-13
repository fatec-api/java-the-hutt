# **Controle de Apontamento de Horas - Java the Hutt**

Projeto desenvolvido pela equipe Java the Hutt do 3º semestre de Desenvolvimento de Software Multiplataforma da FATEC de São José dos Campos, no contexto da metodologia de ensino Aprendizagem por Projetos Integrados (API), em parceria com a GSW.

---
<div align="center">
    
[A Dor do Cliente](#a-dor) | 
[A Solução para o Cliente](#a-solucao) |
[O Desafio](#o-desafio) | 
[Backlog de Produto](#backlog-de-produto) | 
[DoR e DoD](#dor-e-dod) | 
[Cronograma de Evolução do Projeto](assets/sprint-1/cronograma-evolucao.png) | 
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
<a id="a-dor"></a>
## 🎯 A Dor do Cliente
A GSW Software (líder em TI, +520 profissionais) sofre com um gargalo crítico de gestão. Segundo o stakeholder Diego Miranda, o atual sistema de apontamento de horas tornou-se obsoleto, apresentando lentidão e falhas de integração.

No entanto, a dor principal é a cegueira de dados. Com equipes distribuídas por todo o Brasil (de Manaus ao RS), a ferramenta não fornece insights para que a diretoria e o financeiro consigam responder a questões vitais:

Por que o time de desenvolvimento não está performando?

Onde estamos falhando nas entregas?

Onde podemos alocar recursos para melhorar a situação do time?

Impacto: Sem visibilidade sobre a produtividade e a alocação de horas, a empresa sofre com relatórios imprecisos, queda na qualidade dos projetos, perda de contratos e prejuízo financeiro direto.

---
<a id="a-solucao"></a>
## 🚀 A Solução para o Cliente

Dado o curto prazo do projeto de 3 meses e a complexidade de integrar todos os relatórios financeiros e operacionais, a estratégia adotada **não é resolver tudo de uma vez**, mas sim atacar o principal ponto de dor: **a falta de visibilidade sobre a performance das equipes**.  

Em vez de tentar consolidar toda a visão financeira, a solução gera **insights acionáveis sobre produtividade, atrasos e eficiência das entregas**.

### Dados que serão utilizados:
- Logs de mudança de status das tarefas  
- Esforço registrado por profissional  
- Estimativa de tempo por tarefa  
- Tipo ou categoria das tarefas  
- Responsáveis pela documentação das tarefas  

### O que a solução entrega:

1. **Identificação de atrasos por profissional**  
   Permite saber quais profissionais apresentam maior taxa de atraso.  
   **A partir de:** Consulta de Projetos (US07)

2. **Tarefas que demandam mais tempo que o esperado**  
   Permite identificar gargalos por tipo de tarefa e ajustar processos.  
   **A partir de:** Acompanhamento de Atividades e Itens (US08)

3. **Associação de analistas a tarefas críticas**  
   Entende quais analistas estão ligados às tarefas com maior atraso, permitindo decisões de realocação.  
   **A partir de:** Análise de Capacidade Produtiva (US09)

4. **Exportação e análise de apontamentos**  
   Visualização e exportação de dados para CSV, possibilitando análises complementares.  
   **A partir de:** Histórico de Alterações (US10)

5. **Monitoramento do orçamento do projeto**  
   Comparação entre orçamento real e previsto, garantindo controle financeiro eficiente.  
   **A partir de:** Monitoramento de Custo Real por Projeto (US12)
   
---
<a id="o-desafio"></a>
## 🧩 O Desafio Proposto aos Alunos
O sistema de Controle de Apontamento de Horas tem como objetivo centralizar e organizar o registro de horas trabalhadas em projetos, substituindo planilhas e controles dispersos que geram inconsistências e retrabalho. A proposta é oferecer maior visibilidade sobre esforço, custos e base de cobrança, garantindo informações confiáveis para tomada de decisão.

A solução será uma aplicação web com back-end em microserviços e APIs REST e front-end em single-page application, permitindo apontamentos por atividade, com diferentes regras de custo e faturamento por projeto, profissional ou tipo de atividade. O foco é unir flexibilidade nas regras com simplicidade no uso e relatórios claros.

---
<a id="backlog-de-produto"></a>
## 📋 Backlog de Produto

| Rank	| Prioridade | User Stories | Estimativa (Pontos) | Sprint |
| --- | --- | --- | --- | --- |
| 01 | Alta | Como gestor, quero inserir as informações dos profissionais para poder alocá-los em projetos futuros e calcular o custo interno | 5 | 1 |
| 02 | Alta | Como gestor, quero criar novos projetos para que as frentes de trabalho sejam centralizadas e fiquem disponíveis para o lançamento de horas dos profissionais | 3 | 1 |
| 03 | Alta | Como gestor, quero alocar profissionais aos projetos para que eles possam visualizar suas atividades e itens e o sistema calcule a rentabilidade do projeto | 3 | 1 |
| 04 | Alta | Como gestor, quero criar/inserir um item e atividade que será utilizada em um projeto para descrever a tarefa que o profissional realizará e poder atribuir um responsável | 3 | 1 |
| 05 | Alta | Como gestor, quero atribuir um item e atividade ao profissional alocado em um projeto para que ele visualize suas atividades e possa realizar o apontamento de horas | 3 | 1 |
| 06 | Alta | Como profissional, quero realizar o apontamento de horas diário/semanal selecionando os itens e atividades em que trabalhei para registrar meu esforço com precisão | 8 | 1 |
| 07 | Alta | Como gestor, quero revisar, aprovar ou reprovar os apontamentos e acessar o histórico de alterações para garantir que os apontamentos estejam corretos, o faturamento seja justo e os dados sejam auditáveis. | 8 | 2 |
| 08 | Alta | Como gestor, quero visualizar as atividades e itens realizados em um projeto para acompanhar o progresso comparando esforço planejado vs realizado, evidenciando os itens que estão frequentemente atrasadas | 3 | 2 |
| 09 | Alta | Como gestor, quero visualizar a relação entre itens entregues e horas apontadas para analisar qualidade das descrições dos analistas para os itens e a capacidade produtiva dos profissionais. | 5 | 2 |
| 10 | Média | Como gestor, quero visualizar os projetos existentes para acompanhar o consumo de horas dos profissionais, esforço e o andamento das atividades em tempo real | 3 | 2 |
| 11 | Média | Como gestor, quero visualizar a lista de profissionais existentes para saber em quais projetos participam e poder alocá-los de forma estratégica (ex.: especialidade) | 5 | 2 |
| 12 | Média | Como gestor, quero alterar os dados dos profissionais para manter informações e valores atualizados| 5 | 2 |
| 13 | Média | Como financeiro, quero acompanhar o custo real acumulado dos profissionais por projeto para comparar com o orçamento previsto | 5 | 3 |
| 14 | Baixa | Como financeiro, quero visualizar o comparativo entre custo acumulado dos profissionais e valor a ser faturado por projeto para monitorar a rentabilidade | 5 | 3 |
| 15 | Baixa | Como gestor, quero alterar projetos para garantir que as regras de cobrança e custo estejam sempre atualizadas | 5 | 3 |
| 16 | Baixa | Como gestor, quero cadastrar e gerenciar clientes para poder vincular futuros projetos e garantir que as informações de faturamento estejam corretas | 5 | 3 |
| 17 | Baixa | Como gestor, quero visualizar os clientes ativos para poder vinculá-los a novos projetos e garantir a integridade dos relatórios | 3 | 3 |
| 18 | Baixa | Como administrativo, quero alterar as informações dos clientes para manter os dados atualizados e garantir comunicação efetiva | 3 | 3 |
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
| 1 | 16/03/2026 - 05/04/2026 | [Ver Documentação](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?tab=t.zcrpwsovs9pd#heading=h.ec1c7t75nhkv) | <div align="center">[Ver Vídeo](assets/sprint-1/api3dsm-sprint1.gif)</div> | ✅ Concluído |
| 2 | 13/04/2026 - 03/05/2026 | [Ver Documentação](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?tab=t.g2owc95xwzh9) | <div align="center">[Ver Vídeo]()</div> | Em Andamento |
| 3 | 11/05/2026 - 31/05/2026 | [Ver Documentação](/documents/sprint-3/README.md) | <div align="center">[Ver Vídeo]()</div> | ⏳ Pendente |

---
<a id="tecnologias-utilizadas"></a>
## 💻 Tecnologias Utilizadas

### 🎨 Frontend
<p>
<img src="https://cdn.simpleicons.org/html5/E34F26" height="32"/>
<img src="https://cdn.simpleicons.org/css/1572B6" height="32"/>
<img src="https://cdn.simpleicons.org/javascript/F7DF1E" height="32"/>
<img src="https://cdn.simpleicons.org/typescript/3178C6" height="32"/>
<img src="https://cdn.simpleicons.org/react/61DAFB" height="32"/>
<img src="https://cdn.simpleicons.org/tailwindcss/06B6D4" height="32"/>
<img src="https://cdn.simpleicons.org/daisyui/5A0EF8" height="32"/>
<img src="https://cdn.simpleicons.org/nodedotjs/339933" height="32"/>
</p>

### ⚙️ Backend & Dados
<p>
<img src="https://cdn.simpleicons.org/openjdk/ED8B00" height="32"/>  <!-- Java -->
<img src="https://cdn.simpleicons.org/spring/6DB33F" height="31"/> <!-- Spring Boot -->
<img src="https://cdn.simpleicons.org/mysql/4479A1" height="31"/>  <!-- MySQL -->
<!-- <img src="https://cdn.simpleicons.org/docker/2496ED" height="31"/> <!-- Docker -->
<!-- Insomnia -->
<a href="https://insomnia.rest/">
  <img src="https://insomnia.rest/images/insomnia-logo.svg" height="31" alt="Insomnia"/>
</a>
<!-- <img src="https://cdn.simpleicons.org/swagger/85EA2D" height="32"/> <!-- Swagger --> 
</p>

### 🛠️ Ferramentas & DevOps
<p>
<img src="https://cdn.simpleicons.org/git/F05032" height="32"/> <!-- Git -->
<img src="https://cdn.simpleicons.org/github/4B4B4B" height="32"/> <!-- GitHub -->
<img src="https://cdn.simpleicons.org/jira/0052CC" height="32"/> <!-- Jira -->
<img src="https://cdn.simpleicons.org/excalidraw/6965DB" height="32"/> <!-- Excalidraw -->
<img src="https://www.gstatic.com/images/branding/product/1x/docs_2020q4_48dp.png" height="32"/> <!-- Google Docs -->
<img src="https://cdn-icons-png.flaticon.com/512/2111/2111370.png" height="32"/><!-- Discord -->
    <!-- VS Code -->
<a href="https://code.visualstudio.com/">
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" height="32" height="31" alt="VS Code"/>
</a>

<!-- IntelliJ IDEA -->
<a href="https://www.jetbrains.com/idea/">
  <img src="https://resources.jetbrains.com/storage/products/intellij-idea/img/meta/intellij-idea_logo_300x300.png" height="31" alt="IntelliJ IDEA"/>
</a>
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

A estrutura de pastas do projeto (backend e frontend) ainda será definida conforme a evolução da arquitetura da aplicação e a organização dos módulos durante a primeira sprint.
```
java-the-hut
│
├── 📁 backend/        → API REST (Spring Boot)
│   └── 📁 src/
│       └── 📁 main/
│           └── 📁 java/
│               └── 📁 com/
│                   └── 📁 example/
│                       └── 📁 App/
│                           │
│                           ├── 📁 Controller          → Camada responsável por expor os endpoints da API
│                           │
│                           ├── 📁 Dto                 → Objetos de transferência de dados
│                           │   ├── 📁 Request         → DTOs utilizados para receber dados das requisições
│                           │   └── 📁 Response        → DTOs utilizados para retornar dados nas respostas
│                           │
│                           ├── 📁 Exception           → Tratamento de exceções da aplicação
│                           │
│                           ├── 📁 Mapper              → Conversão entre Model e DTO
│                           │
│                           ├── 📁 Model               → Entidades do domínio e mapeamento com o banco de dados
│                           │
│                           ├── 📁 Repository          → Interfaces de acesso ao banco de dados (Spring Data)
│                           │
│                           ├── 📁 Security            → Configurações de autenticação e autorização
│                           │
│                           └── 📁 Service             → Regras de negócio da aplicação
│
└── 📁 frontend/       → Aplicação Web
    └── 📁 src/        → Código-fonte do frontend
        ├── 📁 api/           → Serviços de API, instâncias e chamadas HTTP (ex: AllocationService.tsx, instance.ts)
        ├── 📁 assets/        → Arquivos estáticos (imagens, ícones, gifs)
        ├── 📁 auth/          → Funcionalidades de autenticação
        │   ├── components/   → Componentes específicos de auth
        │   ├── hooks/        → Hooks relacionados a auth
        │   ├── services/     → Serviços internos de auth
        │   └── utils/        → Funções auxiliares de auth
        ├── 📁 components/    → Componentes reutilizáveis em toda a aplicação (modais, formulários, tabelas)
        ├── 📁 contexts/      → Context API / gerenciamento de estado global
        ├── 📁 pages/         → Páginas principais da aplicação (cada tela é um arquivo .tsx)
        ├── 📁 features/      → Módulos de funcionalidades específicas
        │   ├── 📁 Auth/      → Funcionalidades de login, logout e registro
        │   └── 📁 Dashboard/ → Funcionalidades do painel de controle
        ├── 📁 hooks/         → Hooks customizados para lógica compartilhada
        ├── 📁 services/      → Comunicação com a API para CRUD de usuários, projetos, clientes e apontamentos
        ├── 📁 types/         → Tipagens e interfaces TypeScript
        ├── 📁 utils/         → Funções utilitárias (helpers)
        ├── 📁 styles/        → Estilos globais e variáveis de design
        ├── App.tsx           → Componente raiz da aplicação
        └── index.tsx         → Ponto de entrada da aplicação
 ```

## Próximos Passos – Estratégia de Microsserviços

Na primeira sprint, o sistema é monolítico para validar rapidamente as regras de negócio. Nas próximas sprints, será dividido em microsserviços independentes, com responsabilidades isoladas, comunicação via API e bancos próprios. Para mais detalhes, consulte o [Documento de Estratégia de Microsserviços](https://docs.google.com/document/d/1Z_DbshfP_fMyZPNkN-YQ0DQifeGzecKMofmZY3EVt1E/edit?tab=t.gj1c16m9heoa).
.

---
<a id="manual-do-usuario"></a>
## 📜 Manual do Usuário

**:link: Clique no link abaixo para visualizar o Manual do Usuário:**  
> [Manual do Usuário](https://docs.google.com/document/d/12I-0IGaLOCsu6-cSiFregg8mHEq8kEv9FhEO5Tt4_ec/edit?usp=sharing)

---

<a id="manual-de-instalacao"></a>
## 📖 Manual de Instalação


Abaixo está a estrutura prevista para execução local da aplicação.

### 🔧 Pré-requisitos

Antes de iniciar, será necessário ter instalado:

- Java JDK 21 ou superior
- Maven
- Node.js
- MySQL
- Git
- Variáveis de ambiente configuradas para acesso ao banco

### 🌀 Clonando o repositório

```bash
git clone https://github.com/fatec-api/java-the-hut.git
cd java-the-hut
git submodule init
git submodule update
```

---
## ⚙️ Configuração do Backend (Spring MVC)

Passos previstos:

1. Acessar a pasta do backend
```bash
cd api-3dsm-backend
```

2. Configurar variáveis de ambiente no arquivo:
```
application.properties

spring.application.name=App

# ======================
# MySQL (ATIVO)
# ======================
spring.datasource.url=jdbc:mysql://localhost:3306/gsw_api?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=SUA_SENHA_AQUI
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# ======================
# JPA / Hibernate
# ======================
spring.jpa.hibernate.ddl-auto=update
spring.session.jdbc.initialize-schema=always
```
(credenciais do banco, porta do servidor, etc.)

3. Executar o projeto via Maven ou Gradle
```bash
mvn spring-boot:run
```

A API deverá rodar em:
```
http://localhost:8080
```

---

## ⚙️ Configuração do Frontend (React + TypeScript)

1. Acessar a pasta do frontend
```bash
cd api-3dsm-frontend
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
