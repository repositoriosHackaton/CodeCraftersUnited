# CodeCraftersUnited - Proyecto de Sistema de Inicio de Sesión Inteligente

En este repositorio, se encuentra el código creado por el grupo CodeCraftersUnited para el Proyecto Final del Módulo de Inteligencia Artificial del Samsung Innovation Campus (SIC) 2024. El proyecto se titula **"Sistema de Inicio de Sesión Inteligente: Autenticación Facial y Tradicional"**.

## Tabla de contenidos
- [Descripción](#descripción)
- [Arquitectura](#arquitectura)
- [Proceso de Desarrollo](#proceso-de-desarrollo)
- [Funcionalidades](#funcionalidades)
- [Estado del Proyecto](#estado-del-proyecto)
- [Agradecimientos](#agradecimientos)

## Descripción
Este proyecto tiene como objetivo desarrollar un sistema de inicio de sesión que combine autenticación facial y tradicional (usuario y contraseña). Utiliza técnicas avanzadas de visión por computadora y aprendizaje automático para garantizar la seguridad y la precisión en la autenticación de usuarios.

![Ejemplo del Sistema](path_to_image_or_gif) 

## Arquitectura
El sistema está compuesto por las siguientes capas:

1. **Interfaz de Usuario (UI)**: Desarrollada con Tkinter para proporcionar una experiencia de usuario intuitiva.
2. **Procesamiento de Imagen**: Utiliza OpenCV y MTCNN para la captura y detección de rostros.
3. **Almacenamiento de Datos**: Los datos de usuario y las imágenes faciales se almacenan localmente para su posterior comparación.
4. **Motor de Comparación**: Implementado con ORB y BFMatcher de OpenCV para comparar las imágenes faciales y determinar la autenticidad.

![Arquitectura del Proyecto](path_to_architecture_image)

## Proceso de Desarrollo
### Fuente del Dataset
- Se utilizan imágenes capturadas en tiempo real con una cámara web.

### Limpieza de Datos
- La detección y recorte de los rostros se realiza utilizando MTCNN para asegurar que solo se procesen las áreas relevantes de las imágenes.

![Proceso de Limpieza de Datos](path_to_data_cleaning_image)

### Manejo de Excepciones/Control de Errores
- El sistema maneja excepciones comunes como fallos en la captura de la imagen, errores en la lectura/escritura de archivos y problemas en la detección facial.

### Modelo de Machine Learning
- El sistema no utiliza un modelo de ML tradicional, pero emplea algoritmos de visión por computadora (MTCNN y ORB) para la detección y comparación de rostros.

### Estadísticos y Métricas
- La similitud entre las imágenes se evalúa utilizando ORB y se calcula un índice de similitud. Un valor de similitud mayor o igual a 0.98 se considera un inicio de sesión exitoso.

## Funcionalidades Extra
### Implementación de Chatbot
- En futuras versiones, se planea integrar un chatbot que asista a los usuarios en caso de problemas durante el inicio de sesión.

### Tecnología/Herramientas Usadas
- **Librerías**: Tkinter, OpenCV, Matplotlib, MTCNN, Numpy
- **Framework**: No se utiliza un framework específico, pero el proyecto se estructura de manera modular.

### Integración del Proyecto en una Página Web
- Se considera la posibilidad de migrar el sistema a una aplicación web utilizando Flask o Django en combinación con JavaScript para la captura de imágenes.

### Desarrollo de Interfaz Gráfica de Usuario
- La UI se desarrolla utilizando Tkinter, proporcionando una interfaz amigable y fácil de usar tanto para el registro como para el inicio de sesión.

## Estado del Proyecto
El proyecto está en su fase inicial y se encuentra en desarrollo activo. Se han implementado las funcionalidades básicas de registro y autenticación, y se están realizando pruebas para mejorar la precisión y la robustez del sistema.

## Agradecimientos
Agradecemos a Samsung Innovation Campus por la oportunidad y los recursos proporcionados para llevar a cabo este proyecto. También agradecemos a todos los miembros del equipo CodeCraftersUnited por su dedicación y esfuerzo.

---

Por favor, contribuyan a este proyecto mediante Pull Requests y reporten cualquier problema o sugerencia en la sección de Issues. ¡Gracias por su apoyo!
