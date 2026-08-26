# Atividade 06 — Pesquisa de Periódicos e Eventos Científicos

**Projeto de IC:** Benchmark IoT: Amazon RDS (PostgreSQL) vs. Amazon DynamoDB na AWS
**Tema resumido:** estudo experimental comparativo de desempenho (latência, vazão, tempo de resposta) entre um banco relacional (Amazon RDS/PostgreSQL) e um banco NoSQL (Amazon DynamoDB) no armazenamento de dados de sensores IoT, usando uma infraestrutura unificada na AWS (AWS IoT Core, API REST, dashboard analítico).

---

##  Parte 1 — Formas de Publicação Científica

### 1. Artigo científico (journal paper)
- **O que é:** trabalho completo, com revisão por pares, publicado em periódico científico.
- **Para que serve:** divulgar resultados consolidados e maduros de pesquisa, com validação rigorosa da comunidade.
- **Tipo de trabalho:** estudos completos, com metodologia detalhada, experimentos, resultados e discussão aprofundada.
- **Onde encontrar:** portais como SciELO, IEEE Xplore, Portal de Periódicos CAPES, Springer, ACM Digital Library.

### 2. Artigo completo em congresso
- **O que é:** trabalho completo submetido e apresentado em um congresso/simpósio, publicado nos anais do evento.
- **Para que serve:** divulgar resultados de pesquisa em andamento ou concluída, com feedback mais rápido que em periódicos.
- **Tipo de trabalho:** pesquisas experimentais, propostas de sistemas, estudos de caso, comparações técnicas.
- **Onde encontrar:** anais de eventos (ex.: SBC Open Lib / SOL, IEEE Xplore para eventos internacionais).

### 3. Pôster científico
- **O que é:** apresentação visual e resumida de uma pesquisa, exibida fisicamente ou digitalmente durante um evento.
- **Para que serve:** divulgar resultados preliminares e permitir interação direta com o autor durante sessões específicas.
- **Tipo de trabalho:** pesquisas em andamento, projetos de IC, resultados parciais.
- **Onde encontrar:** sessões de pôsteres em congressos, mostras de IC, workshops.

### 4. Mostra de Iniciação Científica
- **O que é:** evento acadêmico voltado especificamente para apresentação de trabalhos de alunos de IC, geralmente promovido pela própria universidade.
- **Para que serve:** treinar o aluno na comunicação científica e divulgar os primeiros resultados da pesquisa.
- **Tipo de trabalho:** projetos de IC em qualquer estágio (proposta, desenvolvimento ou resultados parciais).
- **Onde encontrar:** eventos internos de universidades (ex.: SIICUSP, CIC, Semana de IC institucional).

### 5. Workshop
- **O que é:** evento menor, geralmente satélite de um congresso maior, focado em um subtema específico.
- **Para que serve:** discutir tópicos emergentes ou de nicho com um público mais especializado.
- **Tipo de trabalho:** artigos curtos, propostas iniciais, discussões técnicas específicas.
- **Onde encontrar:** vinculados a grandes eventos (ex.: workshops do SBRC, do SBBD).

---

##  Parte 2 — Periódicos Científicos

**1. IEEE Internet of Things Journal**
- Editora: IEEE (Institute of Electrical and Electronics Engineers)
- Área: Internet das Coisas (arquitetura, tecnologias habilitadoras, big sensor data management, aplicações)
- Temas publicados: arquitetura IoT, gerenciamento de dados de sensores em larga escala, middleware de serviços IoT, aplicações em cidades inteligentes
- Exemplos relacionados ao tema: artigos sobre gerenciamento e armazenamento de dados de sensores em larga escala
- ISSN: 2327-4662
- Qualis: journal internacional de alto impacto (Qualis A1 em Ciência da Computação)
- Link: https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6488907

**2. JIDM — Journal of Information and Data Management**
- Editora: Sociedade Brasileira de Computação (SBC), ligado ao SBBD
- Área: gerenciamento de dados e informação
- Temas publicados: bancos de dados, mineração de dados, data warehousing, design de banco de dados, sistemas de informação geográfica
- Exemplos relacionados ao tema: versões estendidas de artigos premiados do SBBD sobre bancos de dados relacionais e NoSQL
- ISSN: 2178-7107
- Qualis: B1 (quadriênio 2017-2020, CAPES)
- Link: https://journals-sol.sbc.org.br/index.php/jidm

