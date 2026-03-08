# Herramienta de Documentación de Paquetes SSIS 🚀

[English](https://github.com/Cbas12/ssis_package_documentation_tool)

Esta herramienta automatiza el proceso de documentación de paquetes SQL Server Integration Services (SSIS) (archivos .dtsx). Al combinar las capacidades de análisis de Python con IA Generativa, extrae la lógica interna, flujos de control y transformaciones de datos para generar documentación completa y legible para humanos.

## 🚀 Características Principales
- **Análisis Automatizado:** Extrae metadatos, consultas SQL y lógica de tareas directamente de la estructura XML de archivos .dtsx.
- **Análisis Impulsado por IA:** Utiliza Modelos de Lenguaje Grande (LLMs) para explicar transformaciones complejas y lógica empresarial en lenguaje natural.
- **Salida en Markdown:** Genera documentación limpia y estructurada lista para ser alojada en GitHub, GitLab o wikis internos.
- **Eficiencia:** Reduce el tiempo de documentación para procesos ETL heredados o complejos.

## 💰 Eficiencia de Costos
Esta herramienta está diseñada para el procesamiento de múltiples archivos a bajo costo. Durante el desarrollo y pruebas:
- **Escalabilidad:** Documentó exitosamente más de 30 Procedimientos Almacenados.
- **Costo Total:** Menos de $2.50 USD (utilizando la API de Gemini).
- **Valor:** Documentación de alta velocidad a una fracción del costo del trabajo manual o herramientas empresariales.

## 🛠️ Stack Tecnológico
- **Lenguaje:** Python
- **Orquestación de IA:** API de Google Gemini
- **Librerías principales:** lxml para análisis XML, google-generativeai para documentación

## 📋 Requisitos Previos
Antes de ejecutar el notebook, asegúrate de tener:
- Python 3.10+
- Una Clave API de Google AI (Gemini).

⚙️ Configuración
1. **Clonar el repositorio:**
    git clone https://github.com/Cbas12/ssis_package_documentation_tool.git

2. **Configurar Credenciales:**
    - Utiliza el archivo gemini.txt para escribir tu propia Clave API de Gemini. Simplemente copia el texto dentro.

## 📖 Uso
1. Abre *ssis_package_documentation_tool_ESP.ipynb* en VS Code o Jupyter.
2. Asegúrate de haber agregado las rutas de entrada y salida:
 - *ssis_location*: La ruta de la carpeta que contiene tus archivos dtsx, param y conmgr.
 - *temp_output*: La carpeta donde la herramienta guardará temporalmente los resúmenes de los archivos param y conmgr para usarlos en combinación con los archivos dtsx limpios.
 - *docutentation_output_location*: La carpeta donde deseas que se guarden los archivos de documentación.
3. Se sugiere que, al principio de la sección *"PROCESAR LOS ARCHIVOS"* reduzcas el número de archivos procesados inicialmente, solo para asegurar que todo funciona según tus expectativas.
4. Ejecuta todas las celdas. La herramienta procesará cada archivo y generará una explicación detallada en lenguaje natural para cada DTSX.

## 📄 Licencia
Este proyecto es de código abierto. Siéntete libre de clonarlo, descargarlo y adaptarlo a tus propios flujos de trabajo de datos.