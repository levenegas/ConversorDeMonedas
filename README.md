# ConversorDeMonedas
**Currency Converter (Java)**

Este proyecto es una **aplicación de consola en Java** que permite convertir montos entre diferentes monedas utilizando la API pública de ExchangeRate-API.

## 🧭 Características

- Conversión en tiempo real entre múltiples monedas.
- Validación de códigos de moneda soportados.
- Interfaz de línea de comandos fácil de usar.
- Mensajes interactivos personalizados para el usuario.

## 🗂 Estructura del Proyecto
![image](https://github.com/user-attachments/assets/6bdb58f6-5083-4f1a-af6f-e5075ebbf61d)

## 🗂 Diagrama de flujo,
![image](https://github.com/user-attachments/assets/7e7e6bab-bf62-4f3a-8852-14435352c326)

## 🔧 Requisitos
- Java JDK 8 o superior
- Conexión a internet (para consultar la API de tasas de cambio)
- json-20250107.jar [org.json](https://mvnrepository.com/artifact/org.json/json) (puedes descargar el `.jar` o agregarlo como dependencia)

## 📦 Dependencias
Este proyecto usa la librería **org.json** para manejar respuestas JSON. Puedes agregarla así:
Descarga el `.jar` desde: https://repo1.maven.org/maven2/org/json/json/  
Y agrégalo al classpath al compilar.

##▶️ Cómo Compilar y Ejecutar
- Compila el proyecto (asegúrate de incluir el .jar de json en el classpath):
javac -cp ".:json.jar" Main/CurrencyConverter.java APIs/ExchangeRateAPI.java CoinsUnits/Currency.java CoinsUnits/CurrencyList.java

- Ejecuta el programa:
  java -cp ".:json.jar" Main.CurrencyConverter

## 🌐🔑 Fuente de Datos
Se utiliza la ExchangeRate-API versión gratuita.
Clave de API utilizada en el código: c550377872bff94f79329430
     Puedes obtener tu propia API key gratuita registrándote en https://www.exchangerate-api.com/.

## 🌍 Monedas Soportadas
Algunas monedas disponibles en el sistema incluyen: USD, EUR, CRC, GBP, AUD, AED, ARS, entre otras.

## 📸 Ejemplo de uso
Bienvenido al conversor de monedas!, por favor ingrese su nombre:
> Carla

Códigos de Moneda Disponibles:
Código     Nombre                             País
---------------------------------------------------------------
USD        United States Dollar               United States
CRC        Costa Rican Colon                  Costa Rica
...

Ingrese el código de la moneda de origen (ej: USD), o escriba 'SALIR' para terminar:
> USD

Ingrese el código de la moneda destino (ej: EUR):
> EUR

Ingrese la cantidad a convertir:
> 100

*********************************************************
Carla, la cantidad 100.00 USD equivale a 92.35 EUR.
*********************************************************

##📜 Licencia
Este proyecto es de uso libre con fines educativos.
Puedes modificarlo o distribuirlo con fines no comerciales. Se recomienda incluir mención al autor original si se reutiliza públicamente.
