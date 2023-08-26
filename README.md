# Tarea 1
codigo escrito en pseudocodigo

´´´

Algoritmo Conversor_de_medida
		
        //Ingresar la longitud en centimetros
		Escribir "Ingresa la longitud en centímetros:"
		Leer longitud_cm

		//Seleccionar la unidad de conversión
		Escribir "Selecciona a qué unidad deseas convertir:"
		Escribir "1. Metros"
		Escribir "2. Yardas"
		Escribir "3. Varas"
		Escribir "4. Pulgadas"
		Escribir "5. Pies"
		Leer opcion

		//Realizar la conversión según la unidad seleccionada
		Segun opcion Hacer
			Caso 1:
				longitud_convertida = longitud_cm / 100
				unidad_destino = " metros"
			Caso 2:
				longitud_convertida = longitud_cm / 91.44
				unidad_destino = " yardas"
			Caso 3:
				longitud_convertida = longitud_cm / 50.8
				unidad_destino = " varas"
			Caso 4:
				longitud_convertida = longitud_cm / 2.54
				unidad_destino = " pulgadas"
			Caso 5:
				longitud_convertida = longitud_cm / 30.48
				unidad_destino = " pies"
			De Otro Modo:
				Escribir "Opción no válida"
				
		Fin Segun
		
		//Mostrar el resultado de la conversión
		Escribir "La longitud de ", longitud_cm, " centímetros es igual a ", longitud_convertida, unidad_destino
		
	Fin Algoritmo
´´´
___

Codigo escrito en C++

´´´

using namespace std;

int main( ) {

    //Ingresar la longitud en centímetros
    float longitud_cm;
    cout << "Ingresa la longitud en centímetros: ";
    cin >> longitud_cm;
    
    //Seleccionar la unidad de conversión
    int opcion;
    cout << "Selecciona a qué unidad deseas convertir:" << endl;
    cout << "1. Metros" << endl;
    cout << "2. Yardas" << endl;
    cout << "3. Varas" << endl;
    cout << "4. Pulgadas" << endl;
    cout << "5. Pies" << endl;
    cin >> opcion;
    
    float longitud_convertida;
    string unidad_destino;
    
    //Realizar la conversión según la unidad seleccionada
    switch (opcion) {
        caso 1:
            longitud_convertida = longitud_cm / 100;
            unidad_destino = "metros";
            break;
        caso 2:
            longitud_convertida = longitud_cm / 91.44;
            unidad_destino = "yardas";
            break;
        caso 3:
            longitud_convertida = longitud_cm / 50.8;
            unidad_destino = "varas";
            break;
        caso 4:
            longitud_convertida = longitud_cm / 2.54;
            unidad_destino = "pulgadas";
            break;
        caso 5:
            longitud_convertida = longitud_cm / 30.48;
            unidad_destino = "pies";
            break;
        default:
            cout << "Opción no válida" << endl;
            return 1;
    }
    
    //Mostrar el resultado de la conversión
    cout << "La longitud de " << longitud_cm << " centímetros es igual a " << longitud_convertida << " " << unidad_destino << endl;
    
    return 0;
}

´´´
___

codigo escrito en python

´´´

#Ingresar la longitud en centímetros

longitud_cm = float(input("Ingresa la longitud en centímetros: "))

#Seleccionar la unidad de conversión

    print("Selecciona a qué unidad deseas convertir:")
    print("1. Metros")
    print("2. Yardas")
    print("3. Varas")
    print("4. Pulgadas")
    print("5. Pies")
    opcion = int(input())

#Realizar la conversión según la unidad seleccionada

if opcion == 1:

    longitud_convertida = longitud_cm / 100
    unidad_destino = "metros"
elif opcion == 2:

    longitud_convertida = longitud_cm / 91.44
    unidad_destino = "yardas"
elif opcion == 3:

    longitud_convertida = longitud_cm / 50.8
    unidad_destino = "varas"
elif opcion == 4:

    longitud_convertida = longitud_cm / 2.54
    unidad_destino = "pulgadas"
elif opcion == 5:

    longitud_convertida = longitud_cm / 30.48
    unidad_destino = "pies"
else:

    print("Opción no válida")
    exit(1)

#Mostrar el resultado de la conversión

print(f"La longitud de {longitud_cm} centímetros es igual a {longitud_convertida} {unidad_destino}")

´´´

