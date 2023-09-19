# PromedioArreglo

package promedio;

import java.util.Scanner;
import java.util.ArrayList;

public class promedio1 {
	
	public static void main(String[] args) {
		
		ArrayList Lis = new ArrayList();
		
		Scanner alum = new Scanner(System.in);
		Scanner alum1 = new Scanner(System.in);
		int cal[] = new int [5];
		int suma=0;
		float promedio;
		
		
		System.out.println("Calificaciones del Semestre uno\n");
		System.out.println("Ingresa el nombre del alumno(a): ");
		String nom = alum1.nextLine();
		//System.out.println("\n");
		
		System.out.println("Ingresa calificación materia 1: ");
		cal[0] = alum.nextInt();
		
		System.out.println("Ingresa calificación materia 2: ");
		cal[1] = alum.nextInt();
		
		System.out.println("Ingresa calificación materia 3: ");
		cal[2] = alum.nextInt();
		
		System.out.println("Ingresa calificación materia 4: ");
		cal[3] = alum.nextInt();
		
		System.out.println("Ingresa calificación materia 5: ");
		cal[4] = alum.nextInt();
				
		for (int i=0; i<cal.length; i++) {
			suma+=cal[i];
		}
		
		promedio = (suma/cal.length);
		System.out.println("Status de calificaciones. \n ");
		System.out.println("Nombre del estudiante : "+ nom);
		System.out.println(" ");
		System.out.println("Calificación 1 : "+ cal[0]);
		System.out.println("Calificación 2 : "+ cal[1]);
		System.out.println("Calificación 3 : "+ cal[2]);
		System.out.println("Calificación 4 : "+ cal[3]);
		System.out.println("Calificación 5 : "+ cal[4]);
		System.out.println(" ");
		System.out.println("Promedio : " + promedio);
		System.out.println(" ");
		
		if(promedio<=50) {
			System.out.println("Su calificación es : F ");
		}else if(promedio>=51 && promedio<=60) {
			System.out.println("su calificación es : E");
		}else if(promedio>=61 && promedio<=70) {
			System.out.println("Su calificacion es : D");
		}else if(promedio>=71 && promedio<=80) {
			System.out.println("Su calificacion es : C");
		}else if(promedio>=81 && promedio<=90) {
			System.out.println("Su calificación es : B");
		}else if(promedio>=91 && promedio<=100) {
			System.out.println("Su clificación es : A");
		}
	}

}
