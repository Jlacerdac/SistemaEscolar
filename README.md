// 1 atividade
import java.util.Scanner;

public class SistemaEscolar {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double[] notas = new double[8];

        System.out.println("--- Sistema de Cálculo de Médias Escolares ---");

        // Recebe as 8 notas anuais do aluno
        for (int i = 0; i < 8; i++) {
            System.out.printf("Digite a nota do %dº bimestre: ", (i + 1));
            notas[i] = scanner.nextDouble();
        }

        // Calcula as médias bimestrais (já estão nas variáveis individuais)
        double nota1Bimestre = notas[0];
        double nota2Bimestre = notas[1];
        double nota3Bimestre = notas[2];
        double nota4Bimestre = notas[3];
        double nota5Bimestre = notas[4];
        double nota6Bimestre = notas[5];
        double nota7Bimestre = notas[6];
        double nota8Bimestre = notas[7];

        // Calcula as médias semestrais
        double media1Semestre = (nota1Bimestre + nota2Bimestre + nota3Bimestre + nota4Bimestre) / 4.0;
        double media2Semestre = (nota5Bimestre + nota6Bimestre + nota7Bimestre + nota8Bimestre) / 4.0;

        // Calcula a média final
        double mediaFinal = (media1Semestre + media2Semestre) / 2.0;

        // Apresenta os resultados de forma clara
        System.out.println("\n--- Boletim de Resultados ---");

        // Utiliza %.1f para formatar os doubles com uma casa decimal, como no exemplo.
        System.out.printf("1º Bimestre: %.1f\n", nota1Bimestre);
        System.out.printf("2º Bimestre: %.1f\n", nota2Bimestre);
        System.out.printf("3º Bimestre: %.1f\n", nota3Bimestre);
        System.out.printf("4º Bimestre: %.1f\n", nota4Bimestre);
        System.out.printf("   1º Semestre: %.1f\n", media1Semestre);
        System.out.println("---------------------------------");
        System.out.printf("5º Bimestre: %.1f\n", nota5Bimestre);
        System.out.printf("6º Bimestre: %.1f\n", nota6Bimestre);
        System.out.printf("7º Bimestre: %.1f\n", nota7Bimestre);
        System.out.printf("8º Bimestre: %.1f\n", nota8Bimestre);
        System.out.printf("   2º Semestre: %.1f\n", media2Semestre);
        System.out.println("---------------------------------");
        System.out.printf("Média Final: %.1f\n", mediaFinal);

        scanner.close();
    }
}
// 2 atividade
import java.util.Scanner; // Importa a classe Scanner para permitir a entrada de dados pelo usuário

public class ConversorTemperatura {

    public static void main(String[] args) {
        // Cria um objeto Scanner para ler a entrada do usuário via console
        Scanner scanner = new Scanner(System.in);

        // Exibe uma mensagem para o usuário informando sobre a atividade
        System.out.println("--- Atividade 02: Conversor de Temperatura ---");
        System.out.print("Digite a temperatura em graus Celsius (°C): ");

        // Lê o valor em Celsius digitado pelo usuário e armazena em uma variável double
        double celsius = scanner.nextDouble();

        // Realiza o cálculo para converter Celsius para Fahrenheit
        // Fórmula: Fahrenheit = (Celsius × 9/5) + 32
        double fahrenheit = (celsius * 9/5) + 32;

        // Realiza o cálculo para converter Celsius para Kelvin
        // Fórmula: Kelvin = Celsius + 273.15
        double kelvin = celsius + 273.15;

        // Exibe os resultados na tela, formatados de forma clara e informativa
        System.out.println("\n--- Resultados da Conversão ---");
        System.out.printf("Temperatura em Celsius: %.1f °C\n", celsius);
        System.out.printf("Temperatura em Fahrenheit: %.1f °F\n", fahrenheit);
        System.out.printf("Temperatura em Kelvin: %.2f K\n", kelvin);

        // Fecha o objeto Scanner para liberar recursos
        scanner.close();
    }
}


