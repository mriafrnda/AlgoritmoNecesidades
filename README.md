# AlgoritmoNecesidades

    Definir inter_necesitado, cel_necesitado, pc_necesitado, tablet_necesitado Como Entero;
    Definir costo_internet, costo_cel, costo_pc, costo_tablet Como Entero;
    Definir dispositivos_costo, total_general Como Entero;
    Definir correcto Como Cadena;
    Definir total_personas, prioridad_alta, prioridad_media, prioridad_baja Como Entero;
	
    prioridad_alta <- 0;
    prioridad_media <- 0;
    prioridad_baja <- 0;
	
    Escribir "Ingrese el número total de personas encuestadas:";
    Leer total_personas;
	
    Escribir "Ingrese el número de personas que necesitan internet:";
    Leer inter_necesitado;
	
    Escribir "Ingrese el número de personas que necesitan celulares:";
    Leer cel_necesitado;
	
    Escribir "Ingrese el número de personas que necesitan computadoras:";
    Leer pc_necesitado;
	
    Escribir "Ingrese el número de personas que necesitan tablets:";
    Leer tablet_necesitado;
	
    Escribir "¿Cuántas personas tienen prioridad ALTA (1)?";
    Leer prioridad_alta;
    Escribir "¿Cuántas personas tienen prioridad MEDIA (2)?";
    Leer prioridad_media;
    Escribir "¿Cuántas personas tienen prioridad BAJA (3)?";
    Leer prioridad_baja;
	
    Escribir "El total de vecinos en necesidad de internet y dispositivos tecnológicos es: ", inter_necesitado + tablet_necesitado + pc_necesitado + cel_necesitado;
	
    Escribir "Si la información es correcta, ¿desea continuar? (Si/No)";
    Leer correcto;
	
    Si correcto = "Si" Entonces
		
        Escribir "Ingrese el costo del internet por persona:";
        Leer costo_internet;
        Escribir "Costo total de internet: ", costo_internet * inter_necesitado, " soles";
		
        Escribir "Ingrese el costo por computadora:";
        Leer costo_pc;
        Escribir "Costo total de computadoras: ", costo_pc * pc_necesitado, " soles";
		
        Escribir "Ingrese el costo por tablet:";
        Leer costo_tablet;
        Escribir "Costo total de tablets: ", costo_tablet * tablet_necesitado, " soles";
		
        Escribir "Ingrese el costo por celular:";
        Leer costo_cel;
        Escribir "Costo total de celulares: ", costo_cel * cel_necesitado, " soles";
		
        dispositivos_costo <- (costo_pc * pc_necesitado) + (costo_cel * cel_necesitado) + (costo_tablet * tablet_necesitado);
        total_general <- dispositivos_costo + (costo_internet * inter_necesitado);
		
        Escribir "";
        Escribir "========= RESUMEN DE NECESIDADES =========";
        Escribir "Internet: ", inter_necesitado, " personas";
        Escribir "Computadoras: ", pc_necesitado;
        Escribir "Tablets: ", tablet_necesitado;
        Escribir "Celulares: ", cel_necesitado;
        Escribir "";
        Escribir "Prioridad alta: ", prioridad_alta;
        Escribir "Prioridad media: ", prioridad_media;
        Escribir "Prioridad baja: ", prioridad_baja;
        Escribir "";
        Escribir "El costo total a invertir es: ", total_general, " soles";
        Escribir "===========================================";
		
    SiNo
        Escribir "Operación cancelada.";
    FinSi

FinAlgoritmo
