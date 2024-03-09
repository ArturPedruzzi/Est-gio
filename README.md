Questão 01)
 
  fun main() {
    val INDICE: Int = 13
    var SOMA: Int = 0
    var K: Int = 0 
    
    while(K < INDICE){
        K = K + 1
        SOMA = SOMA + K
     }
    println(SOMA)
   }

 A variável SOMA terá o valor 91



Questão 02)
 
   fun main() {
     val numero = 45 
     val verifica = verificaFibonacci(numero)
    
      if (verifica) {
         println("$numero pertence à sequência de Fibonacci.")
       } else {
         println("$numero não pertence à sequência de Fibonacci.")
       }
   } 

   fun verificaFibonacci(numero: Int): Boolean {
     var a = 0
     var b = 1
  
     for (i in 2..numero) {
      val c = a + b
        if (c == numero) {
        return true
       }
      a = b
      b = c
        if (c > numero) {
        break 
       }
   }
    return false
}



Questão 03)

a) 1, 3, 5, 7, _9_
 A sequência soma 2 a cada número que é passado.


 b) 2, 4, 8, 16, 32, 64, _128_
 A sequência pega o dobro do número anterior.


 c) 0, 1, 4, 9, 16, 25, 36, _49_
 A sequência é dos números de 1 a 7 elevado a 2.


 d) 4, 16, 36, 64, _100_
 A sequência é dos números pares de 1 a 10 elevado a 2. 


 e) 1, 1, 2, 3, 5, 8, _13_
 É a sequência de Fibonacci, ou seja, cada número é a soma dos dois anteriores.


 f) 2, 10, 12, 16, 17, 18, 19, __
 Não pude compreender a lógica apresentada.



Questão 04)

  Infelizmente, não consegui interpretar corretamente a pergunta. Algumas frases me pareceram confusas. Por exemplo:
 
  "Você está em uma sala com três interruptores, cada um conectado a uma lâmpada em uma sala diferente." - Até ai tudo bem, deu a entender
  que estou em uma sala na qual possui os interruptores e há outra sala que possui as lâmpadas. 

  "Você não pode ver as lâmpadas da sala em que está," - Agora começa a ficar estranho, pois essa frase me deixou a entender que na mesma sala
  dos interruptores(a sala que eu estou) possui uma ou mais lâmpadas e eu não posso vê-las.
   
  "Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas" - Aqui deixa explícito que as outras duas lâmpadas estão em salas diferentes.
  Pois não seria possível eu dar uma ida em uma sala que já estou, ao falar "uma das salas das lâmpadas" ficou claro para mim que as duas lâmpadas que faltam estão em salas
  diferentes. Além do que, está explícito que posso visitar apenas uma sala duas vezes. 

  Interpretando a pergunta da forma na qual interpretei, ficou impossível concluir esse exercício de lógica. Peço perdão.



Questão 05) 

  fun main() {
      val stringExemplo = "Exemplo Estágio" 
      val inverterString = InverterString(stringExemplo)
      println("String original: $stringExemplo")
      println("String invertida: $inverterString")
  }

  fun InverterString(stringExmp : String): String {
      val charArray = stringExmp.toCharArray()
      val sizeString = charArray.size 
      val inverterArrayChar = CharArray(sizeString)
    
    
      for (i in 0 until sizeString) {
          inverterArrayChar[i] = charArray[sizeString - 1 - i]
      }
    
      return String(inverterArrayChar)
  }
