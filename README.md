# CriptView

CriptView es una aplicación web de monitorización de criptomonedas desarrollada con Python y Streamlit.

Obtiene información del mercado de criptomonedas mediante la API de CoinGecko, almacena los precios históricos en una base de datos SQLite y muestra la información a través de un panel interactivo.

El proyecto combina integración de APIs, procesamiento de datos, gestión de bases de datos y visualización de información en una aplicación sencilla.

## Funcionalidades

* Consulta de precios actuales de criptomonedas.
* Variación porcentual de las últimas 24 horas.
* Almacenamiento de precios históricos.
* Integración con una base de datos SQLite.
* Consulta de registros históricos.
* Gráficos interactivos de evolución de precios.
* Actualización manual de los datos.

## Criptomonedas iniciales

* Bitcoin (BTC).
* Ethereum (ETH).
* Solana (SOL).

## Tecnologías utilizadas

Tecnología	Utilidad
Python	Lenguaje principal de desarrollo
CoinGecko API	Obtención de datos del mercado
Requests	Realización de peticiones HTTP
SQLite	Almacenamiento de datos históricos
SQL	Consultas y gestión de la base de datos
Pandas	Procesamiento y organización de datos
Streamlit	Desarrollo del panel interactivo

## Arquitectura

La aplicación sigue un flujo sencillo de obtención, procesamiento, almacenamiento y visualización de datos.

       CoinGecko API
             |
             v
       Python / Requests
             |
             v
       Procesamiento
          de datos
             |
             v
        Base de datos
           SQLite
             |
             v
       Interfaz Streamlit
             |
             v
           Usuario

## Estructura del proyecto

CriptView/
│
├── app.py
├── api.py
├── database.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── data/
  

## Instalación y ejecución

**Requisitos previos**

* Python 3.11 o superior.
* pip.
* Conexión a Internet.
* Acceso a la API de CoinGecko.

1. Clonar el repositorio

```git clone https://github.com/amedtorres/CryptView.git```

cd CriptView

2. Crear un entorno virtual

python -m venv .venv

Activar el entorno virtual:

Windows:

.venv\Scripts\activate

macOS / Linux:

source .venv/bin/activate

3. Instalar las dependencias

pip install -r requirements.txt

4. Configurar la API

Configurar las credenciales de CoinGecko si son necesarias según el plan de API utilizado.

Las claves de acceso se almacenarán mediante variables de entorno para evitar exponer información sensible en el código fuente.

5. Ejecutar la aplicación

streamlit run app.py

La aplicación se abrirá automáticamente en el navegador.

## Base de datos

CriptView utiliza SQLite como sistema de almacenamiento relacional local.

Los precios históricos de las criptomonedas se almacenarán para permitir consultar registros anteriores y representar su evolución mediante gráficos.

## La tabla principal tendrá una estructura similar a esta:

Campo	Descripción
id	Identificador único del registro
cryptocurrency	Nombre o identificador de la criptomoneda
price_eur	Precio registrado en euros
timestamp	Fecha y hora del registro

La base de datos se creará localmente al inicializar la aplicación.

## Objetivos del proyecto

Este proyecto permite trabajar con conceptos prácticos relacionados con el desarrollo de software y la ingeniería de datos:

* Integración de APIs REST.
* Procesamiento de datos JSON.
* Persistencia de datos.
* Bases de datos relacionales.
* Consultas SQL.
* Gestión de datos históricos.
* Visualización de datos.

## Mejoras futuras

Algunas funcionalidades que podrían incorporarse en futuras versiones:

* Incorporación de nuevas criptomonedas.
* Actualización automática de precios.
* Seguimiento de una cartera personal.
* Comparativas avanzadas del mercado.
* Nuevos indicadores históricos.

## Autor

Amed Torres

Desarrollador de Software Junior | IA & Data Engineering

* LinkedIn: www.linkedin.com/in/amed-torres-
* GitHub: https://github.com/amedtorres

## Aviso legal

CriptView es un proyecto educativo y de desarrollo personal.

Su finalidad es la monitorización del mercado de criptomonedas y la visualización de datos. No ofrece asesoramiento financiero ni ejecuta operaciones de compraventa.

⸻

Estado del proyecto: En desarrollo.
