---
title: ShellScript Hints `#1` - Parâmetros
date: 2021-04-29 23:00:00 +/-TTTT
categories: [programming,shellscript]
tags: [hints, dicas, shellscript]     # TAG names should always be lowercase
---

![Python](/assets/img/bash.png)

#### Hints: 

1. Parâmetros\
   Podemos representar os parâmetros passados durante a execução do script utilizando:
    
    $1 - Primeiro Parâmetro \
    $2 - Segundo Parâmetro  
    $3 - Terceiro Parâmetro\
    <small>e assim por diante...</small>
    
    Para representar todos os parâmetros de uma vez só, podemos utilizar `$@`
    
    Utilizaremos o seguinte script como exemplo:
    
        #!/bin/bash

        echo -e "Este script foi criado para printar os parâmetros passados pelo usuário.\n"

        echo "O primeiro parâmetro passado foi: " $1
        echo "O segundo parâmetro passado foi: " $2
        echo -e "O terceiro parâmetro passado foi:  $3\n "

        echo "A seguir, temos todos os parâmetros passados: " $@

    Para testar, execute o script passando os parâmetros desejados:\
    ![Parameters](/assets/gif/parameters.gif)


