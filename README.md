# Sueldo-trabajador-
import java.util.Scanner;

public class SueldoTrabajador {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Horas trabajadas: ");
        int horas = sc.nextInt();
        System.out.print("Valor por hora: ");
        double valorHora = sc.nextDouble();
        double sueldo = (horas > 40) ? (40 * valorHora + (horas - 40) * valorHora * 2) : (horas * valorHora);
        System.out.println("Sueldo final: " + sueldo * 0.92); // 8% de descuento
        sc.close();
    }
}
