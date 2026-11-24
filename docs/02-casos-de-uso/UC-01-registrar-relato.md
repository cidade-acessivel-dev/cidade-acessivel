# UC-01: Cadastrar local e registrar relato de barreira

> Rascunho inicial para o grupo revisar e completar.

- **Objetivo:** permitir que um participante registre uma barreira de acessibilidade em um local
- **Ator:** Participante da comunidade
- **Entradas:** local (existente ou novo), categoria da barreira, descrição, evidências opcionais
- **Saída esperada:** relato criado com situação **Registrado**, com identificador, autor e data
- **Pré-condições:** participante identificado; [PREENCHER]

## Fluxo principal
1. O participante informa ou seleciona o local
2. Informa categoria e descrição
3. Anexa evidências, se houver (sem dados pessoais desnecessários)
4. O sistema valida e cria o relato na situação **Registrado**
5. O sistema registra autor e data no histórico

## Regras aplicáveis
- [RN-01](../01-dominio/regras-de-negocio.md): local, categoria e descrição compreensível
- [RN-12](../01-dominio/regras-de-negocio.md): evidências públicas sem dados pessoais

## Mudanças de estado permitidas
| De | Para | Quem pode |
|---|---|---|
| (novo) | Registrado | Participante |

## Informações que precisam ser preservadas
- Autor, data de criação e conteúdo original do relato

## Possíveis erros
| Erro | Tipo | Resposta esperada |
|---|---|---|
| Relato sem categoria ou descrição | Regra de negócio | Rejeitar com mensagem clara |
| Falha ao salvar | Falha técnica | [PREENCHER] |
| Evidência com dados pessoais expostos | Regra de negócio | [PREENCHER] |

## Cenários de teste relacionados
- [CT-01](../05-qualidade/cenarios-de-teste.md)