**3. Journal of Big Data (Springer)**
- Editora: SpringerOpen (acesso aberto)
- Área: ciência de dados e big data
- Temas publicados: armazenamento e captura de dados, tecnologias de big data, computação em nuvem, sistemas distribuídos de arquivos e bancos de dados, sistemas de armazenamento escalável
- Exemplos relacionados ao tema: artigos sobre benchmarking de bancos de dados em nuvem e comparação de sistemas de armazenamento
- ISSN: 2196-1115
- Qualis: journal internacional bem avaliado em Ciência da Computação
- Link: https://journalofbigdata.springeropen.com/

---

##  Parte 3 — Congressos e Eventos Científicos

**1. SBBD — Simpósio Brasileiro de Banco de Dados**
- Instituição: Comissão Especial de Bancos de Dados (CEBD) da SBC
- Área: bancos de dados, gerenciamento de dados, ciência de dados e big data
- Assuntos abordados: modelos de dados, sistemas de gerenciamento, indexação, desempenho e confiabilidade de bancos de dados
- Exemplos de trabalhos: comparações entre SGBDs relacionais e NoSQL, benchmarking de bancos de dados
- Periodicidade: anual (desde 1986)
- Local/modalidade: presencial, rotativo entre cidades brasileiras (ex.: SBBD 2025 em Fortaleza-CE, SBBD 2026 em São Carlos-SP)
- Link: https://sbbd.org.br/

**2. SBRC — Simpósio Brasileiro de Redes de Computadores e Sistemas Distribuídos**
- Instituição: SBC e Laboratório de Redes de Computadores (LARC)
- Área: redes de computadores e sistemas distribuídos
- Assuntos abordados: computação em nuvem, IoT, sistemas distribuídos, desempenho de redes
- Exemplos de trabalhos: arquiteturas de testbeds IoT, avaliação de desempenho em ambientes distribuídos e em nuvem
- Periodicidade: anual (há mais de quatro décadas)
- Local/modalidade: presencial, rotativo (ex.: SBRC 2025 em Natal-RN, taxa de aceitação de artigos completos ~36,5%)
- Link: https://sbrc.sbc.org.br/

**3. IEEE World Forum on Internet of Things (WF-IoT)**
- Instituição: IEEE IoT Technical Community
- Área: Internet das Coisas
- Assuntos abordados: aquisição, armazenamento e gerenciamento de dados para IoT, plataformas de computação para IoT, IoT data analytics, cidades inteligentes
- Exemplos de trabalhos: artigos técnicos sobre armazenamento de dados de sensores, deployments reais de sistemas IoT
- Periodicidade: anual
- Local/modalidade: presencial internacional, rotativo (ex.: WF-IoT 2025 em Chengdu, China; WF-IoT 2026 com tema "Connected and Resilient Ecosystems")
- Link: https://wfiot2026.iot.ieee.org/

---

##  Parte 4 — Tabelas

###  Periódicos

| Periódico | Área | Temas relacionados à minha IC | Exemplos de artigos | Link |
|---|---|---|---|---|
| IEEE Internet of Things Journal | Internet das Coisas | Gerenciamento e armazenamento de dados de sensores em larga escala | Artigos sobre big sensor data management e arquiteturas de dados IoT | https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6488907 |
| JIDM (Journal of Information and Data Management) | Bancos de dados e gerenciamento de informação | Comparação entre modelos relacional e NoSQL | Versões estendidas de artigos do SBBD sobre bancos de dados | https://journals-sol.sbc.org.br/index.php/jidm |
| Journal of Big Data (Springer) | Ciência de dados e big data | Benchmarking de bancos de dados em nuvem, sistemas de armazenamento escalável | Artigos sobre avaliação de desempenho de plataformas de nuvem | https://journalofbigdata.springeropen.com/ |

###  Eventos Científicos

| Evento | Área | Temas relacionados à minha IC | Tipo de evento | Link |
|---|---|---|---|---|
| SBBD | Bancos de dados | Comparação de desempenho entre SGBDs relacionais e NoSQL | Simpósio (artigos completos e curtos) | https://sbbd.org.br/ |
| SBRC | Redes de computadores e sistemas distribuídos | Computação em nuvem e IoT | Simpósio (com workshops associados) | https://sbrc.sbc.org.br/ |
| IEEE WF-IoT | Internet das Coisas | Armazenamento e gerenciamento de dados IoT | Congresso internacional | https://wfiot2026.iot.ieee.org/ |

