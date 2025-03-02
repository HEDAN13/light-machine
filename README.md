# Maquina de luz Project - Firmware

This repository contains a compiled `.hex` file ready to be uploaded to an **Arduino UNO**.

## 📌 Description

This firmware allows the Arduino UNO to execute the code without needing to compile it from the source. Simply download the `.hex` file and follow the instructions to upload it to your board.

## 🛠 Requirements

- **Arduino UNO**
- **USB cable for Arduino**
- **Software to upload the .hex file** (avrdude, XLoader, or Arduino IDE)

## 🚀 Firmware Installation and Upload

### ✅ Option 1: Using `avrdude` (recommended method)

If you have `avrdude` installed, you can upload the `.hex` file using the following command:

```sh
avrdude -v -patmega328p -carduino -P COMX -b115200 -D -Uflash:w:firmware.hex:i
```

🔹 **Note:** Replace `COMX` with the correct port for your Arduino (Example: `COM3` on Windows or `/dev/ttyUSB0` on Linux).

### ✅ Option 2: Using XLoader (easier for beginners)

1. Download [**XLoader**](https://github.com/binaryupdates/xLoader).
2. Open XLoader and select:
   - `firmware.hex` in the file field.
   - "Uno" in the device option.
   - The COM port where your Arduino is connected.
3. Click **Upload**.

### ✅ Option 3: Using Arduino IDE (alternative method)

1. Open **Arduino IDE** and connect the Arduino UNO.
2. Go to **File > Preferences** and enable "Show verbose output during upload".
3. Upload any simple code and copy the upload command that appears in the console.
4. Replace the `.hex` file in that command and execute it in the terminal.

## 📜 License

This project is under the **MIT License**. You are free to use, modify, and distribute this firmware, as long as proper attribution is given.

---

📧 If you have any questions or issues, feel free to open an issue in this repository! 😊

---

# Proyecto Arduino UNO - Firmware

Este repositorio contiene un archivo `.hex` compilado para ser cargado en un **Arduino UNO**.

## 📌 Descripción

Este firmware permite que el Arduino UNO ejecute el código sin necesidad de compilarlo desde el código fuente. Simplemente descarga el archivo `.hex` y sigue las instrucciones para cargarlo en tu placa.

## 🛠 Requisitos

- **Arduino UNO**
- **Cable USB para Arduino**
- **Software para cargar el archivo .hex** (avrdude, XLoader, o Arduino IDE)

## 🚀 Instalación y carga del firmware

### ✅ Opción 1: Usar `avrdude` (método recomendado)

Si tienes `avrdude` instalado, puedes cargar el archivo `.hex` con el siguiente comando:

```sh
avrdude -v -patmega328p -carduino -P COMX -b115200 -D -Uflash:w:firmware.hex:i
```

🔹 **Nota:** Reemplaza `COMX` por el puerto correcto de tu Arduino (Ejemplo: `COM3` en Windows o `/dev/ttyUSB0` en Linux).

### ✅ Opción 2: Usar XLoader (más fácil para principiantes)

1. Descarga [**XLoader**](https://github.com/binaryupdates/xLoader).
2. Abre XLoader y selecciona:
   - `firmware.hex` en el campo de archivo.
   - "Uno" en la opción de dispositivo.
   - El puerto COM donde está conectado el Arduino.
3. Haz clic en **Upload**.

### ✅ Opción 3: Usar Arduino IDE (método alternativo)

1. Abre **Arduino IDE** y conecta el Arduino UNO.
2. Ve a **Archivo > Preferencias** y activa "Mostrar salida detallada durante carga".
3. Sube cualquier código simple y copia el comando de carga que aparece en la consola.
4. Reemplaza el archivo `.hex` en ese comando y ejecútalo en la terminal.

## 📜 Licencia

Este proyecto está bajo la **Licencia MIT**. Puedes usar, modificar y distribuir libremente este firmware, siempre que incluyas la atribución correspondiente.

---

📧 Si tienes dudas o problemas, ¡no dudes en abrir un issue en este repositorio! 😊

