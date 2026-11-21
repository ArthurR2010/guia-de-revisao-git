# guia-de-revisao-git

Mini guia de revisão de Versionamento e Colaboração.

## Integrantes

- Aluno A: Arthur Rodrigues
- Aluno B: João Gustavo

## O que tem aqui

- [glossario.md](glossario.md) — oito termos de versionamento.
- [github-flow.md](github-flow.md) — os seis passos do fluxo e explicações sobre branches e diff.
- [combinados.md](combinados.md) — dia e horário de estudo da dupla.

## Nossas respostas

### 1. O diff

No commit “Inclui exemplo na definição de commit”, vimos em vermelho a linha “- **Commit:** registro de um conjunto de mudanças. A mensagem do commit ajuda a entender o que foi feito.” e em verde a linha “- **Commit:** registro de um conjunto de mudanças. A mensagem ajuda a entender o que foi feito. Por exemplo, `Corrige o título do glossário` indica qual parte do arquivo mudou.
”. O vermelho mostra as linhas removidas e o verde mostra as linhas adicionadas.

### 2. O conflito

Um conflito acontece quando o Git precisa de ajuda para combinar mudanças. No nosso caso, nós dois partimos da mesma versão de `combinados.md` e colocamos dias diferentes na mesma linha.

O marcador `<<<<<<< docs/dia-b` mostrava onde começava a proposta de B. O `=======` separava as duas versões. O `>>>>>>> main` mostrava onde terminava a versão que veio da `main`.

A linha final ficou “Dias de estudo: terça e quinta”. Escolhemos essa versão porque proporciona maior volume de estudo e revisão do conteúdo para fixação.

### 3. A revisão

- O Aluno A recebeu: “A diferença entre Git e GitHub ficou clara. Na definição de commit, acho que um exemplo de mensagem ajudaria a entender como ela descreve uma mudança.
”.
- O Aluno B recebeu: “Consegui acompanhar a ordem dos passos. No passo 4, você pode explicar em qual branch a gente faz o ajuste e onde o novo commit aparece?”.

No glossário, o comentário foi específico, reconheceu a clareza na diferença entre Git e GitHub e sugeriu incluir um exemplo de mensagem na definição de commit. No GitHub Flow, o comentário também foi específico, reconheceu a estrutura da sequência dos passos, que permitiu acompanhá-los, e sugeriu uma explicação sobre qual branch o colaborador faz o ajuste e o local em que o novo commit é mostrado. Nos dois PRs, usamos `Request changes` para pedir o ajuste e `Approve` depois de conferir o novo commit.

### 4. Segurança

Se um telefone fosse publicado e apagado no commit seguinte, alguém ainda poderia encontrar o número no commit anterior, pois ele continuaria no histórico do repositório público. Senhas e endereços residenciais também devem ficar fora do repositório.
