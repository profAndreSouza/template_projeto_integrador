# Artefatos de engenharia

Esta pasta guarda documentos que tornam o projeto compreensível e verificável. Os artefatos são selecionados conforme a solução; a lista não obriga projetos a adotar todos os modelos nem todos os tipos de diagrama.

| Pasta | Modelos e exemplos | Use quando |
|---|---|---|
| [`requisitos/`](requisitos/README.md) | [`especificacao-requisitos-template.md`](requisitos/especificacao-requisitos-template.md) | houver comportamentos ou qualidades de produto a especificar |
| [`casos-de-uso/`](casos-de-uso/README.md) | [`diagrama-casos-de-uso-template.md`](casos-de-uso/diagrama-casos-de-uso-template.md), [`caso-de-uso-detalhado-template.md`](casos-de-uso/caso-de-uso-detalhado-template.md) | atores interagirem com o sistema e fluxos ajudarem na validação |
| [`dados/`](dados/README.md) | [`der-template.md`](dados/der-template.md), [`dicionario-de-dados-template.md`](dados/dicionario-de-dados-template.md) | a solução persistir ou transformar dados estruturados |
| [`arquitetura/`](arquitetura/README.md) | [`diagrama-classes-template.md`](arquitetura/diagrama-classes-template.md), [`visao-arquitetural-template.md`](arquitetura/visao-arquitetural-template.md) | for útil explicar estrutura, componentes e integrações |
| [`prototipos/`](prototipos/README.md) | [`ficha-prototipo-tela-template.md`](prototipos/ficha-prototipo-tela-template.md) | houver interface web, mobile ou outro ponto de interação |
| [`testes/`](testes/README.md) | [`plano-e-evidencias-de-testes-template.md`](testes/plano-e-evidencias-de-testes-template.md), [`roteiro-avaliacao-usuarios-template.md`](testes/roteiro-avaliacao-usuarios-template.md) | houver software, experimento ou avaliação a reproduzir |

Projetos de pesquisa, analytics, integração, automação, APIs sem interface e sistemas legados podem substituir ou complementar estes modelos com planos de análise, fontes de dados, contratos, inventários ou roteiros próprios. Documente por que o artefato escolhido serve ao projeto.

## Boas práticas

1. Preserve arquivos editáveis e registre a versão/data da exportação de diagramas e protótipos.
2. Relacione artefatos a requisitos, fontes, decisões e evidências existentes; não force relações um-para-um.
3. Em interfaces móveis, identifique plataforma, dispositivo ou tamanho usado no protótipo e teste; não presuma que uma tela web e uma tela mobile sejam idênticas.
4. Use dados sintéticos nos exemplos e nas evidências públicas. Não inclua dados reais de clientes, credenciais ou informações pessoais.
5. Marque exemplos preenchidos como fictícios e substitua-os antes de entregar o repositório.

**Exemplo fictício:** um sistema de empréstimo com painel web, aplicativo móvel e API pode relacionar o requisito de consultar empréstimos ao caso de uso, aos protótipos web/mobile, à rota da API e ao teste correspondente. O DER só entra na relação se a consulta depender de dados persistidos no modelo.
