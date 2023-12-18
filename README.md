import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        double nota1, nota2, media1, media2, mediageral, mediafinal, notafinal;
        Scanner dado;
        dado = new Scanner(System.in);

        System.out.println("Digite sua nota do primeiro GQ: ");
        nota1 = dado.nextDouble();
        
        System.out.println("Digite sua nota do segundo GQ: ");
        nota2 = dado.nextDouble();

        media1 = nota1 * 0.4;

        media2 = nota2 * 0.6;

        mediageral = (media1 + media2);

        if (mediageral >=7){
            System.out.println("Parabéns você for aprovado com média: "+mediageral);

        }
        else {
            System.out.println("Você precisa realizar a final.");

            System.out.println("Digite sua nota da final: ");
            notafinal = dado.nextDouble();

            mediafinal = (mediageral + notafinal)/2;

            if (mediafinal>5){
                System.out.println("Parabéns você for aprovado com média: "+mediafinal);
            }
            else {
                System.out.println("Infelizmente sua média foi inferior a média necessária para aprovação: "+mediafinal);
            }
           
        }
        
    }
}
