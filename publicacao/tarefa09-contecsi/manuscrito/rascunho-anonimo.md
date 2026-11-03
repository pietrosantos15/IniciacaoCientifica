<!-- RASCUNHO — NÃO SUBMETER. Sem autoria (avaliação cega). Seções de resultados pendentes de dados experimentais. -->

# Avaliação de Desempenho de Bancos de Dados SQL e NoSQL para Armazenamento de Dados de Sensores IoT em Ambiente de Nuvem

**Performance Evaluation of SQL and NoSQL Databases for Storing IoT Sensor Data in a Cloud Environment**

**Resumo**

O crescimento da Internet das Coisas (IoT) gera grandes volumes de dados de sensores, o que exige soluções de armazenamento eficientes e escaláveis. Este trabalho apresenta uma pesquisa em andamento que compara o desempenho do Amazon RDS (PostgreSQL), banco relacional, com o Amazon DynamoDB, banco NoSQL, no armazenamento de dados de sensores IoT na nuvem AWS. Uma arquitetura foi projetada para que sensores simulados enviem telemetria via MQTT ao AWS IoT Core, que a encaminha a uma API REST responsável por gravar, de forma simétrica, nos dois bancos, garantindo a mesma carga de trabalho. As métricas consideradas são latência de inserção, vazão e tempo de resposta de consultas analíticas. [RESULTADOS: inserir valores obtidos ou remover esta frase.] Os resultados pretendem oferecer critérios empíricos para a escolha de modelos de banco de dados em projetos IoT.

**Palavras-chave:** Internet das Coisas; banco de dados relacional; banco de dados NoSQL; Amazon Web Services; desempenho.

**Abstract**

The growth of the Internet of Things (IoT) produces large volumes of sensor data, which requires efficient and scalable storage. This work presents an ongoing study that compares the performance of Amazon RDS (PostgreSQL), a relational database, and Amazon DynamoDB, a NoSQL database, for storing IoT sensor data in the AWS cloud. An architecture was designed so that simulated sensors send telemetry via MQTT to AWS IoT Core, which forwards it to a REST API that writes symmetrically to both databases, guaranteeing the same workload. The metrics considered are insertion latency, throughput and analytical query response time. [RESULTS: insert obtained values or remove this sentence.] The results aim to provide empirical criteria for choosing database models in IoT projects.

**Keywords:** Internet of Things; relational database; NoSQL database; Amazon Web Services; performance.

---

## 1 Introdução

A transformação digital tem reconfigurado os sistemas computacionais em diversos setores. Nesse contexto, a Internet das Coisas (IoT) caracteriza-se pela interconexão de dispositivos físicos que coletam, transmitem e processam dados de forma contínua. Sensores industriais, agrícolas, urbanos e de saúde geram volumes expressivos de dados, o que exige armazenamento eficiente e escalável.

O desempenho do banco de dados afeta diretamente a confiabilidade dessas aplicações, pois sensores costumam gerar dados em alta frequência e de forma ininterrupta. Bancos relacionais são consolidados e robustos do ponto de vista transacional, mas podem apresentar limitações de escalabilidade horizontal sob cargas típicas de IoT. Bancos não relacionais são alternativas com flexibilidade de esquema e alta vazão de escrita (Carr et al., 2023).

A escolha entre essas tecnologias ainda é frequentemente guiada pela familiaridade da equipe, e não por avaliação sistemática sob condições reais. Plataformas de nuvem como a AWS oferecem serviços gerenciados para ingestão de dados de sensores e para os dois paradigmas de armazenamento no mesmo ambiente, o que torna possível uma comparação com infraestrutura equivalente.

## 2 Problema, questão de pesquisa e objetivos

**Problema.** Há escassez de estudos que comparem, de forma simultânea e controlada, um banco relacional gerenciado e um banco NoSQL no mesmo ambiente de nuvem, alimentados por dados de sensores IoT. Muitos trabalhos utilizam configurações heterogêneas, o que compromete a validade dos resultados.

**Questão de pesquisa.** Qual dos dois modelos apresenta melhor desempenho de escrita e de consulta analítica para dados de sensores IoT sob volumes e taxas de inserção crescentes, quando recebem a mesma carga em infraestrutura equivalente?

