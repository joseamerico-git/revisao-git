##✍️ REVISÃO DOS COMANDOS BÁSICOS DO GIT

- GIT    --> Uma ferramenta de controle de versão de códigos open-source 

- GitHub --> Um servidor de Hospedagem, em que utiliza-se o Git.



🔗 # **Tornando a pasta atual em repositório git**
```
    # Iniciando um repositório local como um repositório git
         - git URL
    
    # Buscar URL do repositório no GitHub sem especificar a brach
        - git remote add origin link

        - git remote v

```

🔗 # **Clonando um repositório do git na pasta criada**
```
    # Clonando um repositório git
         - git clone URL
    # Clonar um repositório git, especificando a brach 
        - git clone URL --branch nome-brach --single-brach

```

🔗 # **Salvando alterações em um repositório local**
``` 
   # Adicionando as alterações na árvore

   git add nome-file ou git add . 

   #Mostrando status da árvore de trabalho.
   
   git status 

   git commit -m"desc-commit"

   #Mostrar os commits
   git log

  # PASTAS VAZIAS

  inserir um arquivo vazio dentro da pasta

  touch resumos/resumos-aula1.md
  ex:
  Podemos igonorar a pasta 

  echo resumos/ > .gitignore
  
  git status

   # GIT RECONHECEER PASTAS VAZIAS
   touch aulas/.gitkeep

   git add .

   git status

   git commit -m"adiciona git igonere diretórios"



```

## DESFAZENDO COISAS

Para fazer com que o repositório iniciado com git deixe de ser um repo git

rm -rf .git 
(remove recursivamente a força) o diretório git 

## Restaurando arquivos para nossa árvore

Para retornar o estado de um arquivo.
atenção...
descarta todas as alterações feitas localmente.

git restore

## Alterando mensagem de commits
1 - git commit amend -m"novadescricao"
ou
2 - git commit --amend (vai abrir o editor VIM para você)

## DESFAZER O COMMIT VOLTANDO PARA O COMMIT ANTERIOR

git reset --soft [hash] 
retorna os arquivos para a área de preparaçaõ 
git status (mostra todos os arquivos que estavam no commit )

git resete --mixed [hash] 

(comando padrão do reset) Pega os arquivos que estavam nos commits posteriores e volta para arvore

git reset --hard [hash]

Ignorou o arquivo que estavam no meu commit anterior e desfaz eles apaga os arquivos.

comando detalhado 

git reflog

# Para remover arquivos da area de preparação
    git restore --staged nomearquivo


# Enviando e baixando alterações do GitHub
git add .
git remote add origin URL
git status 
git log
git commit -m"desccommit"
git push -u origin main (-u abreviacao de upstrean)

## Após as alterções serem feitas no repositório remoto precisamos fazer um git pull no repo local para atualizar os arquivos


git pull 
(puxar as alterações realizadas atualizando meu repositório)

## Trabalhando com Braches

Braches são ramificações do projeto. 
Criada uma brach incia-se uma nova brcah que aponta para o mesmo commit da brach de onde foi criada.


## Criando uma brach

git log 

para ver a brach e o commit
atual

git checkout -B nome-brach

## Voltar para a brech anterior

git checkout nome-brach

## Listando as brachs

git brach -v

## Mesclando as braches

git merge nome-brech

## Após mesclar as breaches

git brach -v

git -d nome-brach-a-deletar

## Ver convensões de nomeação padrão de breches e commits

## ALGUMAS SITUAÇÕES QUE POSSAM OCORRER

 - CONFLITOS DE MERGE
 Existem alterações no repositório remoto que ainda não estão no repositório local

 git pull mostrará o conflito

 nos cabe decidir qual alteração permanece vigente.

 














[artigo dio]("https://web.dio.me/articles")
[Diana Martini](https://github.com/DianaMartine/curso-dio-sintaxe-basica-javascript)