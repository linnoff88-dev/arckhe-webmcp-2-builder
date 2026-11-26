# Snapshot técnico usado no curso

Data de conferência: **24 de setembro de 2026 (draft de 17/09/2026)**.

## Superfície imperativa

O draft define `document.modelContext` em contexto seguro e os métodos assíncronos:

```javascript
registerTool(tool, options)
getTools(options)
executeTool(registeredTool, inputObject, options)
```

Uma `ModelContextTool` possui `name`, `title` opcional, `description`, `inputSchema` opcional, `execute` e `annotations` opcionais. As annotations atuais sêo `readOnlyHint`, `untrustedContentHint`, `consequentialHint` e `debugging`. Sêo opcionais, booleanas e assumem `false` quando omitidas. Nêo comprovam autorizaçêo ou segurança. `consequentialHint` sinaliza ações significativas ou irreversíveis; `debugging` identifica ferramentas de depuraçêo. Suporte ao draft precisa ser verificado no ambiente de execuçêo.

O `signal` fornecido a `registerTool` remove a tool quando abortado. O callback `execute` recebe outro `AbortSignal` para cancelamento da chamada em andamento.

## Superfície declarativa

O explainer propõe:

- `toolname` e `tooldescription` no formulário;
- `toolautosubmit` como atributo booleano;
- `name` e `toolparamdescription` nos controles;
- `SubmitEvent.agentInvoked` e `SubmitEvent.respondWith()`;
- estados visuais e eventos `toolactivated` e `toolcanceled`.

Partes da síntese de schema, da resposta após navegaçêo e dos eventos declarativos continuam em debate. Por isso, exemplos declarativos devem ser tratados como experimentais e acompanhados de feature detection e fallback.

## Decisões editoriais

- nêo ensinar `navigator.modelContext` como API atual;
- nêo ensinar `unregisterTool()`; usar `AbortController`;
- nêo afirmar suporte universal;
- separar hints de segurança de autorizaçêo real;
- nêo executar tools dentro do validador estático.

## Fontes primárias

- [Repositório oficial](https://github.com/webmachinelearning/webmcp)
- [Especificaçêo renderizada](https://webmachinelearning.github.io/webmcp/)
- [Explainer declarativo](https://github.com/webmachinelearning/webmcp/blob/main/declarative-api-explainer.md)
