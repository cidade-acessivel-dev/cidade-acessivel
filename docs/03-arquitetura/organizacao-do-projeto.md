# Organização do projeto

> Estrutura **conceitual** para as próximas fases. Nada disto precisa estar implementado agora.

```
src/
├── domain/              # entidades, objetos de valor, agregados, regras
│   ├── relato/
│   ├── acao/
│   └── shared/
├── application/         # casos de uso e contratos (interfaces)
│   ├── use-cases/
│   └── ports/
├── interfaces/          # entradas: API, CLI, web
└── infrastructure/      # banco, armazenamento de evidências, integrações
tests/
├── unit/                # regras e transições de situação
├── integration/         # persistência, permissões, histórico
└── e2e/                 # fluxos completos
```

## Responsabilidade de cada pasta
| Pasta | Responsabilidade |
|---|---|
| `domain` | [PREENCHER] |
| `application` | [PREENCHER] |
| `interfaces` | [PREENCHER] |
| `infrastructure` | [PREENCHER] |
| `tests` | [PREENCHER] |

## Por que esta organização
[PREENCHER: como ela facilita localizar artefatos, manter nomes coerentes e evitar regras espalhadas]
