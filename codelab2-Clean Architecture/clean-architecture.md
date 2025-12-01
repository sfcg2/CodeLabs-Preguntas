# Preguntas

   ## ¿Qué problema busca resolver Clean Architecture en el desarrollo de software?

        La clean architecture busca que la logica de negocio se separe de la infracestrucra, para que la logica
        sea facil de entender y pueda ser modifica sin afectar a lo demas.

   ## ¿Cuáles son las principales capas de Clean Architecture y qué responsabilidad tiene cada una?
      domain: ahi se almacena la logica de negocio (pura)
      application: aqui se ejecutan los casos de uso , que se ejecutan en el dominio con el que se comunica con interfaces.
      infraestructure: aqui se implementa la base de datos, seguridad, controllers, exceptions o persistencia en general detalles tecnicos.
      presentacion: seria ya el frontend/UI la parte visual 
      
   ## ¿Qué relación tiene Clean Architecture con el principio de Inversión de Dependencias (DIP) en SOLID?
      Como Clean Architecture es DIP, ademas de que el dominio su logica no depende de solo abstraciones sino de implementaciones concretas, por eso 
      define interfaces que son implentadas por la application.
      
   ## ¿Por qué es importante desacoplar la lógica de negocio de la infraestructura en una aplicación?
      porque al hacer cambios en bases de datos o los servicios que manejemos en la capa de infraestructura no afectara en nada a 
      la logica implementada
      
   ## ¿Cómo Clean Architecture facilita la escalabilidad y mantenibilidad de un sistema?
      porque maneja capas, donde cada una tiene una responsabilidad y al hacer cambios en el rendimiento o cambiar tecnologias evitamos
      dañar la logica de negocio.
      
   ## ¿Qué diferencia hay entre la capa de dominio y la capa de aplicación en Clean Architecture?
      en dominio se definen las reglas y entidades y application implementa esas reglas con casos de usos.
      
   ## ¿Por qué los controladores (controllers) y la base de datos deben estar en la capa de infraestructura?
      porque tienen detalles externos.
      
   ## ¿Qué ventajas tiene usar una interfaz en la capa de dominio para definir repositorios en lugar de usar directamente JpaRepository?
      porque JpaRepository hace parte de la infraestructura y si definimos ahi los repositorios podriamos dañar la logica de negocio.
   
   ## ¿Cómo interactúan los casos de uso (UseCases) con las entidades de dominio en Clean Architecture?
      Intereactuan mediante interfaces.
   
   ## ¿Cómo se puede aplicar Clean Architecture en una aplicación de microservicios con Spring Boot?
      Separando por capas, teniedno un dominio claro, sus casos de usos, interfaces y su infraestructura.

