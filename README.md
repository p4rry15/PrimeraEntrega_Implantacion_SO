# Manual de Infraestructura Linux

Este repositorio contiene las prácticas y procedimientos documentados en el **Manual de Infraestructura Linux**, desarrollado por Carlos Parriego Urbano para el curso de 1° de ASIR. Es una guía práctica paso a paso para la administración de servidores, gestión de identidades y aplicación de políticas de seguridad en entornos GNU/Linux.

## 📋 Contenido del Proyecto

El manual se divide en seis bloques principales que cubren desde la administración básica hasta la seguridad avanzada:

### 1. Estructura de Directorios Eficiente
* Uso de `mkdir -p` y expansión de llaves `{}` para generar jerarquías complejas en una sola línea.
* Gestión de permisos de escritura en rutas del sistema como `/var` mediante `sudo`.

### 2. Gestión de Usuarios y Grupos (ASIR)
* Creación de grupos departamentales (dev, ops, mark, etc.).
* Automatización de alta de usuarios con directorios personales y shell interactiva.
* Configuración masiva de contraseñas y gestión del ciclo de vida de cuentas (bloqueo y borrado).

### 3. Políticas de Seguridad y Permisos Avanzados
* Implementación de permisos en notación octal.
* **SGID (Set Group ID):** Configuración de directorios colaborativos para herencia de grupo.
* **SUID (Set User ID):** Ejecución de scripts con privilegios delegados.
* **Sticky Bit:** Protección de archivos en directorios públicos para evitar borrados accidentales.

### 4. Auditoría y Monitorización
* Localización de archivos huérfanos y gestión de propietarios con `find`.
* Filtrado de usuarios reales del sistema mediante el análisis de UIDs en `/etc/passwd`.
* Seguimiento de inicios de sesión y actividad del sistema.

### 5. Listas de Control de Acceso (ACL)
* Configuración de seguridad granular para definir permisos específicos por usuario más allá del estándar UGO (User, Group, Others).

### 6. Reportes Automatizados
* Generación de informes de auditoría que incluyen:
  * Estado de contraseñas de los usuarios.
  * Verificación de privilegios administrativos (SUDO).
  * Consolidación de datos en archivos de texto con marcas de tiempo.

---
**Autor:** Carlos Parriego Urbano  
**Curso:** 1° ASIR - Implantación de Sistemas Operativos
