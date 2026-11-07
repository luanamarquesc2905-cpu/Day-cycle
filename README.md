Inicialmente tinha a intenção de criar uma bandeira com o código "if" "else" porém, não estava a conseguir chegar ao resultado desejado. 
Ao experimentar com o "random" e "mouseX" "mouseY", tive a ideia de tentar recriar um ciclo do dia.
O objetivo era criar um círculo que seguisse o cursor, encontrei algumas dificuldades mas estudei alguns códigos disponíveis online e acabei por conseguir.
As únicas partes onde utilizei copypaste do tutorial foi o "let=ball", "let x=0", "let y=0",  "x += (mouseX - x) * 1" e "y += (mouseY - y) * 1".
Para o céu, desenhei um retângulo com a largura da janela e metade da altura da mesma, e, 
usando o "if" "else",  se o "mouseX" fosse menor que o windowWidth/2, o mesmo seria azul claro, se não cumprisse com a condição, 
este seria um violeta a imitar um pôr-do-sol. 
A seguir defini as cores do meu sol/lua, com a seguinte condição: se o "mouseX" fosse menor que o windowWidth/2 o círculo seria amarelo (sol)
porém, se o "mouseX" fosse maior do que o windowWidth/2, este seria então um branco ligeiramente azulado (lua).
Para a relva, desenhei um outro retângulo com a largura da janela, mas que se situasse na metade inferior da mesma. Se o "mouseX" fosse menor do
que o windowWidth/2 então teria um verde mais vivo, se não, seria um verde mais escuro com uma presença de azul, a imitar a iluminação noturna.
Após estes processos todos eu não estava satisfeita, queria que a ausência do sol e da lua trouxesse uma escuridão, para isso inseri um "if" 
dentro do primeiro "if", cuja condição era: se o "mouseY" fosse maior do que o windowHeight/2 o céu se transformava num azul escuro. Quando
testei, parecia estar tudo bem até ultrapassar com o cursor o windowWidth/2, tentei então aplicar, no retângulo da relva, a seguinte condição:
 if(mouseX< windowWidth/2 && mouseY< windowHeight/2){ fill(20,150,70); }else { fill(0,100,80)}, esta que já funcionou como desejado.



 fonte: https://www.geeksforgeeks.org/javascript/create-an-object-that-follows-the-mouse-pointer-using-p5-js/
