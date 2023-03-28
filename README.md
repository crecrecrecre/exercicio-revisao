import java.util.Scanner;
public class exerciciorevisaoo {
     public static void main(String [] args){
         Scanner leitor = new Scanner(System.in);
         String [] nomes = new String[3];
         double [][] contas  = new double [4][4];
         int opcao;
         
         for(int cont = 0; cont < 3; cont++){
             System.out.println("Digite o seu nome: ");
             nomes[cont] = leitor.input.nextLine(); 
         }
         
         exibeString(nomes[]);
         System.out.println(" ");
     }
     
     public void exibeString(String [] nomes){
         for(int i = 0; i < 3; i++){
             System.out.println(nomes[i]);
         }
     }
     
     public void exibeDouble (double [] [] contas) {
          for(int i; i < 4; i++){
              for(int j; j < 4; j++){
                  System.out.printf(contas [i][j] + " | ");
              }
              //System.out.println(" ");
              System.out.printf("\n");
          }
     }
     
     public String verificaNum (int opcao, String [] nomes){
         if (opcao == 1){
             return nomes[0];
         }else if (opcao >= 2 && opcao <= 10){
             return nomes[1];
         }else if (opcao > 10){
             return nomes[2];
         }
         
         return "Opcao invalida";
     }
}
     
     
     
     
     
