# Aula 2: Comandos Básicos do Git

Nesta aula, vamos explorar os comandos essenciais do Git para controlar as alterações no seu projeto localmente.

## `git init`

Inicializa um novo repositório Git.

```bash
git init
```

Cria um diretório oculto `.git` que contém todo o histórico do repositório.

## `git status`

Exibe o estado atual do repositório, incluindo arquivos modificados, novos arquivos não rastreados, etc.

```bash
git status
```

## `git add`

Adiciona arquivos ao staging (área de preparação para o commit).

```bash
git add nome-do-arquivo
# ou para adicionar todos os arquivos modificados:
git add .
```

## `git commit`

Salva o snapshot dos arquivos que estão no staging.

```bash
git commit -m "mensagem do commit"
```

## `git log`

Exibe o histórico de commits.

```bash
git log
```

## `git diff`

Mostra as diferenças entre os arquivos modificados e o último commit.

```bash
git diff
```

## `git checkout`

Restaura arquivos ou troca de branches. Exemplo de uso para voltar a uma versão anterior:

```bash
git checkout <id_do_commit>
```

## `git reset`

Desfaz commits.

```bash
git reset --soft <id_do_commit>   # mantém alterações no staging
git reset --hard <id_do_commit>   # remove tudo após o commit especificado
```

⚠️ Use com cuidado: `--hard` pode causar perda de dados locais.

------

Na próxima aula, veremos como conectar seu repositório local ao GitHub e utilizar repositórios remotos!