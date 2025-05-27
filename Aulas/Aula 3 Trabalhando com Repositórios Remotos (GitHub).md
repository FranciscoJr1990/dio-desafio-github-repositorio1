# Aula 3: Trabalhando com Repositórios Remotos (GitHub)

Nesta aula, vamos aprender como conectar seu repositório local ao GitHub, enviar alterações e colaborar com outras pessoas.

## Criando um repositório no GitHub

1. Acesse [https://github.com](https://github.com/) e faça login.
2. Clique em **New repository**.
3. Escolha um nome, defina a visibilidade (público ou privado) e clique em **Create repository**.

## Conectando o repositório local ao GitHub

Copie o endereço do repositório remoto (HTTPS ou SSH). Exemplo:

```bash
git remote add origin https://github.com/seuusuario/meu-projeto.git
```

Verifique se foi adicionado corretamente:

```bash
git remote -v
```

## Enviando (push) para o GitHub

Envie os commits locais para o repositório remoto:

```bash
git push -u origin main
```

> Use `main` ou `master`, dependendo do nome da sua branch principal.

## Clonando um repositório existente

Para copiar um projeto hospedado no GitHub para seu computador:

```bash
git clone https://github.com/usuario/repositorio.git
```

## Atualizando o repositório local com `pull`

Para trazer as alterações do repositório remoto:

```bash
git pull origin main
```

## Colaborando em equipe

- Use branches para desenvolver funcionalidades sem afetar o código principal.
- Faça commits claros e frequentes.
- Utilize `pull` regularmente para manter seu código atualizado.

------

Na próxima aula, aprenderemos sobre **branches**, como criá-las, alternar entre elas e fazer merge (junção) com a branch principal.