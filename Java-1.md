package questao1;
import java.util.Scanner;

public class Questao1 {

    
    public static void main(String[] args) {
       int convidados;
       int cadeirasAdicionadas;
       
       Scanner entradaConvidados = new Scanner(System.in);
       System.out.println("Quantos convidados terá no evento? \n");
       convidados = entradaConvidados.nextInt();
       entradaConvidados.close();
       
       if (convidados >= 1 && convidados <= 150){
           System.out.println("Use o auditório Alfa \n");
       }
       if (convidados > 150 && convidados <= 220){
           cadeirasAdicionadas = convidados - 150;
           System.out.println("Use o auditório Alfa. \n");
           System.out.println("Inclua mais " + cadeirasAdicionadas);
       }
       if (convidados > 220 && convidados <= 350){
           System.out.println("Use o auditório Beta. \n");
       }
       if (convidados <= 0 || convidados > 350){
           System.out.println("Número inválido \n");
       }
    }
}