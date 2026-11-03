# Tarefa 09 — Submissão ao 21º CONTECSI

**Projeto de IC:** Benchmark IoT: Amazon RDS (PostgreSQL) vs. Amazon DynamoDB na AWS
**Evento:** 21º CONTECSI — Congresso Internacional de Gestão da Tecnologia e Sistemas de Informação
**Página oficial:** https://contecsi.tecsi.org/index.php/contecsi/21CONTECSI/about/submissions
**Sistema de submissão:** https://contecsi.tecsi.org/index.php/contecsi/21CONTECSI/author/submit

## Situação

**Em elaboração.** Modalidade ainda não confirmada (ver abaixo).

## Prazo

- Chamada de trabalhos: 28/08/2026 a **10/11/2026**.

## Modalidade

- **Pretendida:** PSE — Artigo completo (Full Paper).
- **Ponto de atenção:** o PSE é definido pelo CONTECSI como trabalho com pesquisa completa. O estudo ainda não tem resultados experimentais (a pasta `src/experimentos/` está vazia). A modalidade **COM (Research Communication)**, destinada a pesquisas em andamento, pode ser o enquadramento correto nesta fase. Decisão pendente com os orientadores.
- REX e POS são restritos a graduandos. A modalidade não foi escolhida.

## Regras de formatação relevantes (conforme página de diretrizes)

- Apenas arquivo Word (.docx). PDF não é aceito para PSE.
- A4, retrato, espaçamento 1,5, Times New Roman 12 pt.
- Margens: superior e esquerda 3 cm; inferior e direita 2,5 cm.
- Primeira página com título, resumo e palavras-chave, no máximo uma página.
- Se o texto for em português, a primeira página deve ser bilíngue (inglês primeiro).
- Referências em estilo APA, em ordem alfabética. (Observação: o padrão ABNT usado no restante da IC não se aplica a este evento.)
- Sequência sugerida: Introdução, Metodologia, Análise dos Resultados, Conclusões, Recomendações, Referências.
- **Manuscrito anônimo:** sem nomes, afiliações ou ORCID no arquivo. Os dados de autoria vão apenas nos metadados da plataforma. Remover metadados pessoais das propriedades do arquivo Word.
- Uso de IA: texto gerado por IA deve estar entre aspas e a ferramenta deve ser identificada.
- Até 4 autores (autor principal + 3 coautores). Cada autor pode submeter até 3 trabalhos.

## Template

O site não disponibiliza link direto para o template de PSE. O documento de referência citado na atividade (Google Docs) **não foi verificado** como versão atual e não deve ser usado como modelo oficial sem confirmação. Pendente: localizar o template na página de modalidades ou confirmar com a comissão (contecsiusp@gmail.com).

## Exemplos consultados

- Pendente: abrir pelo menos dois trabalhos PSE da 20ª edição (trilha 115) e registrar os links aqui.
  - https://contecsi.tecsi.org/index.php/contecsi/20CONTECSI/schedConf/presentations?searchField=&searchMatch=&search=&track=115
  - https://contecsi.tecsi.org/index.php/contecsi/20CONTECSI/schedConf/presentations?searchField=&searchMatch=&search=&track=110 (REX, referência apenas)

## Estrutura desta pasta

```
tarefa09-contecsi/
├── README.md
├── manuscrito/
│   └── rascunho-anonimo.md      (versão sem identificação de autoria)
└── referencias/
    └── fontes-e-trabalhos-relacionados.md
```

## Título provisório

Avaliação de Desempenho de Bancos de Dados SQL e NoSQL para Armazenamento de Dados de Sensores IoT em Ambiente de Nuvem

## Contribuição científica (provisória)

Comparação controlada entre Amazon RDS (PostgreSQL) e Amazon DynamoDB sob a mesma carga de escrita proveniente de sensores IoT simulados via AWS IoT Core. O desenho experimental é o diferencial, pois as duas bases recebem a mesma carga em paralelo.

## Pendências antes da submissão

- [ ] Decidir PSE ou COM com os orientadores (Deivison Shindi Takatu e Glauco Todesco).
- [ ] Executar os experimentos de carga e coletar latência, throughput e tempo de consulta. Sem isso, a seção de resultados não pode ser escrita.
- [ ] Obter o template oficial de PSE (ou COM) do evento.
- [ ] Converter o rascunho para .docx com a formatação do evento.
- [ ] Remover identificação de autoria do arquivo e das propriedades do Word.
- [ ] Revisar as referências em APA.
- [ ] Cadastrar autores e afiliações na plataforma.
- [ ] Submeter até 10/11/2026 e registrar o comprovante.

## Registro de submissão

- Data: pendente
- Código de confirmação: pendente
