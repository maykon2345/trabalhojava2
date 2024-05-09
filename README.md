Maykon ANTONIO Willemann de macedo



If, else if, e else
Switch case
For loop
While loop


Em JavaScript , um valor verdadeiro é um valor considerado truequando encontrado em um contexto booleano . Todos os valores são verdadeiros, a menos que sejam definidos como falsos . Ou seja, todos os valores são verdadeirosfalse , exceto , 0, -0, 0n, "", null, , undefined, NaNe document.all.

JavaScript usa coerção de tipo em contextos booleanos.

Exemplos de valores verdadeiros em JavaScript (que serão forçados trueem contextos booleanos e, portanto, executarão o ifbloco):



Very often when you write code, you want to perform different actions for different decisions.

You can use conditional statements in your code to do this.

In JavaScript we have the following conditional statements:

Use if to specify a block of code to be executed, if a specified condition is true
Use else to specify a block of code to be executed, if the same condition is false
Use else if to specify a new condition to test, if the first condition is false
Use switch to specify many alternative blocks of code to be executed
Statement that is executed if condition is truthy. Can be any statement, including further nested if statements. To execute multiple statements, use a block statement ({ /* ... */ }) to group those statements. To execute no statements, use an empty statement.

statement2
Statement that is executed if condition is falsy and the else clause exists. Can be any statement, including block statements and further nested if statements.


  01 exeplo 
if (x > 50) {
  /* do something */
} else if (x > 5) {
  /* do something */
} else {
  /* do something */
}]

function checkValue(a, b) {
  if (a === 1) {
    if (b === 2) {
      console.log("a is 1 and b is 2");
    }
  } else {
    console.log("a is not 1");
  }
}


Se a condição for correspondida, o programa executa as instruções asssociadas. Se múltiplos casos corresponderem o valor, o primeiro caso que corresponder é selecionado, mesmo se os casos não forem iguais entre si.

02 Exemplos
var foo = 0;
switch (foo) {
  case -1:
    console.log("1 negativo");
    break;
  case 0: // foo é 0 então aqui o critério foi correspondido, então esse bloco vai rodar
    console.log(0);
  // NOTA: o break esquecido deveria estar aqui
  case 1: // nenhuma instrução break em 'case 0:' então essa instrução vai rodar também
    console.log(1);
    break; // o programa encontra esse break então não vai continuar para o 'case 2:'
  case 2:
    console.log(2);
    break;
  default:
    console.log("default");


    Uma expressão (incluindo expressões de atribuição) ou declarações variáveis. Geralmente usada para iniciar o contador de variáveis. Esta expressão pode, opcionalmente, declarar novas variáveis com a palavra chave var. Essas variáveis não são locais no loop, isto é, elas estão no mesmo escopo que o loop for está. Variáveis declaradas com let são locais para a declaração.

O resultado desta expressão é descartado.

condição
Uma expressão para ser avaliada antes de cada iteração do loop. Se esta expressão for avaliada para true, declaração será executado. Este teste da condição é opcional. Se omitido, a condição sempre será avaliada como verdadeira. Se a expressão for avaliada como falsa, a execução irá para a primeira expressão após a construção loop for.

expressão final
Uma expressão que será validada no final de cada iteração de loop. Isso ocorre antes da próxima avaliação da condição. Geralmente usado para atualizar ou incrementar a variável do contador.

declaração
Uma declaração que é executada enquanto a condição for verdadeira. Para executar múltiplas condições dentro do loop, use uma instrução de bloco ({...}) para agrupar essas condições. Para não executar declarações dentro do loop, use uma instrução vazia (;)

ma expressão avaliada antes de cada passagem através do laço. Se essa condição for avaliada como verdadeira, a rotina é executada. Quando a condição for avaliada como falsa, a execução continua na declaração depois do laço while.

rotina
Uma declaração que é executada enquanto a condição é avaliada como verdadeira. Para executar multiplas declarações dentro de um laço, use uma declaração em bloco ({ ... }) para agrupar essas declarações.
