# Documentação do projeto

Use esta pasta para os documentos acadêmicos e os artefatos de engenharia que ajudem a explicar, construir ou avaliar o projeto. Consulte o [template institucional de TG](TG-Template-ADS-formato-academico%201-v1.docx) e siga as orientações atuais da disciplina. Não transforme todos os exemplos desta estrutura em entregáveis obrigatórios: mantenha somente os que fizerem sentido para o problema e para a etapa.

## Documento acadêmico

- Mantenha a versão editável e a exportação em PDF quando esses arquivos fizerem parte da entrega.
- Registre a data ou versão das cópias para que seja possível saber se DOCX e PDF correspondem ao mesmo conteúdo.
- Preserve a estrutura e a nomenclatura do template institucional; confirme dúvidas de interpretação com a orientação.
- Não use o README ou os modelos de engenharia como substitutos da monografia.

**Exemplo fictício:** `tg.docx` é a versão de trabalho atualizada em 2026-10-20 e `tg.pdf` é a exportação feita na mesma data. A equipe registra os capítulos ainda em redação no controle do projeto, sem afirmar que estão concluídos.

## Artefatos de engenharia

Os modelos ficam organizados por assunto. Copie e adapte somente os que forem úteis.

| Pasta | Conteúdo possível |
|---|---|
| [`artefatos/requisitos/`](artefatos/requisitos/README.md) | requisitos funcionais/não funcionais e regras confirmadas |
| [`artefatos/casos-de-uso/`](artefatos/casos-de-uso/README.md) | objetivos dos atores e especificações de fluxos, quando adequados ao sistema |
| [`artefatos/dados/`](artefatos/dados/README.md) | DER, dicionário e estrutura persistida, se houver dados estruturados |
| [`artefatos/arquitetura/`](artefatos/arquitetura/README.md) | visão arquitetural e classes, conforme necessidade |
| [`artefatos/prototipos/`](artefatos/prototipos/README.md) | protótipos web, mobile ou de outros pontos de interação |
| [`artefatos/testes/`](artefatos/testes/README.md) | roteiro de testes técnicos, avaliação e evidências pertinentes |

Projetos de pesquisa, análise de dados, API sem interface, integração, automação ou evolução de sistema legado podem usar outros artefatos. Registre a justificativa quando um modelo não se aplicar; não crie tabelas, telas ou diagramas apenas para preencher a pasta.

## Backlog, decisões e continuidade

- [`backlog/`](backlog/README.md): use um Product Backlog se a equipe trabalha com uma lista ordenada de produto; projetos de pesquisa e dados podem escolher um plano ou catálogo mais adequado.
- [`decisoes/`](decisoes/README.md): registre decisões importantes de escopo, dados, arquitetura, segurança ou integração.
- [`continuidade/`](continuidade/README.md): compare a linha de base recebida com as contribuições do semestre atual.

## Organização atual

```tex
docs/
├── TG-Template-ADS-formato-academico 1-v1.docx
├── tg.docx                         # adicionar se fizer parte da entrega
├── tg.pdf                          # adicionar exportação correspondente
├── README.md
├── artefatos/
├── backlog/
├── decisoes/
└── continuidade/


## Exemplo de uso

Uma equipe com aplicativo móvel, painel web e API mantém os requisitos, casos de uso e protótipos em `artefatos/`, descreve a instalação nos READMEs dos componentes e registra os cenários de teste. Uma equipe de analytics pode manter proveniência, dicionário de dados e reprodução dos cálculos em `data/` e referenciá-los na monografia. Estes são exemplos; a organização final deve refletir o projeto real.
