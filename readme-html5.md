# História

Tim Bearnes 1991. versão 1.

Funcinamento do HTML

<!DOCTYPE html> não é elemento html diz ao navegador o que você esta escrevendo
<head> contem meta-informações para o navegador e buscador de internet necessita

a tag #<meta >
```
<head>
    <meta charset="utf-8">
    <title>Jose Americo<title>
</head>

```

## SEMANTICA HTML

<section> --> representa uma seção generica lista
<header>  --> cabeçalho de uma <section>
<article> --> artigo de um ex blog
<aside>   --> representa um conteúdo relacionado ao conteúdo principal da página biografi de autor etc..
<footer>  --> rodapé da página ou parte da página de um <article> ou <section> ...
<a href>  --> hiperlink pode ser uma página no site ou site externo
<a target="_blank">--> Indica como o link vai ser aberto _blank em nova haba

# Inserindo imagens no html

<img src="" alt=""> alt="descrição" o alt é altamente recomendado quando a foto não carregar vai aparecer a descrição.

## site lega unsplah
## site para melhorar img tynypng.com

## Listas em Html
<ul> -->lista em que ordem não importa
<ol> -->Ordem são extremamente importantes
<li> -->Item da lista


# Conceitos básicos CSS

 CSS --> Cria regras de estilo 

- SELETORES elementos html 
```
[seletores]
a, p, h1,h3{
    declarações ex: 
    [propriedade : valor;] ===> declarações
    color:red;
}

```
# ID X CLASSES

No html 

```
    <header id="headers" class="headers"></header>

```

No CSS 

```
  #header --> representa id
  
    #header{
        padding:15px;

    }

 .header --> representa classes

    .header{
        padding:15px;
    }

```


### OS ID(S) SÓ PODEM SER USADOS 1 VEZ NA PÁGINA 
### ENQUANTO A CLASSE VÁRIAS VEZES


 📘[Material](https://web.dio.me/course/introducao-criacao-de-websites-com-html5-e-css3/learning/b9735f52-8518-49e1-b294-1d40caeeff43?back=/track/santander-bootcamp-2023-fullstack-java-angular&tab=undefined&moduleId=undefined)

 ### Padding e Margin
 
 
 ```

  .class{           
                 eixo y  esquerdo direito
        padding: 10px           5px

                topo direita   inferior  esque
        padding: 10px     15px    5px     0;
  }

 # image com CSS
  .class{
    bakground-image:url("img/");
  }
 
 ```

 # mdn para estudar
  












