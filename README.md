# HuskyBlizzard-RemapingKeys
 Remapeamento do Teclado Husky Blizzard Gaming 60%

Presta atenção!
---
xmodmap -e "keycode 47 = ccedilla Ccedilla Left" && 
---

xmodmap -e 
---
Comando do terminal chamando o xmodmap pra fazer uma troca de funções de teclas;

"keycode 47 = ccedilla Ccedilla Left"
---
Tudo o que vem entre aspas serve como argumento, ou seja, as funções a serem trocadas ou acrescidas;


keycode 47
---
É o código de tecla. Corresponde ao número através do qual o sistema identifica qual tecla foi acionada. Pra saber qual é o keycode de uma tecla, digite no terminal o comando (xev). Vai aparecer uma micro janela e tudo o que tu precisa fazer é digitar (e anotar) o resultado que vai aparecer no terminal pra identificar o keycode e os keysyms relacionados à tecla acionada;


=
---
O sinal de igualdade serve como atribuição. Igual a maioria das linguagens de programação. Serve para alterar ou acrescentar as funções desejadas ao keycode;


ccedilla Ccedilla Left
---
São os keysyms que eu quero atribuir ao keycode em questão. Nessa etapa é muito importante saber a forma certa de se escrever os keysyms. Por exemplo: ç = ccedilla, Ç = Ccedilha. E deve-se escrever com um espaço entre eles pra separar as outras funções que o mesmo keycode vai receber, como no exemplo acima. Pra saber os keycodes e seus respectivos keysyms, digite o comando (xmodmap -pke) no terminal;


&& 
---
É um concatenador de comandos, indicando que o comando ainda não acabou e que o sistema operacional deve ler e executar o próximo em seguida. Porém, o comando para de ser executado se um deles estiver incorreto.
