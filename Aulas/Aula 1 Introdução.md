# Aula 1: Introdução ao Git

## O que é controle de versão?

Controle de versão é um sistema que registra modificações em arquivos ao longo do tempo, permitindo que você:

* Volte a versões anteriores;
* Compare alterações;
* Trabalhe com outras pessoas sem sobrescrever o trabalho delas.

O Git é um sistema de controle de versão distribuído, amplamente utilizado no desenvolvimento de software.

## Por que usar o Git?

* Histórico completo de mudanças
* Facilidade de colaboração
* Reversão de erros
* Trabalhar com branches (ramificações) para desenvolvimento paralelo

## Instalação do Git

### Windows

Baixe o instalador em: [https://git-scm.com/download/win](https://git-scm.com/download/win)

### macOS

Use o Homebrew:

```bash
brew install git
```

### Linux (Debian/Ubuntu)

```bash
sudo apt update
sudo apt install git
```

Após instalar, confirme:

```bash
git --version
```

## Configurações Iniciais

Configure seu nome de usuário e e-mail:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Verifique as configurações:

```bash
git config --list
```

## Criando seu primeiro repositório local

1. Crie uma nova pasta para o seu projeto:

```bash
mkdir meu-projeto && cd meu-projeto
```

2. Inicie o repositório Git:

```bash
git init
```

3. Crie um arquivo e faça o primeiro commit:

```bash
echo "# Meu Projeto" > README.md
git add README.md
git commit -m "Primeiro commit"
```

4. Veja o status e o histórico:

```bash
git status
git log
```

---

Na próxima aula, aprenderemos os **comandos básicos do Git** para controlar melhor as mudanças no seu projeto.
