# Aplicação de JavaScript Avançado e TypeScript

Como cada conhecimento da fase será usado na implementação futura. Os trechos de código abaixo são **conceituais**.

| Recurso | Como será usado | Justificativa |
|---|---|---|
| Tipagem estática | [PREENCHER] | [PREENCHER] |
| Interfaces | [PREENCHER] | [PREENCHER] |
| Classes | [PREENCHER] | [PREENCHER] |
| Enums ou uniões de tipos | [PREENCHER] | [PREENCHER] |
| Funções puras | [PREENCHER] | [PREENCHER] |
| Módulos ES6+ | [PREENCHER] | [PREENCHER] |
| async / await | [PREENCHER] | [PREENCHER] |
| Generics | [PREENCHER] | [PREENCHER] |
| Tratamento de erros | [PREENCHER] | [PREENCHER] |
| Tipos e contratos compartilhados | [PREENCHER] | [PREENCHER] |

## Falhas técnicas vs violações de regra
[PREENCHER: como o código vai distinguir um erro de infraestrutura de uma regra de negócio violada]

## Exemplo conceitual (rascunho para o grupo discutir)

```ts
// CONCEITUAL: não faz parte de uma implementação real

type SituacaoRelato =
  | "REGISTRADO"
  | "EM_ANALISE"
  | "ACAO_PLANEJADA"
  | "EM_EXECUCAO"
  | "AGUARDANDO_VERIFICACAO"
  | "RESOLVIDO"
  | "ARQUIVADO";

// Função pura: não depende de efeitos externos
function relatoTemDadosMinimos(r: { localId?: string; categoria?: string; descricao?: string }): boolean {
  return Boolean(r.localId && r.categoria && r.descricao && r.descricao.trim().length > 0);
}
```
