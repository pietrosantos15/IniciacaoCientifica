# Benchmark IoT: Amazon RDS (PostgreSQL) vs. Amazon DynamoDB na AWS

### 📌 Título do Projeto
Benchmark IoT: Amazon RDS (PostgreSQL) vs. Amazon DynamoDB na AWS

---

### 📝 Descrição da Proposta
O projeto consiste em um estudo experimental e comparativo focado em fornecer critérios empíricos para a seleção de modelos de banco de dados (relacional e NoSQL) no ecossistema de Internet das Coisas (IoT). A proposta visa mitigar escolhas arquiteturais inadequadas baseadas apenas na familiaridade da equipe de desenvolvimento. Para isso, o sistema simula o fluxo contínuo de múltiplos sensores e utiliza uma infraestrutura unificada na nuvem para submeter de forma simétrica e paralela tanto o banco relacional quanto o NoSQL exatamente à mesma carga de trabalho, avaliando suas limitações estruturais sob cenários de alta volumetria.

---

### 🎯 Objetivos

* **Objetivo Geral:** Avaliar comparativamente o desempenho do Amazon RDS com PostgreSQL e do Amazon DynamoDB no armazenamento de dados oriundos de sensores IoT sob condições controladas de infraestrutura.
* **Objetivos Específicos:** * Configurar um ambiente de testes reprodutível e integrado na nuvem AWS.
    * Implementar rotinas equivalentes de escrita e leitura em paralelo em ambos os bancos de dados.
    * Mensurar e comparar métricas de latência, vazão (*throughput*) e tempo de resposta de consultas analíticas sob diferentes volumes de dados.
    * Desenvolver uma interface visual para validação e acompanhamento contínuo dos resultados obtidos no benchmark.

---

### 🛠️ Tecnologias Utilizadas

* **Ingestão de dados:** AWS IoT Core utilizando o protocolo leve MQTT.
* **Processamento e Integração:** API REST (Back-end) para validação e espelhamento síncrono das escritas.
* **Banco de Dados Relacional:** Amazon RDS executando o motor PostgreSQL.
* **Banco de Dados Não Relacional (NoSQL):** Amazon DynamoDB (modelo chave-valor/serverless).
* **Segurança da Informação:** AWS IAM para gerenciamento de permissões, além de criptografia TLS/SSL e certificados digitais x.509.
* **Camada de Apresentação:** Dashboard Analítico para monitoramento de métricas em tempo real.

---

### 📐 Arquitetura da Solução
A arquitetura é estruturada de forma linear e modular:

1.  Os sensores na borda geram dados continuamente e realizam o envio de telemetria via MQTT para o AWS IoT Core.
2.  O AWS IoT Core recebe as mensagens e as encaminha de forma automatizada via regras de roteamento para a API REST (Back-end).
3.  A API valida os pacotes e efetua requisições de escrita paralelas e simultâneas direcionadas tanto ao Amazon RDS (PostgreSQL) quanto ao Amazon DynamoDB.
4.  O Dashboard Analítico consome os endpoints da API para extrair os registros históricos e correntes, exibindo o comportamento do benchmark.

---

### 🖼️ Diagrama


<img width="1139" height="617" alt="diagramaa" src="https://github.com/user-attachments/assets/a2ea2282-86ae-4535-88c4-f18110bd0cc2" />

---

### 📚 Referências Principais

1. ALMEIDA, Thiago Leite de et al. IOT para monitoramento de equipamentos industriais e armazenamento em banco de dados relacional. **Revista Brasileira de Mecatrônica**, v. 4, n. 2, p. 16-34, 2021.
2. CAMPOS, T. de A. et al. Avaliação de Plataformas de Armazenamento em Nuvem para Dados de Sensores. **ResearchGate**, 2019.
3. CARR, Caroline Nunes et al. Modelagem de dados para a internet das coisas (IOT): desafios e soluções ao modelar dados gerados por dispositivos conectados. **Revista Observatorio de la Economía Latinoamericana**, v. 21, n. 12, p. 23858-23874, 2023.
4. COSTA, R. et al. Uso de Banco de Dados em Arquitetura de Microsserviços. **Journal of Innovation and Science: Research and Application**, 2021.
5. PIRES, Luis Fernando. **Banco de dados para IoT**: uma abordagem analítica sobre desempenho e eficiência. Artigo (Mestrado Profissional) – UNIFACCAMP, 2025.
6. SILVA, A. et al. Banco de Dados para IoT. **Revista de Ubiquidade**, Centro Universitário Anchieta, 2024.
7. SILVA, D. O. et al. Desempenho e Escalabilidade de Plataformas Livres de IoT. In: **Anais do XXXVIII SBRC**, Porto Alegre: SBC, 2020.
