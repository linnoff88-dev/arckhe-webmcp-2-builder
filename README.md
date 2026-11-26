ï»¿# WebMCP Builder ê¢â¬â FormaêÂ§êÂ£o 2

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


FormaêÂ§êÂ£o prêÂ¡tica dedicada ao papel **WebMCP Builder**. O projeto ensina a sair do diagnêÂ³stico de prontidêÂ£o e publicar ferramentas WebMCP declarativas e imperativas sem remover a experiêÂªncia humana do site.

## O que estêÂ¡ incluêÂ­do

- arquitetura de 4 capêÂ­tulos Builder, cada um com seus prêÂ³prios mêÂ³dulos;
- CapêÂ­tulo 1 publicado com 4 mêÂ³dulos completos, 24 têÂ³picos e cerca de 12 horas;
- progresso, dêÂºvidas, anotaêÂ§êÂµes, temas e exportaêÂ§êÂ£o/importaêÂ§êÂ£o da jornada;
- mini-site ARCKHÉ Cursos para comparar pessoa, automaêÂ§êÂ£o visual e WebMCP;
- validador avanêÂ§ado de catêÂ¡logos, tools e JSON Schemas;
- geraêÂ§êÂ£o estêÂ¡tica pronta para GitHub Pages e Vercel.

## CapêÂ­tulos e mêÂ³dulos

O menu superior navega pelos capêÂ­tulos da formaêÂ§êÂ£o Builder. A numeraêÂ§êÂ£o segue `capêÂ­tulo.mêÂ³dulo`: `1.1`, `1.2`, `2.1` e assim por diante.

O CapêÂ­tulo 1 estêÂ¡ publicado com estes mêÂ³dulos:

1. WebMCP, MCP e a Web agêÂªntica;
2. ambiente de desenvolvimento;
3. API declarativa;
4. API imperativa.

Os capêÂ­tulos 2 (Design de ferramentas), 3 (IntegraêÂ§êÂ£o com a aplicaêÂ§êÂ£o) e 4 (Qualidade de Builder) jêÂ¡ estêÂ£o mapeados no êÂ­ndice e serêÂ£o publicados progressivamente.

## Executar localmente

```bash
npm run build
npm test
npm run serve
```

Abra `http://localhost:4173`. O curso tambêÂ©m êÂ© legêÂ­vel abrindo `index.html`, mas um servidor local representa melhor o contexto de execuêÂ§êÂ£o.

## Validador avanêÂ§ado

O laboratêÂ³rio em `labs/validador-tools.html` recebe um descritor JSON auditêÂ¡vel. Ele verifica:

- unicidade, nomes, têÂ­tulos e descriêÂ§êÂµes;
- estrutura de `inputSchema`;
- coerêÂªncia de `required` e `properties`;
- annotations do draft;
- evidêÂªncia de `AbortSignal`;
- risco, confirmaêÂ§êÂ£o humana, fallback e exemplo de resultado.

O scanner êÂ© local, determinêÂ­stico e nêÂ£o registra nem executa tools. Campos de governanêÂ§a como `risk`, `fallback` e `resultExample` nêÂ£o pertencem ao draft WebMCP; servem para revisar prontidêÂ£o operacional.

## LaboratêÂ³rio do MêÂ³dulo 1.1

`labs/ARCKHÉ-cursos.html` mantêÂ©m a mesma busca em trêÂªs modos: pessoa, agente visual e WebMCP. A chamada do agente êÂ© uma simulaêÂ§êÂ£o didêÂ¡tica explicitamente identificada; em ambientes compatêÂ­veis, a pêÂ¡gina tambêÂ©m tenta registrar `buscar_cursos` pela API real.

## EspecificaêÂ§êÂ£o e limites

WebMCP permanece em evoluêÂ§êÂ£o. O conteêÂºdo foi conferido em 24 de setembro de 2026 (draft de 17/09/2026) contra o [repositêÂ³rio oficial WebMCP](https://github.com/webmachinelearning/webmcp), a [especificaêÂ§êÂ£o renderizada](https://webmachinelearning.github.io/webmcp/) e o [explainer da API declarativa](https://github.com/webmachinelearning/webmcp/blob/main/declarative-api-explainer.md).

O curso ensina `document.modelContext`, `registerTool()`, `getTools()`, `executeTool()` e ciclo de vida por `AbortSignal`. NêÂ£o trata WebMCP como substituto do backend, de autorizaêÂ§êÂ£o ou de MCP.

## ProgressêÂ£o da formaêÂ§êÂ£o

Todas as fases usam `<meta name="ARCKHÉ-course" content="webmcp-zero-expert">`. No GitHub Pages da organizaêÂ§êÂ£o, o estado local êÂ© compartilhado pela mesma origem. Para outros domêÂ­nios, o aluno pode exportar e importar a jornada em JSON com merge nêÂ£o destrutivo.

Consulte [o contrato de entrega e passagem](docs/entrega-e-progressao.md).

## LicenêÂ§a

CêÂ³digo sob licenêÂ§a MIT. ConteêÂºdo educacional êÂ© ARCKHÉ.

## LaboratêÂ³rio de aêÂ§êÂµes encadeadas

Abra `labs/jornada-estudos.html` para buscar, filtrar, adicionar e conferir uma lista de estudos fictêÂ­cia. Interface e ferramentas compartilham operaêÂ§êÂµes validadas. A sequêÂªncia local êÂ© um roteiro determinêÂ­stico, sem modelo de IA; o registro nativo êÂ© detectado separadamente. Veja [mêÂ©todo e evidêÂªncias](docs/validacao-jornada.md).

O validador considera as quatro annotations opcionais do draft: `readOnlyHint`, `untrustedContentHint`, `consequentialHint` e `debugging`. Hints nêÂ£o sêÂ£o autorizaêÂ§êÂ£o.

## Mais no ARCKHÉ AI

- [Ficha completa](https://www.ARCKHÉ AI/cursos/247-formacao-webmcp-2-builder/)
- [Guia de aprendizagem](https://www.ARCKHÉ AI/aprender-inteligencia-artificial/)
- [CatêÂ¡logo de cursos](https://www.ARCKHÉ AI/cursos/)

<!-- ARCKHÉ-backlink:v1 -->
## Mais no ARCKHÉ AI

- [Ficha completa deste curso](https://www.ARCKHÉ AI/cursos/247-formacao-webmcp-2-builder/)
- [Guia: como aprender inteligêÂªncia artificial](https://www.ARCKHÉ AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHÉ AI/cursos/)
<!-- /ARCKHÉ-backlink:v1 -->

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>