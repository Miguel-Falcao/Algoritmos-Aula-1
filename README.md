# Algoritmos-Aula-1
Aula mesmo, não sumário

  PROGRAMAÇÃO ESTRUTURADA
  
  #include(visual1);
 
-Filosofia da programação estruturada: dividir para conquistar (técnica de refinamentos sucessivos) 
  O problema inicial é subdividido em subproblemas que por sua vez são divididos em problemas menores, etc. cada subdivisão é mais detalhada do que a anterior.

Problema: Lampada Queimada 
  1 - Remova a lampada 
  2 - Coloque a nova lampada
 
Subdivisão do problema inicial:tskill

  / 1.1 - Posicione a escada debaixo da lampada
1 - 1.2 - Suba na escada até alcançar a lampada
  \ 1.3 - Gire a lampada no sentido anti-horário até que a mesma se solte
  
  / 2.1 - Escolha a nova lampada
2 - 2.2 - Posiciona e nova lampada no soquete
  \ 2.3 - Gire no sentido horário até que a lampada fique firme
  \ 2.4 - Desça da escada
tskill

  ALGORITMOS

-No dicionário: "Qualquer método utilizado para a solução de um determinado problema"
-Na ciência da computação: "Uma sequencia ordenada e sem ambiguidade de passos que levam à solução de um problema"

EX: Usar o orelhão tskill
  1 - Retirar o fone do gancho
  2 - Colocar o cartão telefonico
  3 - Esperar o ruído se discar
  4 - Com o ruído de discar, disque o número desejado
  5 - Se sinal de oucupado faça 
   5.1 - Colocar o fone no gancho e voltar ao passo 1
  6 - Se sinal de chamada faça
   6.1 - Esperar atender o telefone
   6.2 - Conversar
   6.3 - colocar o fone no gancho
   6.4 - Retirar o cartão
 tskill  
   
 PROPRIEDADES DE UM ALGORITMO

-Cada *operação* deve ser *bem definida*
- *Não ambíguo*
- *Eficaz*: Consegue resolver o problema em qualquer situação
- O algoritmo deve terminar após um *número finito de passos*
- Cada passo do algoritmo deve ser executado em um *tempo finito*


~/sudo start visual-1-example
  #include<stdio.h>
main(){
	
	int n, nn, nnn;
	float m;
	
	printf("\t\tPrimeiro método");
	printf("\n");
	printf("Digite n1: ");
	scanf("%d", &n);
	
	printf("Digite n2: ");
	scanf("%d", &nn);
	
	nnn = n + nn;
	m = nnn / 2;
	
	printf("A media eh %.2f", m);
	
	int t = clock();
	while(clock() - t < 1000);
	printf("\n");
	printf("\t\tSegundo metodo");
	printf("\n");
	int n1, n2;
	float m2;
	
    printf("Digite n1: ");
	scanf("%d", &n1);
		
	printf("Digite n2: ");
	scanf("%d", &n2);
	
	m2 = (n1 + n2)/2;
	
	printf("A media eh %.2f", m2);
}

  CONSTRUÇÃO DE ALGORITMOS

Tipos de dados: Define os valores que um dado pode assumir e as operações que podem ser efetuadas sobre o dado.

  TIPOS PRIMITIVOS DE DADOS
  
 1 - Números
 	- Inteiros: valores inteiros, positivos ou negativos.
		ex: 345, -10, 1321
	- Reais: Valores fracionários, positivos ou negativos.
		ex: -20.3, 38.56
 #include(visual2)
 O operador % não pode ser utilizado com reais.
 
 Ex: Operadores / e %
 13/5 (int/int) = 2 (int)
 13/5.0 (int/double) = 2.6 (double)
 13 % 5 = 3  
 
Como obter a parte inteira da divisão (resultado truncado)?
#include<stdio.h>

main(){
	
	// quociente = (dividendo - (dividendo % divisor) / divisor)
			//			13           3                   5
	// ex = 13/5
	/* dividendo = 13  d1
		divisor = 5    d2
		quociente = 2  q
		resto = 3      r
	*/
	
	
	float d1, d2, q, r;
	
	printf("d1");
	scanf("%f", &d1);
	
	printf("\n");
	printf("d2");
	scanf("%f", &d2);
	
	q = (d1 - (d1 % d2) / d2);
	printf("%f", q);
	
	//fazer depois: printar nome dos alunos que tiveram a nota maior q a media da turma 
}

TIPOS DE DADOS NUMÉRICOS EM C:

Tipo				|	Tamanho		|	Faixas de valores

int(números inteiros)   	|	4 Bytes         |	-32768 a 32767
Short(curto)			|	2 Bytes		|	-32768 a 32767
Unsigned(sem sinal)		|	2 Bytes		|	-0 a 65.535
Long(longo)			|	4 Bytes		|	-2,147,483,648 a 2,147,483,647
Float(flutuant precisao simples)|	4 Bytes		|	3.4e-38 a 3.4e+38
double				|    	8 Bytes  	|	1.7 E-308 a 1.7E+308


2 - CARACTERES (1: line100)
  - Representam as letras de (A - Z), os dígitos numéricos (0 - 9) e sinais especiais (Espaço em branco; sinais de pontuação)
  - Aparecem entre aspas duplas
  	ex: "Maria", "Casa 8"

NA LINGUAGEM C:
	Char = 1 byte
	
	ex: char nome[6];
	T|E|S|T|E|\0|; O '\0' representa o fim da cadeia de caracterses











   
 
 
 
