# Publicação na branch entrega-1

Execute no terminal aberto na pasta do seu repositório. Não foi executada nenhuma alteração remota por esta assistência.

1. Confira localização, alterações e remoto:

```sh
git status
git branch --show-current
git remote -v
```

Se aparecer "not a git repository", abra a pasta correta do repositório. Não inicialize outro repositório por engano. Se houver alterações de outro trabalho, preserve-as antes de misturar esta entrega.

2. Crie a branch antes de copiar os arquivos:

```sh
git switch -c entrega-1
```

Se ela já existir localmente, use `git switch entrega-1`. Se existir apenas no GitHub: `git fetch origin` e `git switch --track origin/entrega-1`. Não execute alternativas se o primeiro comando já funcionou.

3. Extraia o ZIP fora do repositório. Copie o conteúdo da pasta do projeto para a raiz do repositório, não o ZIP nem uma pasta extra. Faça uma cópia de segurança fora do repositório antes de substituir um index.html existente. Não apague a pasta .git. Preserve outros arquivos não relacionados.

4. Abra index.html, revise as páginas e realize o checklist. Complete os resultados reais antes do commit.

5. Confira e adicione apenas os arquivos da entrega:

```sh
git status
git add index.html programacao.html palestrantes.html inscricao.html README.md estrutura.txt img docs
git diff --cached --stat
git diff --cached
```

Confira se o diff contém somente os arquivos esperados, inclusive porque img e docs podem já conter outros arquivos no seu repositório. Não publique senhas ou dados pessoais.

6. Crie o commit e publique:

```sh
git commit -m "Entrega 1: quatro paginas HTML semanticas e checklist"
git push -u origin entrega-1
```

Se origin não existir, primeiro copie a URL real do seu repositório no GitHub e configure com `git remote add origin URL_REAL_DO_REPOSITORIO`. Não execute esse comando com o marcador literal. Se o push for recusado, leia o erro; não use --force para resolver sem investigar.

7. No GitHub, selecione entrega-1 e confira os quatro HTML, img e docs. Copie da barra de endereço o link da branch (termina em /tree/entrega-1). Envie esse link na atividade. Não é necessário ativar GitHub Pages para fornecer o link do repositório pedido.

Referências: https://git-scm.com/docs/git-switch e https://docs.github.com/en/contributing/collaborating-on-github-docs/using-git-on-github-docs
