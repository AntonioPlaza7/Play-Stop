# Play-Stop

# Aplicación Android: Reproductor de Audio Básico

Este proyecto es una aplicación básica de reproducción de audio para Android, desarrollada en **Android Studio** utilizando **Kotlin** y **XML**. Fue creada como parte del módulo de **Programación Multimedia y Dispositivos Móviles (PMDM)** del ciclo formativo **DAM (Desarrollo de Aplicaciones Multiplataforma)** en CESUR Andalucía. Su objetivo principal es demostrar el uso de la clase `MediaPlayer` para reproducir archivos de audio almacenados localmente o desde una URL.

## Sobre el Proyecto

La aplicación es un ejercicio práctico para comprender cómo gestionar la reproducción de audio en Android. Proporciona una interfaz de usuario sencilla con botones para controlar la reproducción de una pista de audio: "Reproducir", "Pausar" y "Detener". Además, se ha configurado para liberar los recursos del `MediaPlayer` cuando la aplicación ya no los necesita, lo que es crucial para un buen rendimiento y evitar fugas de memoria.

## Características

* **Reproducción de Audio:** Capacidad para reproducir un archivo de audio (MP3) desde los recursos de la aplicación (`res/raw`) o desde una URL externa.
* **Controles de Reproducción:** Botones intuitivos para:
    * **Reproducir:** Inicia o reanuda la reproducción del audio.
    * **Pausar:** Detiene temporalmente la reproducción.
    * **Detener:** Detiene completamente la reproducción y reinicia la posición.
* **Gestión de Recursos:** Implementación para liberar los recursos del `MediaPlayer` (`release()`) cuando la actividad se destruye, evitando problemas de memoria.
* **Interfaz de Usuario Sencilla:** Diseño claro y funcional para facilitar la interacción con los controles de audio.
* **Compatibilidad:** Probado en un emulador de dispositivo Pixel 8.

## Tecnologías Utilizadas

* **Android Studio:** IDE principal para el desarrollo de aplicaciones Android.
* **Kotlin:** Lenguaje de programación utilizado para la lógica de la aplicación.
* **XML:** Utilizado para definir el diseño de la interfaz de usuario (layouts en `activity_main.xml`).
* **Android SDK:** Con la versión de API necesaria para el desarrollo multimedia.

## Estructura del Proyecto

El proyecto sigue una estructura estándar de Android, con los siguientes componentes clave:

* **`app/src/main/java/com/tu_paquete/tu_app/MainActivity.kt`**:
    * Contiene la lógica principal de la aplicación.
    * Maneja la inicialización y el control del objeto `MediaPlayer`.
    * Define los métodos para `play()`, `pause()`, y `stop()` del audio.
    * Implementa los `OnClickListener` para los botones de la UI.
    * Sobrescribe el método `onDestroy()` para liberar los recursos del `MediaPlayer`.
* **`app/src/main/res/layout/activity_main.xml`**:
    * Define el diseño visual de la interfaz de usuario.
    * Incluye `Button`s para "Reproducir", "Pausar" y "Detener".
    * Organiza los botones en un `LinearLayout` (o similar) verticalmente.
* **`app/src/main/res/raw/`**:
    * Carpeta donde se almacena el archivo de audio local (ej. `audio.mp3`) que la aplicación reproduce.

## Aprendizajes Clave

Durante el desarrollo de este proyecto, se han consolidado los siguientes conocimientos y habilidades:

* Desarrollo de Aplicaciones Android: Creación de una aplicación móvil funcional.
* Reproducción Multimedia en Android: Uso de la clase MediaPlayer para controlar audio.
* Gestión de Recursos Multimedia: Carga de audio desde recursos locales y URLs.
* Control de Interfaz de Usuario: Implementación de Buttons y OnClickListener para interactividad.
* Gestión del Ciclo de Vida de MediaPlayer: Importancia de liberar recursos para optimizar el rendimiento y evitar fugas de memoria.
* Diseño de Layouts con XML: Organización de elementos en la interfaz gráfica de Android.
* Este ejercicio proporciona una base sólida para futuros proyectos que requieran funcionalidades multimedia en aplicaciones Android.
