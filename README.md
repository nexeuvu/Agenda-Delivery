# Sistema de Gestión de Delivery
Este es un proyecto de gestión de pedidos de delivery. Utiliza Laragon como entorno de desarrollo local.
## Requisitos Previos
- Laragon (versión completa recomendada)
- MySQL
- PHP

## Pasos de Instalación

1. Clonar el repositorio:
```bash
git clone [https://github.com/sunombredeusuario/sistema-delivery.git](https://github.com/nexeuvu/Agenda-Delivery.git)
```

2. Abrir Laragon:
   - Iniciar servicios de Apache y MySQL
   - Abrir consola de MySQL

3. Crear Base de Datos:
```sql
CREATE DATABASE bd_delivery;
USE bd_delivery;
```

4. Importar Base de Datos:
   - Abrir la consola de MySQL en Laragon
   - Ejecutar el script SQL proporcionado `bd_delivery.sql`

## Estructura de la Base de Datos

### Tabla Login
- `id`: Clave primaria
- `nombre`: Nombre de usuario
- `email`: Correo electrónico
- `password`: Contraseña hash
- `rol`: Rol de usuario (admin/usuario)

### Tabla Pedidos
- `id`: Clave primaria
- `pedido`: Descripción del pedido
- `responsable`: Persona responsable del pedido
- `estado`: Estado del pedido
- `fecha`: Fecha del pedido
- `prioridad`: Prioridad del pedido
- `notas`: Notas adicionales

## Usuarios Predeterminados
- Admin: 
  - Correo: tiernoninio@gmail.com
- Usuarios Regulares:
  - Correo: cristianacunia@gmail.com
  - Correo: cristianpari@gmail.com

## Notas de Seguridad
- Contraseñas hash (bcrypt)
- Dos roles de usuario: admin y usuario

## Configuración Recomendada
- PHP 7.4+
- MySQL 8.0+
- Usar declaraciones preparadas para interacciones con base de datos

## Licencia
@Copyright NexeuVu
