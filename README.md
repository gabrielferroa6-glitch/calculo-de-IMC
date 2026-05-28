import java.util.Scanner;

public class Main
{
	
  public static void main(String[] args) {
    
    Scanner sc = new Scanner(System.in);
    
    System.out.println("Digite o seu peso:");
    
    double peso = sc.nextDouble();
    
    System.out.println("Digite a sua altura");
    double altura = sc.nextDouble();
    
    double IMC = peso / (altura * altura);
    
    System.out.println("o seu IMC é: " + IMC);
    
    if ( IMC <= 18.5){
        System.out.println("você esta abaixo do peso ideal");
    }
    else if (18.5 < IMC && IMC <= 25){
        System.out.println("você esta com o peso ideal");
    }
    else if ( 25 < IMC && IMC <= 30){
        System.out.println("você esta com sobrepeso");
    }
    else if ( 30 < IMC && IMC <= 35){
        System.out.println("voce esta com obesidade grau I");
    }
    else if (35 < IMC && IMC <= 40){
        System.out.println("você esta com obesidade grau II");
    }
    else if ( 40 < IMC){
        System.out.println("você esta com obesidade grau III");
    }
	}
}
