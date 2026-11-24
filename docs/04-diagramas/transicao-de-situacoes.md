# Transição de situações do Relato de Barreira

> Rascunho baseado no fluxo sugerido no enunciado, com retornos, reabertura e arquivamento. O grupo deve revisar cada transição.

```mermaid
stateDiagram-v2
    state "Em análise" as EmAnalise
    state "Ação planejada" as AcaoPlanejada
    state "Em execução" as EmExecucao
    state "Aguardando verificação" as AguardandoVerificacao

    [*] --> Registrado
    Registrado --> EmAnalise : encaminhar para análise
    EmAnalise --> AcaoPlanejada : definir responsável e planejar ação
    AcaoPlanejada --> EmExecucao : iniciar ação
    EmExecucao --> AguardandoVerificacao : concluir ação
    AguardandoVerificacao --> Resolvido : verificação positiva com evidência e justificativa

    AcaoPlanejada --> EmAnalise : retornar para análise
    EmExecucao --> EmAnalise : retornar para análise
    AguardandoVerificacao --> EmExecucao : verificação negativa
    Resolvido --> EmAnalise : reabrir com nova evidência ou justificativa

    Registrado --> Arquivado : arquivar com motivo
    EmAnalise --> Arquivado : arquivar com motivo
    Resolvido --> Arquivado : arquivar com motivo
    Arquivado --> [*]
```

## Tabela de transições
| De | Para | Quem pode | Exige | Regra |
|---|---|---|---|---|
| Registrado | Em análise | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Em análise | Ação planejada | [PREENCHER] | Responsável definido | RN-04 |
| Ação planejada | Em execução | [PREENCHER] | Objetivo e responsável | RN-04 |
| Em execução | Aguardando verificação | [PREENCHER] | Conclusão da ação | RN-06 |
| Aguardando verificação | Resolvido | Verificador diferente de quem concluiu | Evidência e justificativa | RN-07, RN-08 |
| Resolvido | Em análise (reabertura) | [PREENCHER] | Nova evidência ou justificativa | RN-09 |
| Qualquer | Arquivado | [PREENCHER] | Motivo | RN-10 |

## Duplicidades
Relatos duplicados mantêm o registro original e apontam para o relato de referência. Evitar ciclos entre referências: [PREENCHER: como o grupo vai garantir isso].
