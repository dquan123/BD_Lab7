# Lab 7 - Visualización de Datos
**CC3088 - Bases de Datos 1 | Ciclo 1, 2026**
**Universidad del Valle de Guatemala**

## Área asignada: Marketing (Área 4)

RetailMax es una cadena de tiendas con presencia en múltiples regiones del país. 
Este dashboard analítico fue construido para el área de Marketing, enfocándose en 
el análisis de campañas comerciales y la segmentación de clientes.

## Video de presentación
https://youtu.be/ta_OgXJFUZY

## Dashboard
El dashboard contiene 2 tabs con 6 indicadores cada uno:
- **Tab 1: Campañas y Rendimiento** — Analiza efectividad, alcance e inversión de campañas
- **Tab 2: Clientes y Segmentación** — Analiza comportamiento y valor de cada segmento

## Instrucciones para ejecutar

### Requisitos
- Docker Desktop instalado y corriendo

### Pasos
1. Clonar el repositorio
2. Abrir una terminal en la carpeta del proyecto
3. Ejecutar:
```bash
   docker compose up
```
4. Esperar 5-10 minutos a que PostgreSQL cargue los datos y Metabase inicialice
5. Abrir el navegador en `http://localhost:3000`
6. Iniciar sesión con:
   - **Email:** calificar@uvg.edu.gt
   - **Contraseña:** secret123+
7. El dashboard aparece en **Nuestros análisis → Marketing RetailMax**

## Estructura del repositorio
├── docker-compose.yml        # Ambiente completo PostgreSQL + Metabase

├── init/

│   ├── 00_create_metabase_db.sql  # Crea la base de datos de Metabase

│   ├── 01_DDL.sql                 # Estructura de la base de datos RetailMax

│   ├── 02_DATA.sql                # Datos de RetailMax

│   └── 03_metabase_app.sql        # Dashboard y configuración de Metabase

├── metabase-data/            # Volumen persistente de Metabase

├── informe.pdf               # Documentación de los 12 indicadores

└── README.md

## Integrante
- Diego Quan
