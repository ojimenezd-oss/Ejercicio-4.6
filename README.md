# Ejercicio-4.6
package Profesores;

public class Profesor {

    protected void imprimir() {
        System.out.println("Es un profesor.");
    }
}
package Profesores;

public class ProfesorTitular extends Profesor {

    int años = 0;

    @Override
    protected void imprimir() {
        System.out.println("Es un profesor titular.");
    }

    protected void imprimirAños() {
        System.out.println("Años = " + años);
    }
}
package Profesores;

public class Prueba3 {

    public static void main(String[] args) {

        Profesor profesor1 = new ProfesorTitular();

        ((ProfesorTitular) profesor1).imprimirAños();
    }
}
