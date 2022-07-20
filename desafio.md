# Desafio Algoritmo

Ana e Bruno participaram de um desafio de programação onde foram avaliados com uma pontuação de 1 a 100 em três categorias: clareza, originalidade e dificuldade.

A Avaliação de Ana no desafio é o trio:
``
a = (a[0], a[1], a[2])
`` 
e a avaliação de Bruno é o trio: ``
b = (b[0], b[1], b[2])
``

A tarefa é encontrar os pontos da comparação, comparando a[0] com b[0], a[1] com b[1], a[2] com b[2].

* Se a[i] > b[i] então Ana ganha um ponto
* Se a[i] < b[i] então Bruno ganha um ponto
* Se a[i] = b[i] então ninguém pontua

Pontos de comparação é a pontuação total que uma 
pessoa recebeu.

Dado que A e B determinam os seus respectivos pontos de comparação.

### Exemplo

a = [1,2,3]
b = [3,2,1]

* Para os elementos *0* Bruno ganhou um ponto pois b[0] > a[0].
* Para os elementos iguais a[1] e b[1] ninguém pontuou.
* Finalmente para os elementos *2*, a[2] > b[2] então Ana ganha um ponto.

O Array retornado é [1,1] com a pontuação da Ana na primeira posição e a do Bruno na segunda.

### Descrição da função

Desenvolva a função comparaTrios

A função comparaTrios recebe os seguintes parametros:

* int a[3]: Notas do desafio da Ana.
* int b[3]: Notas do desafio do Bruno.

### Retorno

A Função retorna int[2]: pontuação da Ana na primeira posição e do Bruno na segunda.

### Constraints

* 1 <= a[i] <= 100
* 1 <= b[i] <= 100



//      Resolução

int[] ana = new int[1, 2, 3];
int[] bruno = new int[3, 2, 1];

for(int i = 1; i < 3; i++ ) {
    
if ( ana[i] == bruno[i]) {
    return " Empate, ninguém pontua" 
    }
if ( ana[i] > bruno[i]) {
    return "Ana ganha um ponto"
    }
    else return "Bruno ganha um ponto"

    System.out.printf("ana" + ana + " \n"
                        "bruno" + bruno);
 }




