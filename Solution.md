# ParcialCorte2_POO

#CONCEPTOS

1. ¿Cuáles son las acciones los tres momentos importantes de las excepciones? ¿Cuál es el objetivo de cada una? ¿Cómo se implementa en Java cada acción?

RTA/ Las tres momentos importantes de las excepciones son el try, el catch y el finally. El objetivo principal del try es capturar el error si se produce para posteriormente corregirlo, es decir, captura el código en el cual una posible excepción puede aparecer. Luego, el catch se encarga de definir el conjunto de instrucciones necesarias o de tratamiento del problema capturado con el bloque try anterior. Y por último, el finally se encarga de definir un conjunto de instrucciones necesarias tanto si se produce error o excepción como si no y que por tanto se ejecuta siempre.

Los tres momnetos de las excepciones se implementan de la siguiente forma:

 try{
    //Código que puede provocar errores
 }
 
 catch (Exception e) {
    //gestión del error e tipo Exception
}

finally {
    //código de finally
}


2. ¿Qué es sobre-escritura de métodos? ¿Por qué aplicarla? ¿Cómo impedir que se sobre-escriba un método?

RTA/ La sobre-escritura de métodos u override es una caracteristica que le permite a una subclase proporcionar una implementación especifica de un método que ya está provisto por una de sus superclases o clase padre. El override es muy útil cuando queremos que un método que ya existe se comporte de una manera diferente o especifica de acuerdo al contexto de un programa, también es muy útil a la hora de trabajar clases abstractas e interfaces. 

Para impedir que se sobre-escriba un método solo basta con hacer ese método final, y ya con esto ninguna clase podra hacer override de ese método. Por ejemplo:

public final String nombreMetodo();
