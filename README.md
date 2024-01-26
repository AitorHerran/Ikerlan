# Sistema de Seguridad para Freno de Vehículo
## Descripción
Este proyecto implementa un sistema de seguridad para el frenado de emergencia de un vehículo utilizando el kit de desarrollo de Renesas EK-RA4M1. El objetivo es desarrollar un prototipo que monitoree constantemente la velocidad del sistema y genere una alerta cuando esta supere un umbral de seguridad.

## Tecnologías Utilizadas
I2C
UART
ADC
MQTT
ARM-Cortex
Python
C


## Características Principales
Inicio del sistema mediante un pulsador y visualización en un display LCD.
Lectura continua de la velocidad del vehículo y filtrado de datos para evitar outliers.
Registro de datos y timestamps en un log a través de la Raspberry Pi.
Activación de un freno de emergencia al superar un umbral de velocidad.
Publicación de mensajes en un broker MQTT cuando se activa el freno de emergencia.
Vuelta al estado "SYSTEM ON" cuando la velocidad baja del umbral de emergencia.
Requisitos Funcionales y No Funcionales
Uso del lenguaje C para la EK y Python para la Raspberry Pi.
Implementación de un sistema de diagnóstico safety (CRC) opcional.
Integración con sensores de movimiento, luz, temperatura y humedad como mejoras opcionales.