**Objetivo geral.** Avaliar comparativamente o desempenho do Amazon RDS (PostgreSQL) e do Amazon DynamoDB no armazenamento de dados de sensores IoT em ambiente de nuvem controlado.

**Objetivos específicos.** (a) configurar um ambiente de testes reprodutível na AWS, com sensores simulados e ingestão via AWS IoT Core; (b) implementar rotinas equivalentes de escrita e leitura nos dois bancos; (c) mensurar latência de inserção, vazão e tempo de consulta sob diferentes volumes; (d) desenvolver um painel analítico para acompanhamento dos dados e dos resultados.

**Hipótese.** Espera-se que o DynamoDB apresente desempenho superior em operações de alta taxa de inserção, e que o PostgreSQL apresente vantagem em consultas analíticas complexas e em cargas que exigem consistência transacional. Essa hipótese será testada, não assumida.

## 3 Trabalhos relacionados

Campos et al. (2019) compararam PostgreSQL, MongoDB e VoltDB no armazenamento de dados de sensoriamento em nuvem e concluíram que cada tecnologia tem vantagens conforme o padrão de acesso. Silva et al. (2020) avaliaram o desempenho e a escalabilidade de plataformas livres de IoT, com foco em sistemas distribuídos. Costa et al. (2021) discutiram o uso de bancos relacionais e NoSQL em arquiteturas de microsserviços. Silva et al. (2024) analisaram bancos para IoT, incluindo latência e taxa de ingestão de dados de sensores.

A diferença deste estudo está na simetria do experimento: as duas bases recebem a mesma carga, no mesmo ambiente, a partir do mesmo fluxo de ingestão. [Discutir cada trabalho com a lacuna específica, sem apenas listá-los.]

## 4 Metodologia

A pesquisa é experimental e comparativa. A arquitetura é linear e modular, composta por cinco camadas:

1. **Sensores simulados** geram telemetria continuamente e a enviam via MQTT.
2. **AWS IoT Core** recebe as mensagens e as encaminha por regras de roteamento a uma API REST.
3. **API REST (back-end)** valida os pacotes e grava, em paralelo, no Amazon RDS (PostgreSQL) e no Amazon DynamoDB.
4. **Bancos de dados:** RDS com PostgreSQL (modelo relacional, esquema definido) e DynamoDB (modelo chave-valor serverless).
5. **Painel analítico** consome os endpoints da API para exibir dados históricos e correntes.

A segurança utiliza AWS IAM para permissões, TLS/SSL e certificados X.509 nas comunicações. As métricas serão coletadas sob diferentes volumes e taxas de geração de dados: latência de inserção, vazão (throughput) e tempo de resposta de consultas analíticas.

[Detalhar, antes da submissão: tipo e tamanho das instâncias, versão do PostgreSQL, modo de capacidade do DynamoDB, esquema da tabela, distribuição das cargas (taxas e volumes), número de repetições por cenário, ferramenta de medição e procedimento de coleta.]

## 5 Desenvolvimento do experimento

[Descrever a implementação efetivamente realizada. Atualmente, a arquitetura e o fluxo de dados estão definidos; a implementação dos componentes de ingestão, escrita paralela e painel está em andamento. Não descrever etapas não executadas.]

## 6 Análise dos resultados

[PENDENTE. Esta seção só pode ser escrita com dados experimentais coletados. Incluir tabelas e gráficos numerados e referenciados no texto, com a análise de cada métrica e a comparação com a hipótese. Não inserir valores estimados.]

## 7 Conclusões

Este trabalho apresentou o projeto e o estágio atual de uma pesquisa sobre o desempenho comparativo entre bancos relacionais e NoSQL no armazenamento de dados de sensores IoT na nuvem. A revisão de literatura indica uma lacuna de estudos controlados nesse cenário. [Completar com a principal conclusão empírica, somente após a análise.]

## 8 Limitações e trabalhos futuros

Por se tratar de pesquisa em andamento, os resultados são preliminares. Os sensores são simulados, o que pode diferir de dispositivos reais. As conclusões se restringem às configurações de instância e carga testadas. Como trabalhos futuros, pretende-se ampliar os cenários de carga e avaliar o uso de custos de infraestrutura como métrica adicional.

## Referências

[Montar em APA, somente com as fontes citadas no texto. Ver `../referencias/fontes-e-trabalhos-relacionados.md`.]
