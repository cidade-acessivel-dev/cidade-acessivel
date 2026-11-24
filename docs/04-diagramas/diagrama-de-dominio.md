# Diagrama de domínio

> Rascunho inicial em Mermaid para o grupo ajustar. O GitHub renderiza este bloco automaticamente.

```mermaid
classDiagram
    class Local {
        id
        nome
        localizacao
    }
    class RelatoDeBarreira {
        <<Aggregate Root>>
        id
        categoria
        descricao
        situacao
        autorId
        referenciaDuplicidadeId
    }
    class Evidencia {
        id
        tipo
        publica
    }
    class Verificacao {
        id
        resultado
        justificativa
        verificadorId
    }
    class AcaoDeMelhoria {
        <<Aggregate Root>>
        id
        objetivo
        responsavelId
        periodoPrevisto
        andamento
    }
    class Participante {
        id
        nome
        papeis
    }

    RelatoDeBarreira "1" *-- "0..*" Evidencia : fundamenta
    RelatoDeBarreira "1" *-- "0..*" Verificacao : registra
    RelatoDeBarreira ..> Local : referencia por id
    RelatoDeBarreira ..> Participante : autor, por id
    RelatoDeBarreira ..> RelatoDeBarreira : duplicado de (por id)
    AcaoDeMelhoria "1" ..> "1..*" RelatoDeBarreira : atende, por id
    AcaoDeMelhoria ..> Participante : responsável, por id
```

## Legenda
- Linha cheia com losango: pertence ao limite do agregado
- Linha pontilhada: apenas referência por identificador

## Decisões a registrar
- [PREENCHER: por que Ação de Melhoria é (ou não) um agregado próprio]
- [PREENCHER: o que decidimos deixar fora do agregado Relato]
