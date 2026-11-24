# Cenários de teste

> Condições, ações e resultados abaixo são rascunhos. O grupo deve revisar e ajustar à modelagem escolhida.

| ID | Cenário | Condição inicial | Ação | Resultado esperado | Caso de uso | Regra |
|---|---|---|---|---|---|---|
| CT-01 | Rejeitar relato sem categoria ou descrição | Participante identificado | Registrar relato sem categoria ou sem descrição | Rejeitado com erro de regra de negócio; nada é salvo | UC-01 | RN-01 |
| CT-02 | Impedir relato duplicado de si mesmo | Relato existente A | Marcar A como duplicado de A | Rejeitado; situação de A inalterada | UC-03 | RN-02 |
| CT-03 | Impedir início de ação sem responsável | Ação planejada sem responsável | Iniciar a ação | Rejeitado; ação continua planejada | UC-04, UC-05 | RN-04 |
| CT-04 | Não resolver relato só porque a ação foi concluída | Ação em execução vinculada a um relato | Concluir a ação | Relato vai para "Aguardando verificação", não "Resolvido" | UC-05 | RN-06 |
| CT-05 | Impedir resolução sem verificação e evidência | Relato aguardando verificação | Resolver sem evidência ou sem verificação | Rejeitado; relato continua aguardando | UC-07 | RN-07 |
| CT-06 | Impedir verificação final pelo responsável pela conclusão | Ação concluída por participante P | P tenta registrar a verificação final | Rejeitado | UC-06 | RN-08 |
| CT-07 | Permitir resolução quando as condições forem atendidas | Relato aguardando verificação, verificador diferente de P | Registrar verificação positiva com evidência e justificativa | Relato fica "Resolvido"; autor, data e justificativa no histórico | UC-06, UC-07 | RN-05, RN-07, RN-08 |
| CT-08 | Permitir reabertura justificada preservando histórico | Relato resolvido | Reabrir com nova evidência ou justificativa | Relato volta para análise; histórico anterior preservado | UC-07 | RN-09 |
| CT-09 | Rejeitar alteração por participante sem permissão | Participante sem permissão | Tentar alterar responsável ou registrar verificação restrita | Rejeitado por autorização | UC-04, UC-06 | RN-11 |
| CT-10 | Evidência pública sem dados pessoais | [PREENCHER] | [PREENCHER] | [PREENCHER] | UC-02 | RN-12 |
| CT-11 | Arquivar com motivo preservando histórico | [PREENCHER] | [PREENCHER] | [PREENCHER] | UC-07 | RN-10 |
