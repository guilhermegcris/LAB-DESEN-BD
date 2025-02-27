# LAB-DESEN-BD
ATIVIDADES DE LABORATÓRIO DE DESENVOLVIMENTO DE BANCO DE DADOS


Exercício 1:

import java.util.Scanner;

public class tarefa_1{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Para descobrir ha quantos dias voce nasceu, adicione a quantidade anos, meses e dias na seguinte sequencia:"); 
        
        System.out.print("Digite quantos anos voce tem:"); 
        int ano = scanner.nextInt();
        
        System.out.print("Digite quantos meses voce tem:"); 
        int meses = scanner.nextInt();
        
        System.out.print("Digite quantos dias voce tem:"); 
        int dias = scanner.nextInt();
        
        int tano = ano * 365;
        int tmeses = meses * 30;
        
        int fin = tano + tmeses + dias;
        
        System.out.println("Voce tem " + fin + " dias de vida");
        
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 1

Entradas de teste
Anos = 10
Meses = 3
Dias = 15

Digite quantos anos voce tem = 10
Digite quantos meses voce tem = 3
Digite quantos dias voce tem = 15

tano = ano * 365;	10 * 365 = 3650	
tmeses = meses * 30 = 90
fin = tano + tmeses + dias;	3650 + 90 + 15 = 7495	
fin = 3755

Saída 
"Voce tem 3755 dias de vida"

-----------------------------------------------------------------------------

Exercício 2:

import java.util.Scanner;

public class tarefa1_2 {
     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("Digite o numero de eleitores, a quantidade de votos nulos, brancos e válidos na seguinte sequencia ");
        
        System.out.print("Digite votos totais:");
        float votos = scanner.nextFloat();
        
        System.out.print("Digite votos nulos:");
        float nulos = scanner.nextFloat();
        
        System.out.print("Digite votos brancos:");
        float brancos = scanner.nextFloat();
        
        System.out.print("Digite votos validos:");
        float validos = scanner.nextFloat();       
        
        float vnulos = (nulos/votos)*100;
        float vbrancos = (brancos/votos)*100;
        float vvalidos = (validos/votos)*100;

	float soma = nulos + brancos + validos;

	if (votos != soma) {

	System.out.print("A quantidade de votos nao eh compativel com a quantidade de eleitores");

	} else {        

            System.out.printf("A quantidade de votos nulos é: %.2f%%, brancos é: %.2f%%, válidos é: %.2f%%\n", vnulos, vbrancos, vvalidos);

		}
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 2

Entradas de teste
Total de eleitores: 1000
Votos nulos: 100
Votos brancos: 200
Votos válidos: 700
Execução
Variável	 Cálculo	           Resultado
soma	     100 + 200 + 700	   1000 
vnulos	   (100 / 1000) * 100	 10.00%
vbrancos	 (200 / 1000) * 100	 20.00%
vvalidos	 (700 / 1000) * 100	 70.00%

--------------------------------------------------------------------------
Exercício 3:

import java.util.Scanner;

public class tarefa_3{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Digite salario mensal atual:");
        float sal = scanner.nextFloat();
        
        System.out.print("Digite o percentual de reajuste:");
        float rea = scanner.nextFloat();
        
        float vrea = (rea/100)*sal;

        float tot = sal + vrea;
        
        
        System.out.println("O salario reajustado foi para " + tot + " reais");
        
     }
}
-------------------------------------------------------------------------------------
Teste de Mesa 3

Entrada de teste
Salário mensal: 1000.00
Percentual de reajuste: 10.00
Cálculos
vrea = (10 / 100) * 1000 = 100
tot = 1000 + 100 = 1100

-----------------------------------------------------------------------------------
Exercício 4:

import java.util.Scanner;

public class tarefa_4{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);
        
        System.out.print("Digite o custo do carro:");
        float car = scanner.nextFloat();
        
        float dist = 28;
        
        float imp = 45;
        
        float vfinal = car + (dist/100)*car + (imp/100)*car;
        
