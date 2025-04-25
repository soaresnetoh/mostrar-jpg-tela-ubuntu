# mostrar-jpg-tela-ubuntu
Mostrar um jpg na tela principal do seu ubuntu de tempos em tempos, usando cron


Para exibir um jpeg na tela do ubuntu, precisa:

```
sudo apt update
sudo apt install feh
```

Colocar no cron 

```
0 6-13 * * * DISPLAY=:0 /home/usuario/mensagens/exibir-imagem.sh /home/usuario/mensagens/bom-dia.jpg
30 */2 * * * DISPLAY=:0 /home/usuario/mensagens/exibir-imagem.sh /home/usuario/mensagens/beber-agua.jpg
```