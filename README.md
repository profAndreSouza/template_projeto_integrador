# Repositório do Projeto Integrador / Trabalho de Graduação — ADS

Modelo inicial para equipes que desenvolvem software, aplicativos móveis, integrações, automações, análises de dados ou projetos que combinam essas frentes. Adapte a estrutura ao problema e aos entregáveis reais: as pastas de tecnologia são opcionais e não indicam, por si só, que um componente foi implementado.

O documento acadêmico deve seguir o [template institucional disponível em `docs/`](docs/README.md). Este README orienta o uso do repositório; ele não substitui o documento acadêmico nem as orientações do professor.

## Identificação

- **Projeto:** Nome usado pela equipe
- **Equipe:** identificação da equipe ou autores conforme orientação da disciplina
- **Orientação:** preencher quando aplicável
- **Cliente ou parceiro:** nome público ou descrição geral; não inclua dados pessoais ou informações confidenciais
- **Disciplina/etapa:** PI, TG I, TG II ou outra etapa
- **Versão analisada:** tag, release ou commit, quando houver
- **Atualizado em:** AAAA-MM-DD

## Resumo do projeto

Descreva em um parágrafo o contexto, o problema, quem é afetado, o objetivo e o que já foi produzido. Diferencie resultados observados de resultados esperados. Siga a extensão e a estrutura indicadas pelo template acadêmico e pela orientação da disciplina quando houver exigência.

**Exemplo fictício:** Uma escola registra empréstimos de equipamentos em planilhas separadas, o que dificulta consultar a disponibilidade. A equipe está desenvolvendo uma aplicação com uma interface web e um aplicativo móvel para registrar solicitações; uma API compartilhada mantém os dados. Nesta versão, o fluxo de solicitação está implementado em ambiente local e ainda não foi validado pela escola.

## Problema, objetivos e avaliação

- **Problema ou necessidade:** descreva a necessidade documentada, sem expor dados confidenciais.
- **Objetivo:** informe o resultado que o projeto pretende produzir.
- **Pergunta ou hipótese:** preencha quando a natureza da pesquisa e a orientação acadêmica pedirem. Não invente hipótese para projeto em que ela não se aplica.
- **Como será avaliado:** indique testes, análise, demonstração, avaliação com participantes ou validação pelo cliente, conforme o método do projeto. Registre resultados somente depois de obtê-los.

**Exemplo fictício:** Problema: a equipe escolar não consegue consultar com facilidade quais equipamentos estão emprestados. Objetivo: construir um fluxo que permita registrar e consultar empréstimos. Avaliação prevista: executar cenários com dados sintéticos e, após autorização, discutir o fluxo com representantes da escola.

## Escopo e situação desta versão

### Incluído ou produzido

- Descreva funcionalidades, análises, integrações ou artefatos concluídos e em andamento. Identifique o estado de cada item.

### Fora do escopo ou ainda não iniciado

- Registre exclusões, itens adiados e dependências conhecidas. Não trate uma ideia como decisão aprovada.

### Limitações, premissas e riscos

- Explique a limitação, seu impacto e a ação ou decisão pendente.

**Exemplo fictício:** A interface web e o aplicativo móvel consultam a mesma API em ambiente local. Notificações push e publicação nas lojas não fazem parte desta versão. A avaliação com usuários depende de autorização da escola.

Registre mudanças relevantes de escopo ou arquitetura em [decisões](docs/decisoes/README.md). Em projetos continuados, compare a entrega recebida com o trabalho deste semestre em [continuidade](docs/continuidade/README.md).

## Componentes e evidências

Use a tabela para explicar o que existe, o estado e onde encontrar evidência. Remova as linhas não aplicáveis; não crie componentes apenas para preencher o modelo.

| Componente ou frente | Estado | Evidência e localização |
|---|---|---|
| Pesquisa, requisitos ou backlog | Não iniciado / em andamento / concluído / N/A | `docs/` ou outro caminho real |
| API ou backend | Não iniciado / em andamento / concluído / N/A | `backend/` ou caminho real |
| Interface web | Não iniciado / em andamento / concluído / N/A | `frontend/` ou caminho real |
| Aplicativo móvel | Não iniciado / em andamento / concluído / N/A | `mobile/` ou caminho real |
| Dados, ETL ou integração | Não iniciado / em andamento / concluído / N/A | `data/` ou caminho real |
| Empacotamento e implantação | Não iniciado / em andamento / concluído / N/A | `application/` ou caminho real |
| Testes e validação | Não iniciado / em andamento / concluído / N/A | `docs/artefatos/testes/` ou caminho real |
| Documento acadêmico | Não iniciado / em andamento / concluído / N/A | `docs/` e versão/data |

## Rastreabilidade do projeto

Registre relações que existam no projeto. A cadeia ajuda a explicar o trabalho, mas não exige que todo requisito gere uma tabela, classe, endpoint ou tela.

| Necessidade/objetivo | Requisito, pergunta ou item de trabalho | Caso de uso/modelo/protótipo | Implementação ou análise | Validação/evidência | Estado |
|---|---|---|---|---|---|
| Exemplo: consultar equipamentos disponíveis | RF-01, se aprovado | UC-01 e protótipo da consulta | API e interfaces web/mobile | Cenário com dados fictícios; resultado registrado no roteiro | Em andamento |

Mantenha identificadores consistentes nos documentos e no código. Quando uma relação não se aplicar, explique o motivo em vez de preencher com uma associação artificial.

## Organização do repositório

```tex
docs/          documento acadêmico, requisitos, modelos, decisões e evidências
backend/       API ou serviços de backend, se existirem
frontend/      interface web, se existir
mobile/        aplicativo móvel, se existir
data/          dados sintéticos, consultas ou pipelines, se aplicável
application/   scripts de integração, implantação ou execução conjunta, se aplicável


Uma equipe pode manter somente `docs/`, `mobile/` e `backend/`, por exemplo. Um projeto de análise de dados pode usar `data/` e `docs/` sem criar uma interface. Ajuste a estrutura e os READMEs às tecnologias realmente utilizadas.

## Continuidade de semestre

Se o projeto recebeu código, pesquisa, protótipos, documentos ou dados de uma etapa anterior, registre a linha de base e diferencie o que foi herdado, alterado, criado, validado ou descontinuado. Se começou nesta etapa, registre que não há linha de base anterior. Consulte [continuidade](docs/continuidade/README.md).

## Como começar

1. Leia [`docs/README.md`](docs/README.md) e mantenha somente os artefatos pertinentes.
2. Consulte o README de cada componente existente: [`backend/`](backend/README.md), [`frontend/`](frontend/README.md), [`mobile/`](mobile/README.md) e [`application/`](application/README.md).
3. Registre os pré-requisitos e comandos efetivamente usados pela equipe; não copie exemplos como se fossem comandos testados no projeto.
4. Use dados fictícios em desenvolvimento e testes. Nunca versione senhas, tokens, chaves privadas ou dados pessoais/reais do cliente.

## Exemplo preenchido (fictício)

O exemplo da escola nesta página é inventado e serve apenas para demonstrar como distinguir problema, escopo, componentes e evidências. Substitua-o pelos fatos confirmados do projeto; não o apresente como requisito ou validação real.
