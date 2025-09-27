## 🌡️ Control de Aerotermia Ferroli Omnia R32 con ESPHome

Este proyecto proporciona una configuración YAML para [ESPHome](https://esphome.io/) (ahora llamado **ESPBuilder**) que permite controlar una aerotermia **Ferroli Omnia R32** mediante **Modbus RTU** usando un **ESP32** (preferiblemente modelo **C3**).

> 🔄 Este repositorio es un **fork** de [Mosibi/Midea-heat-pump-ESPHome](https://github.com/Mosibi/Midea-heat-pump-ESPHome), con entidades adicionales específicas del modelo **R290**, incluyendo:
>
> - COP instantáneo
> - Generación de potencia clasificada por ACS, frío o calor
> - Energía renovable generada
> - Consumo de potencia

---

### 🧬 Compatibilidad

Aunque solo ha sido testeado en el modelo **Ferroli Omnia R32 ST3.2 de 10kW**, esta configuración es compatible con toda la familia de aerotermias derivadas de **Midea**, como:

- Ferroli
- Midea
- Mundoclima
- Kosner R32
- EAS

---

### 🛠️ Requisitos

- ESP32 (preferiblemente C3)
- Conversor Modbus RS485 (TTL-RS485)
- Aerotermia con soporte Modbus RTU (ID de esclavo: 1)
- Home Assistant con ESPBuilder (ESPHome) integrado

---

### ⚙️ Personalización necesaria

Antes de compilar el YAML, asegúrate de ajustar:

- 🔧 Pines GPIO para la conexión Modbus
- 🔐 Clave de API (`api_key`)
- 🔑 Contraseña OTA (`ota_password`)
- 🧩 Variables de configuración específicas de tu instalación

---

### 🚀 Instalación

1. Conecta el ESP32 al bus RS485 de la aerotermia.
2. Ajusta las variables en el YAML según tu instalación.
3. Compila y flashea el firmware con ESPBuilder.
4. Añade el dispositivo a Home Assistant.
5. ¡Empieza a monitorizar y controlar tu aerotermia!

---

### 📊 Funcionalidades

- Lectura de temperaturas, presiones y estados del sistema
- Control de modos de funcionamiento (calefacción, refrigeración, ACS)
- Monitorización energética avanzada
- Integración completa con Home Assistant

---

### 🧪 Estado del proyecto

✅ Testeado en Ferroli Omnia R32 ST3.2 10kW  
🧪 Experimental para otros modelos Midea
PENDIENTE:
- añadir entidad climate de forma nativa
- limpiar entidades sin uso



---

## 🌡️ Control of Ferroli Omnia R32 Heat Pump with ESPHome

This project provides a YAML configuration for [ESPHome](https://esphome.io/) (now called **ESPBuilder**) to control a **Ferroli Omnia R32** heat pump via **Modbus RTU** using an **ESP32** (preferably **C3** model).

> 🔄 This repository is a **fork** of [Mosibi/Midea-heat-pump-ESPHome](https://github.com/Mosibi/Midea-heat-pump-ESPHome), with additional entities specific to the **R290** model, including:
>
> - Instantaneous COP
> - Power generation classified by DHW, cooling, or heating
> - Renewable energy generated
> - Power consumption

---

### 🧬 Compatibility

Although only tested on **Ferroli Omnia R32 ST3.2 10kW**, this configuration is compatible with the full family of **Midea-derived** heat pumps:

- Ferroli
- Midea
- Mundoclima
- Kosner R32
- EAS

---

### 🛠️ Requirements

- ESP32 (preferably C3)
- Modbus RS485 converter (TTL-RS485)
- Heat pump supporting Modbus RTU (slave ID: 1)
- Home Assistant with ESPBuilder (ESPHome) integration

---

### ⚙️ Required Customization

Before compiling the YAML, make sure to adjust:

- 🔧 GPIO pins for Modbus connection
- 🔐 API key (`api_key`)
- 🔑 OTA password (`ota_password`)
- 🧩 Configuration variables specific to your setup

---


### 🚀 Installation

1. Connect the ESP32 to the RS485 bus of the heat pump.
2. Adjust the YAML variables to match your setup.
3. Compile and flash the firmware using ESPBuilder.
4. Add the device to Home Assistant.
5. Start monitoring and controlling your heat pump!

---

### 📊 Features

- Read temperatures, pressures, and system states
- Control operating modes (heating, cooling, DHW)
- Advanced energy monitoring
- Full Home Assistant integration

---

### 🧪 Project Status

✅ Tested on Ferroli Omnia R32 ST3.2 10kW  
🧪 Experimental for other Midea-based models

