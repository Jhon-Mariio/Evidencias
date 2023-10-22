<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Su documentación aquí -->


Actividad 1
abstract class Vehiculo {
    
    abstract void acelerar();
    abstract void frenar();
    abstract void girar();
}

class Coche extends Vehiculo {

    @Override
    void acelerar() {
        System.out.println("El coche acelera");
    }

    @Override
    void frenar() {
        System.out.println("El coche frena");
    }

    @Override
    void girar() {
        System.out.println("El coche gira");
    }

 
}

class Bicicleta extends Vehiculo {

    @Override
    void acelerar() {
        System.out.println("La bicicleta acelera");
    }

    @Override
    void frenar() {
        System.out.println("La bicicleta frena");
    }

    @Override
    void girar() {
        System.out.println("La bicicleta gira");
    }
    
}

class Moto extends Vehiculo {

    @Override
    void acelerar() {
        System.out.println("La moto acelera"); 
    }

    @Override
    void frenar() {
        System.out.println("La moto frena");
    }

    @Override
    void girar() {
        System.out.println("La moto gira");
    }
    
}
Main
public static void main(String[] args) {
     ArrayList<Vehiculo> vehiculos = new ArrayList<>();
        vehiculos.add(new Coche());
        vehiculos.add(new Bicicleta());
        vehiculos.add(new Moto());

        for (Vehiculo vehiculo : vehiculos) {    
            vehiculo.acelerar();
            vehiculo.frenar();
            vehiculo.girar();
            
        }
    }
Submódulo: Lógica de Programación Periodo: 2023-2
Estudiante: Jhon Mario Castrillón Gutierrez 


