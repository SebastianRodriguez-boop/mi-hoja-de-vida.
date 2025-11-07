public class HojaDeVida {
 // Atributos
private String nombre;
private String correo;
private String[] estudios;
private String[] habilidades;

//  Constructor con tus datos personales
public HojaDeVida() {
this.nombre = "Sebastian David Rodriguez Guzman";
this.correo = "rodriguezguzmansebastian@gmail.com";

this.estudios = new String[]{
"Bachillerato Académico"
"Tecnico en asistencia administrativa"
"Estudiante de Ingeniería de Sistemas en UNIMINUTO"

};

this.habilidades = new String[]{
"Excelente manejo de las matemáticas",
"Facilidad para aprender cosas nuevas",
"Organizado y puntual"
};
}

//  Método para imprimir con formato
public void imprimir() {
System.out.println("HOJA DE VIDA\n");

System.out.println(" Nombre: " + nombre);
System.out.println(" Correo: " + correo);

System.out.println("\n Formación Académica:");
for (String e : estudios) {
System.out.println(" - " + e);
}

System.out.println("\n Habilidades:");
for (String h : habilidades) {
System.out.println(" - " + h);
}
}

//  Método principal
public static void main(String[] args) {
HojaDeVida hv = new HojaDeVida();
hv.imprimir();
}
}
