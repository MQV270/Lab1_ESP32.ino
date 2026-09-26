# Laboratorio 1 – Generación y calibración de señales analógicas con ESP32

## Descripción

Este repositorio contiene los archivos correspondientes al Laboratorio de Taller de Equipos Biomédicos II.

El proyecto tiene como objetivo generar y calibrar una señal analógica utilizando un ESP32 mediante dos métodos de salida:

- Conversión digital-analógica (DAC).
- Modulación por ancho de pulso (PWM) con filtrado RC.

## Implementación

El programa permite ingresar mediante el Monitor Serial un voltaje deseado entre 0.00 y 3.30 V.

La salida DAC se genera mediante el GPIO25 y la salida PWM mediante el GPIO27.

La señal PWM se configura con una frecuencia de 5000 Hz y una resolución de 8 bits. Posteriormente, se utiliza un filtro RC pasabajos para obtener una señal continua aproximada.

El programa también muestra en el Monitor Serial el voltaje ingresado, el código de 8 bits calculado y el voltaje teórico correspondiente.

## Archivos

### Laboratorio_1_ESP32.ino
Código fuente utilizado para la generación simultánea de las salidas DAC y PWM del ESP32.

### Montaje_Proteus.pdsprj
Archivo del proyecto utilizado para representar el montaje del circuito en Proteus.

## Componentes principales

- ESP32
- Resistencia
- Capacitor
- Protoboard
- Cables jumper
- Osciloscopio
- Multímetro digital

## Resultados

Se realizaron mediciones de voltaje para diferentes valores programados y se compararon las salidas DAC y PWM filtrada mediante el cálculo del error porcentual y la estimación de la resolución.

## Referencia

Laboratorio 1 – Generación y calibración de una señal analógica con ESP32.
Taller de Equipos Biomédicos II – UNMSM.
