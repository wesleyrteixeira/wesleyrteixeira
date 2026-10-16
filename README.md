<div align="center">

# Wesley Rodrigues Teixeira

**Especialista em Projetos de RPA e IA · Automação Fiscal e Financeira**

Construo automações que tiram do caminho a conferência manual de notas, extratos e relatórios, com regra fiscal no código e rastreabilidade de ponta a ponta.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/wesley-rodrigues-teixeira-a7595163/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:wesleyrteixeira@hotmail.com)

`+63% das NFS-e aprovadas sem analista` · `~24 robôs orquestrados em Kubernetes` · `extratos bancários diários via API`

</div>

---

## Sobre mim

Sou **engenheiro mecatrônico** e cheguei à automação pelo caminho dos processos: qualidade automotiva (ISO/TS 16949), excelência operacional e melhoria contínua em logística. Por isso, antes de escrever um robô, eu mapeio o processo, meço e só então automatizo.

Hoje sou **Especialista em Projetos de RPA e IA na Trinus**, onde conduzo iniciativas de melhoria contínua da concepção à mensuração de resultados, desenvolvendo automações e produtos internos para as áreas **fiscal, financeira e contábil**: da captura do documento na fonte (portal da NFS-e, SEFAZ, APIs bancárias, ERPs) até a validação, o registro e a publicação do resultado para quem decide.

| Frente | O que eu faço |
|---|---|
| **Fiscal** | Conciliação de NFS-e com processos de pagamento, validação de ISS, IRRF, CSRF e INSS contra a legislação, extração de notas por IA |
| **Financeiro** | Integração com APIs bancárias via mTLS, extratos e francesinha diários, relatórios de ERP |
| **Plataforma** | DAGs do Airflow em Kubernetes, boilerplate corporativo para novos robôs, portal interno de operação das automações |

---

## Como eu trabalho

- **Processo antes de código.** Automatizar um processo ruim só faz o erro acontecer mais rápido; primeiro se mapeia, mede e simplifica.
- **Regra fiscal é código, não planilha.** Alíquotas e retenções são validadas contra fonte oficial, versionadas e auditáveis.
- **IA com rede de proteção.** LLM extrai; validação determinística (CNPJ, regex, tabelas oficiais) e um gate de confiança decidem o que segue sozinho e o que vai para revisão humana.
- **Segredo não mora no repositório.** Certificados e credenciais ficam no Key Vault; histórico limpo e gitleaks no CI.
- **Automação precisa provar valor.** Cada robô fiscal tem painel mostrando quanto resolveu sozinho e quanto ainda precisou de analista.

---

## Projetos em destaque

### 🧾 Análise fiscal automatizada de NFS-e
**Contexto:** toda nota de serviço passava por conferência manual de impostos antes do pagamento.
**Solução:** robô que concilia processos de pagamento pendentes no ERP com o XML da nota e valida as retenções contra a legislação. Sem XML, três agentes de IA (extração, auditoria e consolidação) leem o PDF ou a imagem de qualquer layout municipal. O resultado volta ao ERP como comentário e status.
**Resultado:** **mais de 63% das notas aprovadas automaticamente**, com painel de ROI acompanhando a evolução semana a semana.

`Python` · `OpenAI` · `Anthropic` · `PyMuPDF` · `SQL Server` · `Databricks`

### 🏦 Integração bancária
**Contexto:** extratos e saldos de várias empresas capturados e conciliados à mão.
**Solução:** serviços em Clean Architecture que consomem as APIs do Itaú e do ABC Brasil via mTLS, gravam saldos e francesinha diariamente e geram o extrato mensal em PDF no layout do internet banking. Inclui uma ferramenta própria para emitir e rotacionar os certificados no Key Vault.
**Resultado:** extratos de todas as empresas do grupo publicados diariamente, sem intervenção.

`Python` · `reportlab` · `AKS CronJob` · `Azure Key Vault` · `Azure Pipelines`

