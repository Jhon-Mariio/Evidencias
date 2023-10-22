<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


<!-- Su documentación aquí -->

Superclase Conversor

public abstract class Conversor { protected String unidadOrigen; protected String unidadDestino;

public Conversor(String unidadOrigen, String unidadDestino) {
    this.unidadOrigen = unidadOrigen;
    this.unidadDestino = unidadDestino;
}

 public abstract double convertir(double cantidad); }

     }else if (unidadOrigen.equals("Onzas") && unidadDestino.equals("Gramos")){
        double resultado = cantidad * 28.3495;
        return resultado;
    }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Libras")){
        double resultado = cantidad * 2204.62;
        return resultado;
    }else if (unidadOrigen.equals("Libras") && unidadDestino.equals("Toneladas")){
        double resultado = cantidad * 0.000453592;
        return resultado;
    }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Gramos")){
        double resultado = cantidad * 1000000;
        return resultado;
    }else if (unidadOrigen.equals("Gramos") && unidadDestino.equals("Toneladas")){
        double resultado = cantidad * 0.000001;
        return resultado;
    }else if (unidadOrigen.equals("Toneladas") && unidadDestino.equals("Miligramos")){
        double resultado = cantidad * 1000000000;
        return resultado;
    }else if (unidadOrigen.equals("Miligramos") && unidadDestino.equals("Toneladas")){
        double resultado = cantidad * 0.000000001;
        return resultado;
    }else if (unidadOrigen.equals("Kilogramos") && unidadDestino.equals("Miligramos")){
        double resultado = cantidad * 1000000;
        return resultado;
    }else if (unidadOrigen.equals("Miligramos") && unidadDestino.equals("Kilogramos")){
        double resultado = cantidad * 0.000001;
        return resultado;
    }else{
        throw new IllegalArgumentException("Pesos no compatibles");
    }
}
}

Subclase Divisas
public class Divisas extends Conversor{
public Divisas(String unidadOrigen, String unidadDestino) {
    super(unidadOrigen, unidadDestino);
}

@Override
public double convertir(double cantidad) {
   if (unidadOrigen.equals("Dolar") && unidadDestino.equals("Euro")){
        double resultado = cantidad * 0.98;
        return resultado;
    } else if (unidadOrigen.equals("Euro") && unidadDestino.equals("Dolar")) {
        double resultado = cantidad * 1.06;
        return resultado;
    } else if (unidadOrigen.equals("Dólar") && unidadDestino.equals("Peso colombiano")) {
        double resultado = cantidad * 4073.34;
        return resultado;
    } else if (unidadOrigen.equals("Peso colombiano") && unidadDestino.equals("Dólar")) {
        double resultado = cantidad * 0.00025;
        return resultado;
    } else if (unidadOrigen.equals("Euro") && unidadDestino.equals("Peso colombiano")) {
        double resultado = cantidad * 4312.24;
        return resultado;
    } else if (unidadOrigen.equals("Peso colombiano") && unidadDestino.equals("Euro")) {
        double resultado = cantidad * 0.00023;
        return resultado;
    }else {
        throw new IllegalArgumentException("Divisas no compatibles");
    }
}
}
 




