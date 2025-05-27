# Aula 5: Boas Práticas com Git e GitHub

Nesta aula, abordaremos práticas recomendadas para manter seus repositórios organizados, seguros e colaborativos.

## Escrevendo boas mensagens de commit

- Seja claro e objetivo.
- Use o imperativo (ex: "Corrige bug na função de login").
- Inclua contexto, se necessário.

Exemplo:

```bash
git commit -m "Adiciona validação de e-mail no formulário de cadastro"
```

## Usando o `.gitignore`

Evite subir arquivos desnecessários (logs, arquivos temporários, dependências, etc.).

Crie um arquivo `.gitignore` na raiz do projeto com conteúdo como:

```
node_modules/
*.log
.env
.DS_Store
```

Você pode gerar automaticamente em: https://www.toptal.com/developers/gitignore

## Commits pequenos e frequentes

- Faça commits com mudanças coesas.
- Evite commits grandes e confusos.
- Ajuda no rastreamento de bugs e revisão de código.

## Branches para cada funcionalidade ou correção

- Crie uma branch para cada tarefa (feature, bugfix, etc.).
- Nomeie de forma descritiva: `feature/login`, `fix/validacao-email`

## Pull Requests (PRs) claros

- Escreva títulos objetivos.
- Descreva as alterações realizadas.
- Peça revisão antes de fazer o merge na branch principal.

## Evite subir arquivos sensíveis

Nunca adicione arquivos como `.env` com senhas ou chaves de API. Use o `.gitignore` e armazene essas informações de forma segura.

## Sincronize com frequência

- Use `git pull` para manter seu repositório atualizado.
- Resolva conflitos imediatamente para evitar acúmulo.

------

Com estas práticas, seu fluxo de trabalho com Git e GitHub será mais limpo, produtivo e seguro. Parabéns por concluir o mini curso! 🎉

Se quiser expandir o conteúdo, considere aulas sobre Git Flow, rebase, squash, tags e CI/CD.