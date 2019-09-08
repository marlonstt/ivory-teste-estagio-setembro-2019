# ivory-teste-estagio-setembro-2019
 
 O objetivo do programa é calcular o fatorial de um determinado número(ex: 5! = 5 * 4 * 3 * 2 * 1).
 
 O programa em execução declara uma variável de inteiros "numero" que recebe o valor 5, declara "resultado" do tipo int e depois diz que "resultado" é igual ao valor retornado pelo método "Calcular(numero)" na "Main".
O método "Calcular(int numero)" é chamado diretamente por ser do tipo "static"(não pode ser instânciado) e pertencer ao mesmo 
corpo de classe de onde foi chamado e então "Calcular(int numero)" recebe "numero" por valor como parametros e é executado.
Em execução "Calcular(int numero)" em seu corpo declara uma variável local "int resultado" para servir de retorno ao método,
logo após é criado uma estrutura de controle "if" e também "else" que diz que se "numero" for menor ou igual a 1, o método deve
retornar 1, senao, a variável local "resultado" recebe "numero" x "Calcular(--numero), percebe-se que é subtraido de "numero" que 
era igual a 5 o valor 1 nos parametros do método e então o método "Calcular()" entra novamente em execução e como em "loop", vai 
fatorando o valor de "numero" dentro do método até que "numero" seja menor ou igual a 1 e entao entra na estrutura de controle "if" 
que por sua vez retorna o valor 1 para "Calcular(--numero)" e então voltando a primeira chamada do método "Calcular()" na "Main", 
dentro do else, é finalizada a atribuição a "resultado" e é retornado o valor atual de "resultado" pelo método.
 Na "Main" "resultado" recebeu o valor calculado pelo método e em seguida é impreso na tela.
 Feito isso, o programa aguarda o toque de alguma tecla do teclado para terminar a execução.
 
 O resultado exibido na tela é o numero 120 que é o fatorial de 5(ex: 5! = 5 * 4 * 3 * 2 * 1).
 
  Ao meu ver o codigo possui erros nos tipos de dados das variaveis declaradas e também no tipo de dados do método"int Calcular()", pois, 
 se fosse calcular o fatorial de um numero muito grande, por exemplo 100!, a variável "int resultado" não suportaria armazenar um valor 
 tão grande e a impressão sairia errada. Por tanto, seria legal mudar para double o método "Calcular()" e sua variável local "resultado" e 
 na "Main" também mudaria "numero" para var (para seguir a Padronização codificação) e "resultado" para double.
