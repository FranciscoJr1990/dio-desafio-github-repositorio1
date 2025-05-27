# Aula 4: Branches e Merge

Branches (ramificações) permitem trabalhar em novas funcionalidades ou correções de forma isolada, sem afetar o código principal. Nesta aula, aprenderemos a criar, alternar, juntar e excluir branches.

## Criando uma nova branch

```bash
git branch nome-da-branch
```

## Alternando entre branches

```bash
git checkout nome-da-branch
```

Ou crie e já altere:

```bash
git checkout -b nome-da-branch
```

## Listando branches

```bash
git branch
```

A branch atual estará marcada com um asterisco `*`.

## Fazendo merge de uma branch

1. Volte para a branch principal (ex: `main`):

```bash
git checkout main
```

1. Junte a outra branch:

```bash
git merge nome-da-branch
```

## Lidando com conflitos

Se dois arquivos foram modificados em linhas semelhantes, o Git solicitará que você resolva os conflitos manualmente. Após resolver:

```bash
git add arquivo-conflitante
git commit -m "Resolve conflitos"
```

## Excluindo uma branch

Após fazer o merge:

```bash
git branch -d nome-da-branch
```

## Dica: Usando branches com GitHub

- Crie uma branch localmente, suba para o GitHub:

```bash
git push -u origin nome-da-branch
```

- Abra um Pull Request no GitHub para revisão e merge.

------

Na próxima aula, veremos **boas práticas de Git e GitHub**, incluindo mensagens de commit, uso de `.gitignore` e colaboração eficiente.