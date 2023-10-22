<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 7 


<!-- Su documentación aquí -->

import java.util.logging.Logger; public class Productos {

public String Nombre; private double Precio; protected int Cantidad; final String Fabricante; static String Marca; String Categoria;

public Productos(String Nombre, double Precio, int Cantidad, String Fabricante, String Categoria) { this.Nombre = Nombre; this.Precio = Precio; this.Cantidad = Cantidad; this.Fabricante = Fabricante; this.Categoria = Categoria; }

public String getNombre() { return Nombre; }

public double getPrecio() { return Precio; }

public int getCantidad() { return Cantidad; }

public String getFabricante() { return Fabricante; }

public static String getMarca() { return Marca; }

public String getCategoria() { return Categoria; }

public void setNombre(String Nombre) { this.Nombre = Nombre; }

public void setPrecio(double Precio) { this.Precio = Precio; }

public void setCantidad(int Cantidad) { this.Cantidad = Cantidad; }

public static void setMarca(String Marca) { Productos.Marca = Marca; }

public void setCategoria(String Categoria) { this.Categoria = Categoria; }

}

MAIN public class Actividadad4 {

public static void main(String[] args) { Productos Productos1 = new Productos(“celular”, 800000, 2, “xiaomi”, “media”);

System.out.println(Productos1.getNombre()); System.out.println(Productos1.getPrecio()); System.out.println(Productos1.getCantidad()); System.out.println(Productos1.getFabricante()); System.out.println(Productos1.getCategoria());

Productos1.setNombre(“Smartphone”); System.out.println(Productos1.getNombre());

} }

Submódulo: Lógica de Programación Periodo: 2023-2
Estudiante: 




