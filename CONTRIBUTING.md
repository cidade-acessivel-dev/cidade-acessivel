# Como trabalhamos neste repositório

## Antes do primeiro commit
Configure no Git o **mesmo e-mail da sua conta do GitHub**. Sem isso, os commits não aparecem no seu perfil.

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email-do-github@exemplo.com"
```

## Fluxo de trabalho
1. Atualize a branch principal: `git pull`
2. Crie uma branch para o que for fazer: `git checkout -b docs/glossario`
3. Faça commits pequenos, com mensagens claras (ex.: `docs: define termos do glossário`)
4. Envie a branch: `git push -u origin docs/glossario`
5. Abra um Pull Request e peça revisão de pelo menos uma pessoa do grupo
6. Depois de aprovado, faça o merge e apague a branch

## Convenções
- Nome de branch: `docs/assunto`, `diagrama/assunto` ou `fix/assunto`
- Arquivos e pastas em minúsculas, com hífen, sem acento (ex.: `regras-de-negocio.md`)
- Trechos de código em TypeScript são **conceituais**: indique isso no cabeçalho
- Procure por `[PREENCHER]` para encontrar o que ainda falta escrever

## Responsáveis por área
| Área | Responsável |
|---|---|
| Domínio e glossário | [PREENCHER] |
| Casos de uso | [PREENCHER] |
| Arquitetura | [PREENCHER] |
| Diagramas | [PREENCHER] |
| Qualidade e testes | [PREENCHER] |
| Roadmap e vídeo | [PREENCHER] |
