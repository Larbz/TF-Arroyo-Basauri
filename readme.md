# Presentación del Proyecto: Drones de Delivery con Multi-Agent System (MAS)
![UPC_logo_transparente](./images/UPC_logo_transparente.png)

# Tópicos en Ciencias de la Computación

## Integrantes:
- Roberto Carlos Basauri Quispe
- Luis Roberto Arroyo Bonifaz

## 2023


## Introducción
En la era actual de la tecnología y la digitalización, la eficiencia en la entrega de productos es un factor crucial para las empresas. Nuestro equipo ha decidido abordar este desafío mediante la implementación de un sistema de entrega de drones utilizando un Sistema Multiagente (MAS). El objetivo es simular la entrega de productos en una ciudad con puntos de entrega predefinidos.

## Definición del Problema
El problema que abordamos es la entrega eficiente de productos en una ciudad. Los drones de entrega tienen el potencial de revolucionar la logística, pero su implementación presenta desafíos significativos. Estos incluyen la navegación segura, la optimización de rutas y la coordinación entre múltiples drones.

## Motivación
Nuestra motivación para este proyecto proviene de la creciente necesidad de soluciones de entrega rápidas y eficientes. Creemos que los drones de entrega, cuando se implementan correctamente, pueden proporcionar una solución efectiva. Además, este proyecto nos brinda la oportunidad de explorar y aplicar conceptos de MAS en un escenario del mundo real.

## Objetivos
Nuestro objetivo principal es desarrollar un sistema de simulación para la entrega de productos utilizando drones en una ciudad con puntos de entrega predefinidos. Queremos demostrar que un sistema bien diseñado puede mejorar la eficiencia y la velocidad de las entregas.

## Metodología
Para este proyecto, utilizaremos el conjunto PADE (Python Agent DEvelopment) para el desarrollo del MAS y QT para la interfaz gráfica. PADE es una herramienta poderosa y flexible para el desarrollo de sistemas multiagente en Python. QT, por otro lado, es un marco de trabajo para el desarrollo de interfaces gráficas de usuario.

1. **Selección de herramientas**: Hemos seleccionado PADE para el desarrollo del MAS debido a su flexibilidad y facilidad de uso. Para la interfaz gráfica, hemos seleccionado QT debido a su robustez y amplia gama de características.

2. **Configuración**: Configuraremos PADE y QT en nuestro entorno de desarrollo. Esto incluirá la instalación de las bibliotecas necesarias y la configuración de los parámetros necesarios para nuestro proyecto.

3. **Desarrollo de agentes**: Desarrollaremos varios agentes para nuestro sistema. Esto incluirá agentes para manejar la recepción de productos, la navegación a los puntos de entrega y la entrega de productos.

4. **Pruebas y optimización**: Una vez que hayamos desarrollado nuestros agentes, realizaremos pruebas exhaustivas para asegurarnos de que funcionan como se esperaba. También trabajaremos en la optimización de nuestros agentes para mejorar la eficiencia de las entregas.

## Diagrama
![Diagrama](./images/diagram.png)

## Implementación
Primero se crean las clases de los agentes a utilizar, Cliente y Dron, ambos heredan de la clase Agente que proporciona Pade. Cada agente tiene que tener definido un comportamiento, el del cliente estara ligado unicamente a un tiempo, el del dron a la recepcion de un mensaje de protocolo FIPA.
Luego tenemos que crear variables globales que nos ayudaran con los estados de nuestro agentes. Se crea un array para todos los agentes que se ejecutara en bucle, un array para guardar los clientes, un array para los drones, y una cola para los drones que nos ayudara a manejar las asignaciones de deliverys.
Despues de instanciados los agentes se procede a almacenar en las estructuras de datos. Se ejecutan los bucles y se proceden a definir las reglas de funcionamiento.

### Sprites
Cliente solicitando un pedido

![Cliente solicitando un pedido](./images/character.png)

Cliente alimentandose

![Cliente alimentandose](./images/characterEating.png)

Dron libre para pedido

![Dron libre para pedido](./images/dron.png)

Dron realizando un envio

![Dron realizando un envio](./images/dronBusy.png)

### Captura del programa

![Captura del programa](./images/programaSs.jpg)