---

##  Parte 5 — Análise

**1. Qual periódico encontrado possui maior relação com o seu tema?**
O JIDM é o que mais se aproxima do tema, pois é um periódico brasileiro focado especificamente em gerenciamento de dados, incluindo comparações entre modelos de banco de dados relacional e NoSQL, que é exatamente o núcleo do projeto.

**2. Qual evento científico possui maior relação com o seu tema?**
O SBBD é o mais aderente, por ser o principal evento brasileiro e da América Latina em bancos de dados, reunindo pesquisas sobre desempenho, indexação e comparação de sistemas de gerenciamento de dados — tema central do benchmark proposto.

**3. Que tipos de pesquisas você encontrou nesses periódicos e eventos?**
Predominam estudos experimentais e comparativos (benchmarks) entre SGBDs relacionais e NoSQL, artigos sobre arquiteturas de armazenamento de dados IoT, e trabalhos sobre desempenho de bancos de dados em ambientes de nuvem, avaliando métricas como tempo de resposta, vazão e uso de recursos.

**4. O que você percebeu sobre as pesquisas que estão sendo desenvolvidas na sua área?**
Percebi que há uma forte tendência de comparação entre bancos relacionais e NoSQL aplicada a cenários de grande volume de dados (IoT, big data), com foco recorrente em métricas de desempenho (latência, throughput, uso de CPU/memória) e no uso de ambientes de nuvem (AWS, Azure, GCP) como infraestrutura de teste.

**5. Como essa pesquisa pode ajudar no desenvolvimento da sua IC?**
Conhecer esses periódicos e eventos ajuda a identificar o vocabulário técnico e as métricas usadas pela comunidade científica em benchmarks de bancos de dados, além de indicar possíveis destinos futuros para submissão dos resultados da IC e servir de referência metodológica para o desenho dos experimentos.

---

##  Parte 6 — Trabalhos Semelhantes

**Trabalho 1**
- Título: An Automated Data Engineering Pipeline for Anomaly Detection of IoT Sensor Data
- Autores: não especificado nos metadados consultados (disponível no arXiv)
- Ano: 2021
- Onde foi publicado: arXiv (preprint)
- Link: https://arxiv.org/pdf/2109.13828
- Relação com o tema: o trabalho compara diretamente PostgreSQL e DynamoDB para armazenamento de dados de sensores IoT, avaliando qual banco é mais adequado para escrita contínua de grandes volumes de dados — mesma comparação de tecnologias do projeto de IC.

**Trabalho 2**
- Título: Estudo Comparativo de Bancos de Dados NoSQL
- Autores: Dinei Rockenbach, Nadine Anderle, Dalvan Griebler, Samuel Souza
- Ano: não especificado com precisão nos metadados consultados
- Onde foi publicado: disponível via Academia.edu / citado em publicações da SBC
- Link: https://www.academia.edu/36545206/Estudo_Comparativo_de_Bancos_de_Dados_NoSQL
- Relação com o tema: avalia o desempenho de SGBDs não relacionais no contexto de IoT, usando ferramenta de benchmarking e dataset real de IoT, medindo tempo de resposta, vazão, taxa de erros e consumo de CPU/memória — mesma metodologia (benchmarking com métricas de desempenho) aplicada no projeto.

---

##  Links das Fontes Utilizadas

- https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6488907
- https://en.wikipedia.org/wiki/IEEE_Internet_of_Things_Journal
- https://journals-sol.sbc.org.br/index.php/jidm
- https://journals-sol.sbc.org.br/index.php/jidm/about
- https://journalofbigdata.springeropen.com/about
- https://sbbd.org.br/
- https://sbbd.org.br/2026/sobre/
- https://sol.sbc.org.br/index.php/sbbd
- https://sbrc.sbc.org.br/2026/en/home/
- https://sol.sbc.org.br/index.php/sbrc/about
- https://sol.sbc.org.br/index.php/sbrc
- https://wfiot2026.iot.ieee.org/authors/call-papers
- https://arxiv.org/pdf/2109.13828
- https://www.academia.edu/36545206/Estudo_Comparativo_de_Bancos_de_Dados_NoSQL
