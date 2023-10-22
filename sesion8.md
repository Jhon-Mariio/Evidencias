<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 


<!-- Su documentación aquí -->


Super clase Musica
public abstract class Musica {
public String tituloCancion;

public Musica(String tituloCancion) {
    this.tituloCancion = tituloCancion;
}

public void setTituloCancion(String tituloCancion) {
    this.tituloCancion = tituloCancion;
}
 public abstract void   play(); 
 public abstract void   stop(); 
 public abstract void   pause(); 
 public abstract void   next (); 
 public abstract void   previous(); 
}


Cancion
public class Cancion extends Musica {
private String artista;
private String Album;

public Cancion(String artista, String Album, String tituloCancion) {
    super(tituloCancion);
    this.artista = artista;
    this.Album = Album;
    
    
}

@Override
public void setTituloCancion(String tituloCancion) {
    super.setTituloCancion(tituloCancion); 
}

@Override
public void play() {
    System.out.println("Reproduccir");
    
}

@Override
public void stop() {
    System.out.println("Parar");
}

@Override
public void pause() {
   System.out.println("Pausar"); 
}

@Override
public void next() {
    System.out.println("Siguiente");
} 
   
@Override
public void previous() {
    System.out.println("Anterior");
}   
   
   
}

BandaSonora

public class BandaSonora extends Musica {

private String pelicula;

public BandaSonora(String pelicula, String tituloCancion) {
    super(tituloCancion);
    this.pelicula = pelicula;
}

@Override
public void play() {
    
    System.out.println("Reproduccir Pelicula");
    
}

@Override
public void stop() {
    System.out.println("Para pelicula");
          
}

@Override
public void pause() {
    System.out.println("Pausar pelicula");        
    
}

@Override
public void next() {
    System.out.println("Adelantar pelicula");
    
    
}

@Override
public void previous() {
    System.out.println("Retroceder pelicula");
    
   
}
}

Album

public class Album extends Musica{

private String canciones;

public Album(String canciones, String tituloCancion) {
    super(tituloCancion);
    this.canciones = canciones;
}

@Override
public void play() {
    System.out.println("Reproduccir Album");
    
   
}

@Override
public void stop() {
    System.out.println("Para album");
    
}

@Override
public void pause() {
    System.out.println("Pausar album");
    
}

@Override
public void next() {
   System.out.println("siguiente album");
    
}

@Override
public void previous() {
    System.out.println("Anterior album");
    
    
}
}

Submódulo: Lógica de Programación Periodo: 2023-2
Estudiante: Jhon Mario Castrillón Gutierrez 



