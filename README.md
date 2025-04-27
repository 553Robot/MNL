# MNL

// ¡Bienvenido a MNL! Este es un lenguaje de programación en español que puedes usar para crear juegos, aplicaciones y más.
// Welcome to MNL! This is a programming language in Spanish that you can use to create games, apps, and more.

// A continuación, te explicaré los tipos de scripts y las condiciones que puedes usar en MNL.
// Below, I will explain the types of scripts and the conditions you can use in MNL.


// Tipos de Scripts en MNL:
// Types of Scripts in MNL:
// 1. ScriptGeneral: Afecta a todos los jugadores en la partida. // Affects all players in the game.
// 2. ScriptJugador: Solo se ejecuta en un jugador específico. // Runs only for a specific player.
// 3. ScriptServidor: Maneja la lógica del servidor y la interacción entre jugadores. // Handles server-side logic and player interaction.
// 4. ScriptUsuario: Se utiliza para aplicaciones y no videojuegos. // Used for applications, not games.


// Condiciones en MNL:
// Conditions in MNL:
// Las condiciones se utilizan para tomar decisiones dentro del código. Algunas de las más comunes son:
// Conditions are used to make decisions in the code. Some of the most common ones are:
// - si (if): Se usa para verificar si algo es verdadero y ejecutar un bloque de código si es cierto. // "si" (if): Used to check if something is true and execute code if it is.
// - entonces (then): Se usa junto con "si" para especificar lo que sucede si la condición es verdadera. // "entonces" (then): Used with "si" to specify what happens if the condition is true.
// - salva (else): Se usa para ejecutar un bloque de código si la condición no se cumple. // "salva" (else): Used to execute code if the condition is false.
// - verdadero (true): Es el valor de una condición cuando es cierto. // "verdadero" (true): The value of a condition when it's true.
// - falso (false): Es el valor de una condición cuando no se cumple. // "falso" (false): The value of a condition when it's false.


// Explicación de los Comentarios:
// Explanation of the Comments:
// Los comentarios son anotaciones que se agregan al código para explicar qué hace el código. No afectan la ejecución del programa. En MNL, los comentarios comienzan con "//" y todo lo que sigue es un comentario. Esto es útil para hacer que el código sea más fácil de entender y mantener.
// Comments are annotations added to the code to explain what the code does. They do not affect the execution of the program. In MNL, comments begin with "//" and everything following it is a comment. This is helpful to make the code easier to understand and maintain.


// Ahora veamos cómo usar estos conceptos en MNL:
// Now let's see how to use these concepts in MNL:


script("ScriptGeneral") // Este es un ejemplo de un ScriptGeneral. // This is an example of a ScriptGeneral.


si (jugador.vida < 50) entonces // Si la vida de un jugador es menor a 50... // If a player's health is less than 50...
    mostrar("¡Tu vida está baja, busca salud!") // Se muestra este mensaje a todos los jugadores. // This message will be shown to all players.
salva
    mostrar("Tu vida está a buen nivel.") // Si la vida es mayor o igual a 50, se muestra este mensaje. // If the health is greater than or equal to 50, this message will be shown.
fin


script("ScriptJugador") // Este script solo afecta a un jugador. // This script only affects one player.

si (jugador.nombre == "Juanito") entonces // Si el jugador se llama "Juanito"... // If the player is named "Juanito"...
    mostrar("¡Hola Juanito, prepárate para la batalla!") // Se muestra solo a Juanito. // This message will only be shown to Juanito.
salva
    mostrar("Bienvenido jugador, buena suerte.") // Si el jugador no es Juanito, se le muestra este mensaje. // If the player is not Juanito, this message will be shown.
fin

script("ScriptServidor") // Este es un script para la lógica del servidor. // This is a script for server-side logic.

si (tiempo_de_juego > 300) entonces // Si el tiempo de juego es mayor a 5 minutos... // If the game time is greater than 5 minutes...
    mostrar("¡Ya han pasado 5 minutos!") // Se muestra este mensaje a todos los jugadores. // This message will be shown to all players.
salva
    mostrar("El juego está en progreso.") // Si no han pasado 5 minutos, muestra esto. // If 5 minutes haven't passed, show this.
fin

script("ScriptUsuario") // Este es un script para aplicaciones, no juegos. // This script is for applications, not games.

si (boton_presionado == "Inicio") entonces // Si el jugador presiona el botón "Inicio"... // If the player presses the "Start" button...
    iniciar_juego() // Inicia el juego. // Start the game.
salva
    mostrar("Por favor, presiona 'Inicio' para comenzar.") // Si no se presiona el botón "Inicio", muestra esto. // If the "Start" button is not pressed, show this.
fin

// Resumen:
// Summary:
// 1. Los tipos de scripts determinan cómo y dónde se ejecuta el código en MNL (en todos los jugadores, en un jugador, en el servidor o en la aplicación). // The types of scripts determine how and where the code runs in MNL (for all players, for a single player, on the server, or in the application).
// 2. Las condiciones permiten controlar el flujo de ejecución en el código dependiendo de si ciertas condiciones son verdaderas o falsas. // Conditions allow you to control the flow of execution depending on whether certain conditions are true or false.
// 3. Las condiciones básicas son "si" (if), "entonces" (then), "salva" (else), "verdadero" (true), y "falso" (false). // Basic conditions are "si" (if), "entonces" (then), "salva" (else), "verdadero" (true), and "falso" (false).

// ¡Ahora estás listo para comenzar a usar MNL y crear tus propios proyectos!
// Now you're ready to start using MNL and create your own projects!

// ¡Sigue explorando las posibilidades con este increíble lenguaje de programación!
// Keep exploring the possibilities with this amazing programming language!