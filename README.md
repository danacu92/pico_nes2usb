# ENGLISH
# NES Controller to USB Adapter 
## Overview

This project implements an adapter to connect an NES (Nintendo Entertainment System) controller to a computer via USB using a Raspberry Pi Pico (RP2040). The adapter translates NES controller inputs into USB HID reports like a standard USB gamepad, allowing the controller to be used on modern systems. It was developed in C using Visual Studio Code with the Raspberry Pi Pico extension and uses the TinyUSB library.

## Requirements

### Hardware
- Raspberry Pi Pico (RP2040)
- NES controller
- Micro USB cable
- Optional: Female connector or extension cable for the NES controller for more robust wiring

### Software
- Visual Studio Code with the [Raspberry Pi Pico extension](https://marketplace.visualstudio.com/items?itemName=raspberry-pi.raspberry-pi-pico)
- Raspberry Pi Pico SDK
- TinyUSB library (included in the Pico SDK)
- CMake and a compatible C compiler (e.g., GCC for ARM)

## Instructions

1. **Hardware Connection**
   - Connect the NES controller to the Raspberry Pi Pico according to the following schematic:
![Connection Schematic](https://github.com/user-attachments/assets/72919f68-bb07-4a20-b9b2-63b6456f92c2)

2. **Firmware Loading**
   - Connect the Raspberry Pi Pico to your computer while holding down the **BOOTSEL** button.
   - Download the `.uf2` file available in the *releases* section of this repository.
   - Drag the `.uf2` file to the Pico’s storage device.
   - The Pico will automatically restart and be ready to use with the NES controller.

## Compilation

1. Clone or download this repository.
2. Open Visual Studio Code and install the [Raspberry Pi Pico extension](https://marketplace.visualstudio.com/items?itemName=raspberry-pi.raspberry-pi-pico).
3. In the left sidebar, select the **Raspberry Pi Pico Project** section.
4. Choose the **Import Project** option and select the downloaded project folder.
5. The project should now be ready to compile.

## Notes

- The project assumes the use of the standard NES controller protocol. Non-standard or third-party controllers may require adjustments.
- The adapter was successfully tested on a PC using RetroArch and on a Raspberry Pi with RetroPie.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
# ESPAÑOL
# Adaptador de Control NES a USB

## Descripción General

Este proyecto implementa un adaptador para conectar un control de NES (Nintendo Entertainment System) a una computadora mediante USB utilizando una Raspberry Pi Pico (RP2040). El adaptador traduce las entradas del control NES en reportes USB HID como un gamepad USB, lo que permite usar el control en sistemas modernos. Fue desarrollado en C usando Visual Studio Code con la extensión Raspberry Pi Pico y utiliza la librería TinyUSB.

## Requisitos

### Hardware
- Raspberry Pi Pico (RP2040)
- Control NES
- Cable micro USB
- Opcional: Conector hembra o cable alargador para el control NES, para un cableado más prolijo y robusto

### Software
- Visual Studio Code con la [extensión de Raspberry Pi Pico](https://marketplace.visualstudio.com/items?itemName=raspberry-pi.raspberry-pi-pico)
- SDK de Raspberry Pi Pico
- Librería TinyUSB (incluida en el SDK de Pico)
- CMake y un compilador C compatible (por ejemplo, GCC para ARM)

## Instrucciones

1. **Conexión del Hardware**
   - Conecta el control NES a la Raspberry Pi Pico según el siguiente esquema:
![Connection Schematic](https://github.com/user-attachments/assets/72919f68-bb07-4a20-b9b2-63b6456f92c2)
2. **Carga del Firmware**
   - Conecta la Raspberry Pi Pico a tu computadora mientras mantienes presionado el botón **BOOTSEL**.
   - Descarga el archivo `.uf2` disponible en la sección de *releases* de este repositorio.
   - Arrastra el archivo `.uf2` a la unidad de almacenamiento de la Pico.
   - La Pico se reiniciará automáticamente y estará lista para usar con el control de NES.

## Compilación

1. Clona o descarga este repositorio.
2. Abre Visual Studio Code e instala la [extensión de Raspberry Pi Pico](https://marketplace.visualstudio.com/items?itemName=raspberry-pi.raspberry-pi-pico).
3. En la barra lateral izquierda, selecciona la sección **Raspberry Pi Pico Project**.
4. Elige la opción **Importar Proyecto** y selecciona la carpeta del proyecto descargado.
5. Con eso ya deberia estar listo para compilar.


## Notas

- El proyecto asume el uso del protocolo estándar del control NES. Controles no estándar o de terceros podrían requerir ajustes.
- El adaptador fue probado con éxito en PC usando RetroArch y en una Raspberry Pi con RetroPie.
