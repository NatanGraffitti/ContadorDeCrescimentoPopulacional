import java.util.Scanner;

public class CrescimentoPopulacional {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int populacaoInicial; // Variável para armazenar o total inicial de espécies
        int t; // Variável para o tempo inicial em anos
        int numeroPeriodos = 0; // Variável para contar o número de períodos a serem calculados
        
        // Solicita ao usuário o total inicial de espécies
        System.out.println("Digite o total de espécies a ser contabilizada:");
        populacaoInicial = scanner.nextInt();
        
        // Solicita ao usuário o tempo inicial em anos
        System.out.println("Digite o tempo inicial em anos a ser calculado:");
        t = scanner.nextInt();
        
        // Loop while para permitir que o usuário faça múltiplos cálculos de períodos
        while (true) {
            // Solicita ao usuário o número de períodos a serem contados
            System.out.println("Digite o número de períodos a ser contado:");
            numeroPeriodos = scanner.nextInt();
            
            int populacaoAtual = populacaoInicial; // Variável para armazenar a população atual
            
            // Loop for para simular o crescimento populacional em cada período
            for (int periodos = 1; periodos <= numeroPeriodos; periodos++) {
                int novaPopulacao = (int) Math.round(populacaoAtual * periodos); // Calcula a nova população no período atual
                
                // Exibe a população no período atual
                System.out.println("População no período " + periodos + ": " + novaPopulacao);
                
                populacaoAtual = novaPopulacao; // Atualiza a população atual para o próximo período
            }
            
            // Pergunta ao usuário se deseja continuar calculando mais períodos
            System.out.println("Deseja calcular mais períodos? (Digite 0 para sair ou outro número para continuar)");
            int continuar = scanner.nextInt();
            
            if (continuar == 0) {
                break; // Sai do loop while se o usuário digitar 0
            }
        }
        
        scanner.close(); // Fecha o scanner para liberar recursos
    }
}