        System.out.println("O custo final do carro para o consumidor é" + vfinal);
        
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 4

Entrada de teste
Custo de fábrica do carro: 50.000,00
Cálculo
Distribuidor: (28 / 100) * 50000 = 14000
Impostos: (45 / 100) * 50000 = 22500
Preço final: 50000 + 14000 + 22500 = 86500

----------------------------------------------------------------------------------------
Exercício 5:

import java.util.Scanner;

public class tarefa_5 {

    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite o salario fixo: ");
        float sf = scanner.nextFloat();
        
        System.out.print("Digite a quantidade de carros vendidos: ");
        float carv = scanner.nextFloat();
        
        System.out.print("Digite o valor recebido por carro vendido: ");
        float vcv = scanner.nextFloat();
        
        float tv = carv * vcv; 
        float comissao = tv * 0.05f; 
        float tot = sf + comissao; 
        
        System.out.printf("O valor total de vendas: %.2f reais\n", tv);
        System.out.printf("O salario final: %.2f reais\n", tot);
        
    }
}
-------------------------------------------------------------------------------------
Teste de Mesa 5

Entrada de Teste
Salário fixo: 1000
Carros vendidos: 5
Valor por carro vendido: 10000
Cálculo
Valor total de vendas: 5 * 10000 = 50000
Comissão: 50000 * 0.05 = 2500
Salário final: 1000 + 2500 = 3500

-----------------------------------------------------------------------------------------
Exercício 6:

import java.util.Scanner;

public class tarefa_6 {

     public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite a temperatura em Fahrenheit: ");
        float fahrenheit = scanner.nextFloat();
        
        float celsius = (fahrenheit - 32) * 5 / 9;
        
        System.out.printf("A temperatura em Celsius é " + celsius);
        
     }
}
-------------------------------------------------------------------------------------
Teste de Mesa 6

Entrada de Teste
Temperatura em Fahrenheit: 212

Cálculo

Celsius = (212 − 32) × 5/9
Celsius = (180*5)/9 = 100

-----------------------------------------------------------------------------------------
Exercício 7:

import java.util.Scanner;

public class tarefa_7{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite um numero:");
        int num = scanner.nextInt();
        
        if (num>10) {
            
        System.out.println("É maior que 10");    
        
        } else{
        System.out.println("Não é maior que 10");
        }
     }
}
-------------------------------------------------------------------------------------
Teste de Mesa 7

Entrada 1
Digite um número: 15

Saída 1
É maior que 10

Entrada 2
Digite um número: 7

Saída 2
Não é maior que 10

-------------------------------------------------------------------------------------
Exercício 8:

import java.util.Scanner;

public class tarefa_8{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite um numero:");
        float num = scanner.nextFloat();
        
        if (num >= 0) {
        System.out.println("O numero eh positivo");
        } else{
        System.out.println("O numero eh negativo");     
        }
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 8

Entrada 1
Digite um número: 1

Saída 1
O numero é positivo

Entrada 2
Digite um número: -1

Saída 2
O numero é negativo

-----------------------------------------------------------------------------------------
Exercício 9:

import java.util.Scanner;

public class tarefa_9{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite a quantidade de maca:");
        int maca = scanner.nextInt();
        
        float preco;
        
        if (maca >= 12) {
        preco=1f;   
        } else{
        preco=1.30f;     
        }
        float val = maca*preco;
        System.out.print("O preco de "+maca+" macas sera R$"+val);

     }
}


-------------------------------------------------------------------------------------
Teste de Mesa 9


ENTRADA
Quantidade de maçãs compradas:

CONDIÇÃO:
Para (Maçãs >= 12)

Se verdadeiro

Maçãs * 1.00 = preço

Se não

Maçãs * 1.30 = preço

SAIDA
"O preço pago pelas maçãs é igual a "+preço+

EXEMPLO

QUANTIDADE DE MAÇAS = 10
CONDIÇÃO: FALSA

10 * 1.3 = PREÇO