### ⚙️ Plataforma de automações
**Contexto:** robôs sem padrão de projeto, agendamento ou visibilidade para as áreas.
**Solução:** Airflow 3 em Kubernetes, em que cada DAG sobe um pod com o robô; boilerplate corporativo com ports, CI, testes e gitleaks; e um portal em Next.js para listar, executar, agendar e monitorar as automações.
**Resultado:** **cerca de 24 DAGs em produção** sob o mesmo padrão de deploy e observabilidade.

`Airflow` · `Kubernetes` · `Next.js` · `TypeScript` · `Python`

### 📥 Captura de documentos fiscais
**Contexto:** download manual de notas, empresa por empresa.
**Solução:** RPA no portal nacional da NFS-e com certificados A1 do Key Vault e cliente SOAP mTLS para o serviço de distribuição de NF-e da SEFAZ, com controle de NSU.
**Resultado:** notas emitidas e recebidas de todas as empresas com certificado disponíveis no banco e no SharePoint.

`Python` · `Playwright` · `SOAP` · `mTLS` · `SQL Server`

### 📚 Inteligência tributária
**Contexto:** tabelas de retenção desatualizadas e códigos de serviço declarados errados nas notas.
**Solução:** auditoria da base de retenções federais contra 25 fontes oficiais, catálogo tributário 2026 com índice de busca (RAG), classificador de item da LC 116 e correlação de 1.332 CNAEs com os itens de serviço. Também incluiu estudos da API da NFS-e nacional e da calculadora CBS da reforma tributária.
**Resultado:** base de referência confiável para as validações fiscais automáticas.

`Python` · `OpenAI` · `RAG` · `SQL` · `APIs públicas`

### 💬 Cobrança Zero Touch
**Contexto:** cobrança e relacionamento manuais com clientes de uma locadora.
**Solução:** régua de lembretes por WhatsApp com multa e juros, lembretes de manutenção, programa VIP e relatório diário de inadimplência.

`Node.js` · `n8n` · `PostgreSQL` · `Asaas` · `WhatsApp`

---

## Stack principal

**Linguagens e back-end**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)

**Automação, IA e infraestrutura**

![Apache Airflow](https://img.shields.io/badge/Apache_Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=anthropic&logoColor=white)

---

## Trajetória

| Período | Empresa | Papel | Escopo |
|---|---|---|---|
| 2025 – atual | **Trinus** | Especialista em Projetos de RPA e IA | Gestão de projetos de melhoria contínua, automações fiscais, financeiras e contábeis com IA, integrações bancárias e plataforma de RPA |
| 2023 – 2025 | **Trinus** | Analista de Melhoria Contínua Sênior | Automações e integrações com a API do ERP usando Python (Requests, Flask, FastAPI, Django) e Power Automate |
| 2022 – 2023 | **Comfrio** | Engenheiro de Melhoria Contínua | Análise de fluxos logísticos, identificação de ineficiências e projetos de melhoria |
| 2021 – 2022 | **Comfrio** | Analista de Excelência Operacional | Otimização de processos e inteligência de mercado |
| 2014 – 2019 | **Metalúrgica Agathon** | Engenheiro de Processos de Qualidade | Sistema de gestão de processos e controle de qualidade de produtos automotivos (ISO/TS 16949) |
| 2012 – 2014 | **Metalúrgica Agathon** | Estagiário de Engenharia da Qualidade | Análises dimensionais, testes e registro de resultados |

---

## GitHub em números

<div align="center">

![Gráfico de atividade](https://github-readme-activity-graph.vercel.app/graph?username=wesleyrteixeira&hide_border=true&theme=tokyo-night&area=true)

</div>

---

## Vamos conversar?

Tenho interesse especial em **automação fiscal e tributária**, **IA aplicada a documentos** e **integrações financeiras**, inclusive o que muda com a reforma tributária.

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/wesley-rodrigues-teixeira-a7595163/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:wesleyrteixeira@hotmail.com)

</div>
