import java.util.Scanner;

public class Main {
    public static void main (String [] args) {
        ConversorTemperatura conversao = new ConversorTemperatura();
        Scanner scanner = new Scanner(System.in);

        System.out.println("Digite uma temperatura em celsius: ");
        double celsius = scanner.nextDouble();

        System.out.println("Temperatura em Fahrenheit; " + conversao.celsiusParaFahreheint(celsius));
        System.out.println("Temperatura em Kelvin: " + conversao.celsiusParaKelvin(celsius));
        System.out.println("Temperatura em reaumur: " + conversao.celsiusParaReaumur(celsius));
        System.out.println("Temperatura em rankine; " + conversao.celsiusParaRankine(celsius));
    }
}

public class ConversorTemperatura {
        public double celsiusParaFahreheint(double celsius){
        return celsius * 1.8 + 32;
        }

        public double celsiusParaKelvin(double celsius){
                return celsius + 273.15;
        }

        public double celsiusParaReaumur(double celsius){
                return celsius * 0.8;
        }

        public double celsiusParaRankine(double celsius){
                return celsius *1.8- + 32 + 459.67;
        }
}
