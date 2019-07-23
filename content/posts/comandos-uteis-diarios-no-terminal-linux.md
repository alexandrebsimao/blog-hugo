+++
title = "Comandos úteis diários no terminal Linux"
date = "2019-07-15"
author = "Alexandre"
cover = "hello.jpg"
description = "Comandos úteis de uso diário no terminal Linux."
+++

Utilizo o Linux diariamente no trabalho ou em casa, seguido do terminal que está sempre aberto, uma ferramenta indispensavel na vida de um desenvolvedor.

Irei listar aqui alguns comandos e atalhos úteis que utilizo diariamente no terminal Linux.

- history
O `history` é um ótimo comando para listar o histórico de seus últimos comandos executados no términal. Perfeito para identificar o que foi feito nos últimos comandos ou para relembrar de algum comando esquecido.

- Atalho CTRL+R
Assim como `history` que mostra o histórico de comandos executados, esse atalho permite realizar uma busca pelo comando que algum momento foi executado. Basta digitar uma parte do comando e lhe dará as sujestões e quando encontrar basta teclar 'Enter'.

- cat
O `cat` permite visualizar o conteúdo de um arquivo. Ele basicamente abrirá e terminará a execução no final do arquivo, sem a opção de interagir. Ex.: `cat log/production.txt`

- tail
O `tail` é muito semelhante ao `cat`, mas ele permite abrir um arquivo e visualizar o seu conteúdo em tempo real, caso seja realizado alguma alteração. Ele é uma ótima solução para visualização de logs para acompanhamento em tempo real ou limitar o número de linhas. No exemplo abaixo o parâmetro `-f` o arquivo continua aberto e o `-n 500` limita para as últimas 500 linhas. 
Ex.: `tail -f -n 500 log/production.txt`

- grep
O `grep` pode ser utilizado junto com o `cat` ou `tail` que permite buscar um conteúdo especifico de dentro de um arquivo. Existem inúmeros maneiras de realizar uma busca com o `grep`, possibilitando o uso de regex, limitadores e outros. Um exemplo básico de seu uso: `cat log/production.txt | grep 'exception'`

- cd
O `cd` serve para navegar entre diretórios. Por exemplo, quero acessar o diretório de downloads via terminal, eu digito `cd ~/Downloads`.

- ls
O `ls` lista todos os objetos dentro da pasta atual ou de alguma pasta que se referir. Por exemplo, estou dentro da pasta de downloads e digito ls, será listado os objetos da pasta. Também podemos informar o caminho que queremos ver o conteúdo da pasta. Ex.: `ls ~/Documentos`

- mkdir
O `mkdir` tem como função criar uma pasta. Sua função é bem simples. Se estou dentro da pasta Documentos e informar `mkdir Projetos`, será criado a pasta Projetos dentro da minha pasta Documentos. Também posso adicionar o diretório caso eu não esteja dentro da pasta especifica. Por exemplo, estou na pasta de Documentos mas quero criar uma pasta de Thumbnails dentro da pasta Imagens `mkdir ~/Imagens/Thumbnails`.

- rm
O `rm` remove um arquivo ou pasta. Sua função é bem simples. `rm Thumbnails`. Se for remover alguma pasta que tenha arquivos dentro e você tem certeza que queira remover, deve informar no comando que a remoção será recursiva. TENHA CUIDADO E CONSIÊNCIA NO USO DESSE COMANDO, POIS REMOVE TODO O CONTEÚDO DENTRO DA PASTA. `rm -r Thumbnails`.

- mv
O `mv` serve para mover pastas e arquivos. Basta informar a origem e o destino. Ex.: `mv ~/Imagens/Thumbnails ~/Projetos/Thumbnails`. É importante informar o nome do arquivo ou da pasta também no destino. Dessa forma você também pode aproveitar para renomear o objeto.

- cp
O `cp` funciona da mesma forma que o `mv`, mas para copias. Ex.: `cp ~/Imagens/Thumbnails ~/Projetos/Thumbnails`.

Existem muitos outros que facilitam a vida no uso do sistema, mas esses são alguns dos comandos básicos de uso diário no terminal Linux.

Até mais!