PREÇO = 13


-------------------------------------------------------------------------------------
Exercício 10:

import java.util.Scanner;

public class tarefa_10{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite a primeira nota:");
        float n1 = scanner.nextFloat();
        
        System.out.print("Digite a segunda nota:");
        float n2 = scanner.nextFloat();
        
        float tot = (n1 + n2) / 2;
        
        if (tot >= 6) {
        System.out.println("Aluno aprovado!");
        } else{
        System.out.println("Aluno reprovado!");     
        }
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 10

Entrada 1
Nota 1: 7.0
Nota 2: 6.0

Cálculo
(7.0+6.0)/2=6.5

Saida 1
Aluno aprovado!

Entrada 2
Nota 1: 5.0
Nota 2: 6.0

Cálculo
(5.0+6.0)/2=5.5

Saida 2
Aluno reprovado!


-------------------------------------------------------------------------------------
Exercício 11:
import java.util.Scanner;

public class tarefa_11 {

     public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite o ano atual: ");
        int ano = scanner.nextInt();
        
        System.out.print("Digite o ano de nascimento: ");
        int nas = scanner.nextInt();        
        
        int idade = ano - nas; 

        if (idade >= 16) {
            System.out.println("Você poderá votar");
        } else {
            System.out.println("Você não poderá votar");
        }
     }
}
-------------------------------------------------------------------------------------
Teste de Mesa 11

Entrada 1
Digite o ano atual: 2025
Digite o ano de nascimento: 2009

Saida 1 
Você poderá votar

Entrada 2
Digite o ano atual: 2025
Digite o ano de nascimento: 2011

Saida 2 
Você não poderá votar


-------------------------------------------------------------------------------------
Exercício 12:
import java.util.Scanner;

public class tarefa_12{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite um numero:");
        int n1 = scanner.nextInt();
        
        System.out.print("Digite outro numero:");
        int n2 = scanner.nextInt();        
        
        if (n1 == n2){
         System.out.println("Os numeros são iguais");   
        } else{
        if (n1 > n2) {
        System.out.println(n1 + " é maior");
        } else{
        System.out.println(n2 + " é maior");     
        }
     }
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 12

Entrada 1
Digite o primeiro número: 8
Digite o segundo número: 3

Saída 1
8 é maior

Entrada 2
Digite o primeiro número: 8
Digite o segundo número: 10

Saída 2
10 é maior

-------------------------------------------------------------------------------------
Exercício 13:

import java.util.Scanner;

public class tarefa_13{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite um numero:");
        int n1 = scanner.nextInt();
        
        System.out.print("Digite um outro numero:");
        int n2 = scanner.nextInt();        
        
        if (n1 == n2) {
            System.out.println("Os números são iguais.");
        } else if (n1 > n2) {
            System.out.println("Ordem decrescente: " + n1 + " - " + n2);
        } else {
            System.out.println("Ordem decrescente: " + n2 + " - " + n1);
        }
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 13

Entrada 1
Digite o primeiro número: 10
Digite o segundo número: 5

Saida 1
Ordem decrescente: 10 - 5

Entrada 2
Digite o primeiro número: 1
Digite o segundo número: 7

Saida 2
Ordem decrescente: 7 - 1
-------------------------------------------------------------------------------------
Exercício 14:
import java.util.Scanner;

public class tarefa_14{

     public static void main(String []args){
        
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite a hora que comecou o jogo:");
        int h1 = scanner.nextInt();
        
        System.out.print("Digite a hora que terminou o jogo:");
        int h2 = scanner.nextInt();  
        
        int temp;
        
        if (h2 >= h1){
         temp = h2 - h1; 
        }
        else{
        temp = (24 - h1) + h2;
        }
        System.out.print(temp);
     }
}

-------------------------------------------------------------------------------------
Teste de Mesa 14

Entrada
Digite a hora que começou o jogo: 14
Digite a hora que terminou o jogo: 18

Saida
O jogo durou 4 horas

-------------------------------------------------------------------------------------
Exercício 15:

import java.util.Scanner;

public class tarefa_15 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite o numero de horas trabalhadas no mes: ");
        int horasTrabalhadas = scanner.nextInt();

