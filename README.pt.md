<h1 align="center">Oii, eu me chamo Patrick!</h1>

<p align="center">
  <b>Desenvolvedor Back-end · Java/Spring & C#/.NET · Python · Estudante de Análise e Desenvolvimento de Sistemas</b>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/kau%C3%AApatrickgodoi/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:kauepatrickbrito@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

<p align="center">
  <a href="https://github.com/patrick-0990/patrick-0990/blob/main/README.md">🇺🇸 Read in English</a>
</p>

---

## Sobre mim

Sou desenvolvedor back-end e trabalho construindo plataformas internas de automação e CRMs para as áreas jurídica e financeira, com **Java/Spring Boot** e **C#/.NET**.

Se tem algo que me encanta na computação, são duas coisas: **arquitetura de software** e **algoritmos**. Gosto de entender por que uma solução escala, por que ela é a escolha certa para aquele contexto e como organizar um sistema para que ele continue simples de evoluir. No dia a dia, isso aparece no trabalho com concorrência, filas, processamento assíncrono e integrações resilientes.

Atualmente curso Análise e Desenvolvimento de Sistemas e estou aprofundando meus estudos em **system design** e **inteligência artificial**.

<details>
<summary><b>Arquitetura e design patterns</b></summary>

<br>

Tenho uma base sólida em design patterns: conheço bem os padrões criacionais, estruturais e comportamentais, como Factory, Builder, Adapter e Template Method, e já apliquei vários deles em produção, como Strategy, Specification e Observer (eventos de domínio), além de padrões de resiliência como Circuit Breaker e Bulkhead.

Também possuo uma boa bagagem em arquitetura de software: já implementei projetos com Clean Architecture, DDD, CQRS e Arquitetura Hexagonal (o famoso Ports & Adapters).

</details>

<details>
<summary><b>O que já construí profissionalmente</b></summary>

<br>

> Projetos proprietários (desenvolvidos na empresa em que trabalho): descrevo as soluções de forma genérica, sem código.

- **Orquestração de workflow**: pipeline assíncrono com mais de 10 etapas sequenciais modelado como máquina de estados, usando Strategy Pattern (novas etapas entram sem alterar o orquestrador), rastreio de jobs, retry e proteção contra execução duplicada. *O maior desafio aqui foi modelar os estados e entender as regras de domínio por trás de cada rotina.*

- **IA aplicada**: análise e resumo de documentos com LLM usando saída estruturada (JSON Schema), chat com contexto plugável por assunto e controle de custo de tokens por funcionalidade.

- **Concorrência**: locks de domínio, locking pessimista e otimista, executores dedicados e fan-out com `CompletableFuture`; fila persistente em PostgreSQL com `FOR UPDATE SKIP LOCKED` e graceful shutdown dos workers.

- **Resiliência em integrações**: circuit breaker, bulkhead e rate limiter (Polly v8) numa integração crítica com API de terceiros, com backoff exponencial, respeito ao `Retry-After` e renovação automática de token. *Esse aqui deu trabalho: foi necessário por causa de uma instabilidade que tínhamos com um provedor de dados.*

- **Integrações**: clientes HTTP declarativos (OpenFeign e Refit) com diversos sistemas externos, mTLS, Idempotency-Key, SFTP, AWS Lambda e S3 com URLs pré-assinadas. *Integrações desse tipo tinham uma camada própria no código, irmã da camada de Infrastructure da Clean Architecture tradicional.*

- **ETL e qualidade de dados**: importação em massa de CSV orientada a eventos, com detecção de encoding, relatório de erros por linha, reprocessamento seletivo e enriquecimento de dados plug-and-play. *Implementei usando uma tabela de staging, o que poupou muito retrabalho: ficava mais fácil para o usuário quando ele sabia exatamente qual dado estava errado.*

- **RPA e web scraping**: automações com Playwright (Chromium headless) e evidências de execução armazenadas no S3. *Atuei tanto em automações RPA com Selenium e Playwright quanto em scraping de HTML.*

- **Processamento de documentos**: geração de .docx (OpenXML), conversão DOCX → PDF com LibreOffice headless, extração de texto (PDFBox), compressão adaptativa de PDF e planilhas (Apache POI, ClosedXML).

- **Segurança**: hash de senhas com Argon2id e autenticação JWT com refresh token rotativo de uso único. *Security by design sempre em mente!*

- **Motor de relatórios**: engine genérica de relatórios e templates CSV baseada em catálogo configurável, reaproveitada por vários módulos. *Esse foi muito bacana de implementar: havia muitos dados disponíveis e pouca flexibilidade nos relatórios.*

</details>

<details>
<summary><b>Um desafio que me marcou</b></summary>

<br>

Um dos meus maiores desafios até hoje aconteceu logo no começo da minha experiência como desenvolvedor. O sistema de ajuizamento precisava dos nomes exatos de fóruns e comarcas para conseguir ajuizar um caso, e não havia uma fonte padronizada para esses dados.

Para resolver isso, criei do zero uma estrutura relacional interna para armazenar essas informações e fui buscá-las via scraping em sites de tribunais, listas telefônicas e PDFs que encontrei na web. Além de todo o trabalho de coleta e organização das tabelas, os nomes raramente batiam certinho entre uma fonte e outra, então implementei a distância de Levenshtein para fazer a correspondência aproximada entre eles.

</details>

---

## Stack principal

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Anthropic API](https://img.shields.io/badge/Anthropic_API-191919?style=for-the-badge&logo=anthropic&logoColor=white)

<sub>Também trabalho com: GraphQL · MySQL · SQL Server · JPA/Hibernate · EF Core · Flyway · Terraform · JUnit · xUnit · Testcontainers · Playwright</sub>

---

## Interesses e o que estou estudando

- **System Design**: sistemas distribuídos, filas e mensageria (SQS, Outbox Pattern), idempotência, escalabilidade, consistência e tolerância a falhas.
- **Inteligência Artificial**: agentes de IA (LLMs, tool use, RAG e orquestração de agentes) e algoritmos de machine learning (aprendizado supervisionado e não supervisionado, avaliação de modelos).

---

<p align="center"><i>Obrigado por ler até aqui!</i></p>
