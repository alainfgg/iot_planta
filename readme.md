# Plataforma IoT para una Planta de Manufactura

## Descripción del Proyecto 
Sistema integral de Industria 4.0 diseñado para una planta de manufactura. El objetivo es recolectar datos de telemetría (temperatura y vibración) mediante una red de sensores IoT en maquinaria pesada para realizar mantenimiento predictivo mediante modelos de IA.

## Arquitectura seleccionada
Se implementa una Arquitectura Lakehouse. Esta elección permite la escalabilidad necesaria para el flujo constante de datos de sensores y la interoperabilidad para el entrenamiento de modelos de IA y visualización en dashboards.

## STACK Tecnológico
Para poder ejecutar este proyecto, se requieren de las siguientes herramientas y entornos de ejecución.

- Git: Control de versiones del código y documentación.

- Docker & Docker Compose: Oorquestación de contenedores (Kafka, bases de datos).

- Lenguaje: Python 3.9+

- Apache Kafka: Motor de ingesta para los flujos de datos en tiempo real.

- PostgreSQL / Delta Lake: Para el almacenamiento estructurado y analítico.

## Instrucciones de instalación

1.- Clonar el repositorio: git clone https://github.com/usuario/proyecto-iot-planta.git

2.- Configurar variables de entorno: Copiar el archivo `.env.example` a `.env` con las credenciales locales.

3.- Desplegar infraestructura: Ejecutar `docker-compose up -d` para levantar los servicios de Kafka y la base de datos.

4.- Instalar dependencias de Python: `pip install -r requirements.txt`

5.- Iniciar ingesta: Ejecutar `python scripts/ingesta_sensores.py`.

## Estructura del repositorio

├── data/               
├── docs/               
├── models/             
├── notebooks/          
├── scripts/            
├── docker-compose.yml  
└── README.md          

## Equipo

- Alain González García - Modelado, entrenamiento, visualización y documentación.