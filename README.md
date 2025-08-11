# -Administraci-n-de-Base-de-Datos-Relacional---COVID19-BCS
Proyecto de gestión de una base de datos MySQL para datos epidemiológicos de COVID-19 en Baja California Sur. Incluye diseño de esquema, automatización de respaldos, seguridad y monitoreo.
## Tecnologías
- MySQL 8.0+
- Python 3.x (para limpieza inicial)
- MySQL Workbench

## Estructura
/Data
├── COVID19MEXICO.csv # Datos fuente
├── bcs.csv # Datos filtrados
/Scripts
├── limpieza.py # Script de procesamiento
├── eventos.sql # Automatización

## Instalación
1. Importar esquema SQL:
   ```sql
   CREATE DATABASE bajal;
   USE bajal;

   Ejecutar scripts de creación de tablas (ver Docs/esquema.sql).

Uso
Respaldos programados:
CREATE EVENT backup_event ON SCHEDULE EVERY 3 DAY DO
-- Código de respaldo
Monitoreo:
ANALYZE TABLE registros;

Documentación