        System.out.print("Digite o valor do salario por hora: ");
        double salarioHora = scanner.nextDouble();

        int horasSemanais = 40;
        int semanasMes = 4;
        int horasNormaisMensais = horasSemanais * semanasMes;
        double salarioTotal;

        if (horasTrabalhadas > horasNormaisMensais) {
            int horasExtras = horasTrabalhadas - horasNormaisMensais;
            double valorHoraExtra = salarioHora * 1.5;
            salarioTotal = (horasNormaisMensais * salarioHora) + (horasExtras * valorHoraExtra);
        } else {
            salarioTotal = horasTrabalhadas * salarioHora;
        }

        System.out.printf("O salario total do funcionario e: R$ %.2f\n", salarioTotal);
    }
}


-------------------------------------------------------------------------------------
Teste de Mesa 15

Entrada 1 (Sem horas extras)
Digite o número de horas trabalhadas no mês: 160
Digite o valor do salário por hora: 20

Saida 1
O salário total do funcionário é: R$ 3200.00

Entrada 2 (Com horas extras)
Digite o número de horas trabalhadas no mês: 180
Digite o valor do salário por hora: 20

Saida 2
Horas extras trabalhadas: 20
O salário total do funcionário é: R$ 3500.00

-------------------------------------------------------------------------------------
Exercício 16:
public class tarefa_16 {
    public static void main(String[] args) {

        double jan = 15000;
        double fev = 23000;
        double mar = 17000;

        double totalTri = jan + fev + mar;
        double mediaMensal = totalTri / 3;

        System.out.printf("O gasto total no trimestre foi de R$ %.2f\n", totalTri);
        System.out.printf("A média mensal de gastos foi de R$ %.2f\n", mediaMensal);
    }
}


-------------------------------------------------------------------------------------
Teste de Mesa 16

Saida
O gasto total no trimestre foi de R$ 55000.00
A média mensal de gastos foi de R$ 18333.33

-------------------------------------------------------------------------------------
Exercício 17:

import java.util.Scanner;

public class tarefa_17 {

    public static void main(String[] args) {
    
        Scanner scanner = new Scanner(System.in);

        System.out.print("Digite a nota P1: ");
        double P1 = scanner.nextDouble();

        System.out.print("Digite a nota E1: ");
        double E1 = scanner.nextDouble();

        System.out.print("Digite a nota E2: ");
        double E2 = scanner.nextDouble();

        System.out.print("Digite a nota API: ");
        double API = scanner.nextDouble();

        System.out.print("Digite a nota X: ");
        double X = scanner.nextDouble();

        System.out.print("Digite a nota SUB (ou rec): ");
        double SUB = scanner.nextDouble();

        // Calculando o primeiro termo
        double primeiroTermo = (P1 * 0.6) + (((E1 + E2) / 2) * 0.4);
        primeiroTermo = primeiroTermo * 0.5;

        // Calculando segundo termo de forma segura
        double segundoTermo = 0;
        if (primeiroTermo > 5.9) {
            segundoTermo = (primeiroTermo - 5.9) / (primeiroTermo - 5.9);
        }

        // Cálculo da média final
        double resultado = primeiroTermo + (segundoTermo * (API * 0.5)) + X + (SUB * 0.3);

        // Exibindo a média formatada com 2 casas decimais
        System.out.printf("A média de LP1 do aluno é: %.2f%n", resultado);
    }
}

    

-------------------------------------------------------------------------------------
Teste de Mesa 17

Entrada

Digite a nota P1: 7.0
Digite a nota E1: 6.5
Digite a nota E2: 7.2
Digite a nota API: 8.0
Digite a nota X: 2.0
Digite a nota SUB (ou rec): 6.5

Saida
A média de LP1 do aluno é: 9.12
