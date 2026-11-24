# Arquitetura proposta

O objetivo é permitir que o sistema evolua sem depender de uma interface ou banco de dados específico para que as regras sejam compreendidas.

## Camadas e responsabilidades

| Camada | Papel | O que NÃO deve conter |
|---|---|---|
| Domínio | Entidades, objetos de valor, agregados e regras de negócio | Acesso a banco, HTTP, detalhes de tela |
| Casos de uso (aplicação) | Orquestram o domínio para cada objetivo do usuário | Regras de negócio duplicadas |
| Interfaces de entrada | API, telas e outras entradas que chamam os casos de uso | Regras de negócio |
| Infraestrutura | Persistência, armazenamento de evidências, integrações | Decisões de negócio |

[PREENCHER: ajuste os nomes e as responsabilidades conforme a escolha do grupo]

## Onde cada coisa acontece

| Preocupação | Onde ocorre | Justificativa |
|---|---|---|
| Regras de negócio | [PREENCHER] | [PREENCHER] |
| Validação de formato | [PREENCHER] | [PREENCHER] |
| Verificação de permissões | [PREENCHER] | [PREENCHER] |
| Persistência | [PREENCHER] | [PREENCHER] |
| Integrações futuras | [PREENCHER] | [PREENCHER] |
| Histórico de mudanças | [PREENCHER] | [PREENCHER] |

> Ocultar um botão na interface não substitui a autorização no backend.

## Como o projeto poderá evoluir
[PREENCHER: backend, frontend, mobile e integrações, conforme a ementa. Microsserviços só com justificativa explícita.]
