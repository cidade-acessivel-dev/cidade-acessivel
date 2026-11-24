# Regras de negócio

> Proposta inicial baseada no enunciado. O grupo pode refinar, acrescentar e remover regras. Para cada regra, indique onde será aplicada na arquitetura e como será validada.

| ID | Regra | Onde será aplicada | Como validar |
|---|---|---|---|
| RN-01 | Um relato precisa conter local, categoria e descrição compreensível | [PREENCHER] | [PREENCHER] |
| RN-02 | Um relato não pode ser marcado como duplicado de si mesmo | [PREENCHER] | [PREENCHER] |
| RN-03 | Relacionar duplicidades preserva os registros e indica o relato de referência | [PREENCHER] | [PREENCHER] |
| RN-04 | Uma ação deve ter objetivo e responsável antes de ser iniciada | [PREENCHER] | [PREENCHER] |
| RN-05 | Mudanças de situação registram autor, data e justificativa quando exigida | [PREENCHER] | [PREENCHER] |
| RN-06 | Concluir uma ação não significa, por si só, resolver a barreira relatada | [PREENCHER] | [PREENCHER] |
| RN-07 | Um relato só pode ser resolvido após verificação com evidência e justificativa | [PREENCHER] | [PREENCHER] |
| RN-08 | A verificação final é registrada por participante diferente do responsável que informou a conclusão da ação | [PREENCHER] | [PREENCHER] |
| RN-09 | Reabrir um relato resolvido exige nova evidência ou justificativa verificável | [PREENCHER] | [PREENCHER] |
| RN-10 | Arquivar um relato exige motivo e não apaga seu histórico | [PREENCHER] | [PREENCHER] |
| RN-11 | Participante sem permissão não altera responsáveis nem registra verificações restritas | [PREENCHER] | [PREENCHER] |
| RN-12 | Evidências para consulta pública não expõem rostos, documentos ou dados pessoais desnecessários | [PREENCHER] | [PREENCHER] |

## Fluxo de situações
Ver [diagrama de transição](../04-diagramas/transicao-de-situacoes.md).

## Tratamento de duplicidades sem ciclos
[PREENCHER: como evitar que A aponte para B e B para A, ou cadeias circulares]

## Regra de negócio, validação de formato e controle de interface
Regras de negócio vivem no domínio. Validações de formato (ex.: campo vazio, tamanho) ficam nas bordas. Ocultar um botão na interface **não** substitui a autorização no backend.
