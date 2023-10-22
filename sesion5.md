<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


<!-- Su documentación aquí -->

public class Producto { private String nombre; private double precio; private int cantidad;

public Producto() {
    this.nombre = "desconocido";
    this.precio = 0.0;
    this.cantidad = 0;   
}

public Producto(String nombre, double precio) {
    this.nombre = nombre;
    this.precio = precio;
    this.cantidad = 0;
}

 public Producto(String nombre, double precio, int cantidad) {
    this.nombre = nombre;
    this.precio = precio;
    this.cantidad = cantidad;
 }
 
 public double ValorTotal() {
    return precio * cantidad;
}
 
 public void mostrarInformacion() {
    System.out.println("Nombre: " + this.nombre);
    System.out.println("Precio: $" + this.precio);
    System.out.println("Cantidad: " + this.cantidad);
    System.out.println("Valor Total: $" + ValorTotal());
}
      
 public void incrementarCantidad() {
    cantidad++;
}
 
 public void incrementarCantidad(int cantidadIncrementar) {
    cantidad += cantidadIncrementar;
}
 
public void actualizarPrecio(double nuevoPrecio) {
    precio = nuevoPrecio;
}

 public void actualizarPrecio(double nuevoPrecio, String moneda) {
    if (moneda.equals("euro")) {

        precio = nuevoPrecio * 0.93;
    } else if (moneda.equals("peso colombiano")) {

        precio = nuevoPrecio * 0.00003;
    }
}
 
 public void actualizarPrecio(double nuevoPrecio, String moneda, double tasaCambio) {
    if (moneda.equals("euro") || moneda.equals("peso colombiano")) {
        precio = nuevoPrecio * tasaCambio;
    }
 }    }



 MAIN
public static void main(String[] args) { {


Producto p1 = new Producto();
    Producto p2 = new Producto("Camiseta", 20.0);
    Producto p3 = new Producto("Zapatos", 100.0, 5);


    System.out.println("Información del Producto 1:");
    p1.mostrarInformacion();
    System.out.println();

    System.out.println("Información del Producto 2:");
    p2.mostrarInformacion();
    System.out.println();

    System.out.println("Información del Producto 3:");
    p3.mostrarInformacion();
    System.out.println();

  
    p1.incrementarCantidad();
    p2.incrementarCantidad(3);
    p3.actualizarPrecio(25.0);
    p3.actualizarPrecio(80.0, "euro");
    p2.actualizarPrecio(50000.0, "peso colombiano");
    p2.actualizarPrecio(100.0, "dólar", 1.2);  

  
    System.out.println("Información actualizada del Producto 1:");
    p1.mostrarInformacion();
    System.out.println();

    System.out.println("Información actualizada del Producto 2:");
    p2.mostrarInformacion();
    System.out.println();

    System.out.println("Información actualizada del Producto 3:");
    p3.mostrarInformacion();
} } }

Submódulo: Lógica de Programación Periodo: 2023-2
Estudiante: Jhon Mario Castrillón Gutierrez 





