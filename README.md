# MNL
Bienvenido a MNL! Este es un lenguaje en español, también la gente de habla inglesa lo puede usar/Welcome to MNL! This is a language in Spanish, but English-speaking people can also use it.
i will explain the sintaxis:

// This is a ScriptGeneral, it affects all players in the game
// Este es un ScriptGeneral, afecta a todos los jugadores en el juego

ScriptGeneral
    // If the player's X position is greater than 100, move them to the left
    // Si la posición X del jugador es mayor que 100, muévelo a la izquierda
    Si ("jugador.posX" > 100) entonces
        // This command moves the player to the left
        // Este comando mueve al jugador a la izquierda
        moverJugador("izquierda")
    Fin

    // If the player's health is below 50, show a warning
    // Si la salud del jugador es menor a 50, muestra una advertencia
    Si ("jugador.vida" < 50) entonces
        // Notify the player that they are low on health
        // Notifica al jugador que tiene poca salud
        mostrar("¡Cuidado! Poca vida")
    Fin
Fin

// Remember, ScriptGeneral affects all players in the game!
// ¡Recuerda, ScriptGeneral afecta a todos los jugadores en el juego!

// You can use ScriptJugador for player-specific actions
// Puedes usar ScriptJugador para acciones específicas de un jugador

ScriptJugador
    // This script only runs for the individual player
    // Este script solo se ejecuta para el jugador individual

    // If the player presses the "jump" key, make the player jump
    // Si el jugador presiona la tecla "salto", haz que el jugador salte
    Si ("jugador.tecla" == "salto") entonces
        // Make the player jump
        // Haz que el jugador salte
        saltar()
    Fin

    // If the player's score reaches 100, show a congratulatory message
    // Si la puntuación del jugador alcanza 100, muestra un mensaje de felicitación
    Si ("jugador.puntuacion" == 100) entonces
        // Congratulate the player for reaching 100 points
        // Felicita al jugador por alcanzar los 100 puntos
        mostrar("¡Felicidades! Alcanzaste 100 puntos")
    Fin
Fin

// ScriptServidor is for server-side actions that affect the game world
// ScriptServidor es para acciones del servidor que afectan el mundo del juego

ScriptServidor
    // If the game time exceeds 3600 seconds, end the game
    // Si el tiempo de juego excede los 3600 segundos, termina el juego
    Si ("tiempo_de_juego" > 3600) entonces
        // End the game after 1 hour of playtime
        // Termina el juego después de 1 hora de tiempo de juego
        terminarJuego()
    Fin

    // If the player's ping is above 200ms, show a warning
    // Si el ping del jugador es superior a 200ms, muestra una advertencia
    Si ("jugador.ping" > 200) entonces
        // Warn the player that their connection is slow
        // Advierte al jugador que su conexión es lenta
        mostrar("Advertencia: tu conexión es lenta")
    Fin
Fin

// Finally, ScriptUsuario is used for apps, not games
// Finalmente, ScriptUsuario se usa para aplicaciones, no juegos

ScriptUsuario
    // If the user presses the "submit" button, send the form data
    // Si el usuario presiona el botón "enviar", envía los datos del formulario
    Si ("usuario.boton" == "enviar") entonces
        // Send the form data
        // Envía los datos del formulario
        enviarFormulario()
    Fin
Fin
