+++
title = "Comandos úteis diários no terminal Linux"
date = "2019-07-12"
author = "Alexandre"
cover = "hello.jpg"
description = "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nec interdum metus. Aenean rutrum ligula sodales ex auctor, sed tempus dui mollis. Curabitur ipsum dui, aliquet nec commodo at, tristique eget ante."
+++

Utilizo o Linux diariamente no trabalho ou em casa, seguido do terminal que está sempre aberto, uma ferramenta indispensavel na vida de um desenvolvedor.

Irei listar aqui alguns comandos e atalhos úteis que utilizado diariamente no terminal Linux.

- history
O `history` é um ótimo comando para listar o histórico de seus últimos comandos executados no términal. Perfeito para identificar o que foi feito nos últimos comandos ou para relembrar de algum comando esquecido.

- Atalho CTRL+R
Assim como `history` que mostra o histórico de comandos executados, esse atalho permite realizar uma busca pelo comando que algum momento foi executado. Basta digitar uma parte do comando e lhe dará as sujestões e quando encontrar basta teclar 'Enter'.

- cat
O `cat` permite visualizar o conteúdo de um arquivo. Ele basicamente abrirá e terminará a execução no final do arquivo, sem a opção de interagir. Ex.: `cat log/production.txt`

- tail
O `tail` é muito semelhante ao `cat`, mas ele permite abrir um arquivo e visualizar o seu conteúdo em tempo real, caso seja realizado alguma alteração. Ele é uma ótima solução para visualização de logs para acompanhamento em tempo real ou limitar o número de linhas. No exemplo abaixo o parametro `-f` o arquivo continua aberto e o `-n 500` limita para as últimas 500 linhas. 
Ex.: `tail -f -n 500 log/production.txt`

- grep
O `grep` pode ser utilizado junto com o `cat` ou `tail` que permite buscar um conteúdo especifico de dentro de um arquivo. Existem inúmeros maneiras de realizar uma busca com o `grep`, possibilitando o uso de regex, limitadores e outros. Um exemplo básico de seu uso: `cat log/production.txt | grep 'exception'`

- ps aux
O `ps aux` permite visualizar todos os processos do sistema operacional. Junto com o `grep` permite buscar por processos especificos. Muito útil quando precisa encontrar algum processo para finalizar. 
Ex.: `ps aux | grep firefox` 

- kill
O `kill` literalmente serve para matar 