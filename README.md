# WebMCP Builder â€” FormaÃ§Ã£o 2

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


FormaÃ§Ã£o prÃ¡tica dedicada ao papel **WebMCP Builder**. O projeto ensina a sair do diagnÃ³stico de prontidÃ£o e publicar ferramentas WebMCP declarativas e imperativas sem remover a experiÃªncia humana do site.

## O que estÃ¡ incluÃ­do

- arquitetura de 4 capÃ­tulos Builder, cada um com seus prÃ³prios mÃ³dulos;
- CapÃ­tulo 1 publicado com 4 mÃ³dulos completos, 24 tÃ³picos e cerca de 12 horas;
- progresso, dÃºvidas, anotaÃ§Ãµes, temas e exportaÃ§Ã£o/importaÃ§Ã£o da jornada;
- mini-site INEMA Cursos para comparar pessoa, automaÃ§Ã£o visual e WebMCP;
- validador avanÃ§ado de catÃ¡logos, tools e JSON Schemas;
- geraÃ§Ã£o estÃ¡tica pronta para GitHub Pages e Vercel.

## CapÃ­tulos e mÃ³dulos

O menu superior navega pelos capÃ­tulos da formaÃ§Ã£o Builder. A numeraÃ§Ã£o segue `capÃ­tulo.mÃ³dulo`: `1.1`, `1.2`, `2.1` e assim por diante.

O CapÃ­tulo 1 estÃ¡ publicado com estes mÃ³dulos:

1. WebMCP, MCP e a Web agÃªntica;
2. ambiente de desenvolvimento;
3. API declarativa;
4. API imperativa.

Os capÃ­tulos 2 (Design de ferramentas), 3 (IntegraÃ§Ã£o com a aplicaÃ§Ã£o) e 4 (Qualidade de Builder) jÃ¡ estÃ£o mapeados no Ã­ndice e serÃ£o publicados progressivamente.

## Executar localmente

```bash
npm run build
npm test
npm run serve
```

Abra `http://localhost:4173`. O curso tambÃ©m Ã© legÃ­vel abrindo `index.html`, mas um servidor local representa melhor o contexto de execuÃ§Ã£o.

## Validador avanÃ§ado

O laboratÃ³rio em `labs/validador-tools.html` recebe um descritor JSON auditÃ¡vel. Ele verifica:

- unicidade, nomes, tÃ­tulos e descriÃ§Ãµes;
- estrutura de `inputSchema`;
- coerÃªncia de `required` e `properties`;
- annotations do draft;
- evidÃªncia de `AbortSignal`;
- risco, confirmaÃ§Ã£o humana, fallback e exemplo de resultado.

O scanner Ã© local, determinÃ­stico e nÃ£o registra nem executa tools. Campos de governanÃ§a como `risk`, `fallback` e `resultExample` nÃ£o pertencem ao draft WebMCP; servem para revisar prontidÃ£o operacional.

## LaboratÃ³rio do MÃ³dulo 1.1

`labs/inema-cursos.html` mantÃ©m a mesma busca em trÃªs modos: pessoa, agente visual e WebMCP. A chamada do agente Ã© uma simulaÃ§Ã£o didÃ¡tica explicitamente identificada; em ambientes compatÃ­veis, a pÃ¡gina tambÃ©m tenta registrar `buscar_cursos` pela API real.

## EspecificaÃ§Ã£o e limites

WebMCP permanece em evoluÃ§Ã£o. O conteÃºdo foi conferido em 24 de setembro de 2026 (draft de 17/09/2026) contra o [repositÃ³rio oficial WebMCP](https://github.com/webmachinelearning/webmcp), a [especificaÃ§Ã£o renderizada](https://webmachinelearning.github.io/webmcp/) e o [explainer da API declarativa](https://github.com/webmachinelearning/webmcp/blob/main/declarative-api-explainer.md).

O curso ensina `document.modelContext`, `registerTool()`, `getTools()`, `executeTool()` e ciclo de vida por `AbortSignal`. NÃ£o trata WebMCP como substituto do backend, de autorizaÃ§Ã£o ou de MCP.

## ProgressÃ£o da formaÃ§Ã£o

Todas as fases usam `<meta name="inema-course" content="webmcp-zero-expert">`. No GitHub Pages da organizaÃ§Ã£o, o estado local Ã© compartilhado pela mesma origem. Para outros domÃ­nios, o aluno pode exportar e importar a jornada em JSON com merge nÃ£o destrutivo.

Consulte [o contrato de entrega e passagem](docs/entrega-e-progressao.md).

## LicenÃ§a

CÃ³digo sob licenÃ§a MIT. ConteÃºdo educacional Â© INEMA.

## LaboratÃ³rio de aÃ§Ãµes encadeadas

Abra `labs/jornada-estudos.html` para buscar, filtrar, adicionar e conferir uma lista de estudos fictÃ­cia. Interface e ferramentas compartilham operaÃ§Ãµes validadas. A sequÃªncia local Ã© um roteiro determinÃ­stico, sem modelo de IA; o registro nativo Ã© detectado separadamente. Veja [mÃ©todo e evidÃªncias](docs/validacao-jornada.md).

O validador considera as quatro annotations opcionais do draft: `readOnlyHint`, `untrustedContentHint`, `consequentialHint` e `debugging`. Hints nÃ£o sÃ£o autorizaÃ§Ã£o.

## Mais no INEMA.CLUB

- [Ficha completa](https://www.inema.club/cursos/247-formacao-webmcp-2-builder/)
- [Guia de aprendizagem](https://www.inema.club/aprender-inteligencia-artificial/)
- [CatÃ¡logo de cursos](https://www.inema.club/cursos/)

<!-- inema-backlink:v1 -->
## Mais no INEMA.CLUB

- [Ficha completa deste curso](https://www.inema.club/cursos/247-formacao-webmcp-2-builder/)
- [Guia: como aprender inteligÃªncia artificial](https://www.inema.club/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.inema.club/cursos/)
<!-- /inema-backlink:v1 -->

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>