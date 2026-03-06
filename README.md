# DUNAB - Digital Universal Network of Automated Banking

**DUNAB** es una aplicación integral de simulación bancaria desarrollada en Java. Proporciona una interfaz gráfica de usuario (GUI) robusta para que los usuarios gestionen sus finanzas personales, incluyendo ahorros, inversiones y transacciones seguras.

Este proyecto fue desarrollado como parte de un curso de **Estructuras de Datos**, demostrando la integración de componentes GUI, gestión de bases de datos y lógica de negocios.

---

## 🚀 Características Principales

### 🔐 Gestión de Usuarios
- **Autenticación Segura**: Sistemas integrados de Inicio de Sesión y Registro.
- **Gestión de Perfil**: Visualización y gestión de la información del usuario (ID de cuenta, Nombre, Correo, etc.).

### 💰 Operaciones Financieras
- **Saldo en Tiempo Real**: Seguimiento de los montos *Disponible*, *Total* y *Guardado* (Ahorros).
- **Transferencias**: Envío de dinero entre cuentas de forma instantánea.
- **Depósitos y Retiros**: Operaciones bancarias estándar soportadas a través de una interfaz de teclado numérico personalizada.
- **Ahorros ("Cajitas")**: Movimiento de fondos a un área de ahorro dedicada para gestionar metas.

### 📈 Sistema de Inversión
- **Ganancias Simuladas**: Invierte una parte del saldo y recibe rendimientos aleatorios (1% a 3%) para simular el comportamiento del mercado.

### 📜 Historial de Transacciones
- **Feed en Vivo**: Visualización de las últimas 6 transacciones directamente en el dashboard.
- **Exportación Completa**: Descarga de todo el historial de transacciones en un archivo `.txt` para mantenimiento de registros offline.

### 📧 Notificaciones
- **Alertas por Correo**: Integración con JavaMail para notificar a los usuarios sobre actividades importantes de la cuenta.

---

## 🛠️ Stack Tecnológico

- **Lenguaje**: Java
- **Framework GUI**: Swing / AWT (con animaciones personalizadas y transiciones basadas en hilos).
- **Base de Datos**: MySQL vía JDBC (para la persistencia de datos de usuario y registros de transacciones).
- **Comunicación**: API JavaMail.
- **Soporte IDE**: NetBeans (estructura de proyecto basada en Ant).

---

## 📂 Estructura del Proyecto

- `Proyecto_inter/`: Directorio principal del proyecto Java.
    - `src/proyecto_inter/`: Contiene la lógica central y las clases GUI.
        - `Logis/`: Formularios de autenticación (`Login.java`, `register.java`).
        - `Conexion.java`: Gestión de la conexión a la base de datos.
        - `EnviarCorreo.java`: Servicio de notificación por correo electrónico.
    - `src/imagenes/`: Activos de la interfaz de usuario (iconos, fondos, botones).
- `design/`: Archivos fuente de diseño y SVG para los elementos visuales del proyecto.
- `DUNAB+ entrega.pdf`: Documentación del proyecto y detalles de la entrega.

---

## ⚙️ Requisitos e Instalación

1. **Java Development Kit (JDK)**: Versión 8 o superior.
2. **Base de Datos MySQL**:
    - Asegurarse de que el servidor MySQL esté en funcionamiento.
    - Configurar los detalles de conexión en `src/proyecto_inter/Conexion.java`.
3. **Librerías**:
    - `mysql-connector-java` para la conectividad de la base de datos.
    - `javax.mail` para las funciones de correo electrónico.

### Ejecución del Proyecto
Abrir la carpeta `Proyecto_inter` en **NetBeans** o cualquier IDE que soporte proyectos Ant, y ejecutar `Login.java` o el punto de entrada principal definido en la configuración del proyecto.

---

## 🎨 Experiencia Interactiva
La aplicación cuenta con transiciones de UI fluidas (Deslizar Arriba/Abajo/Izquierda/Derecha) utilizando implementaciones personalizadas de `Thread` para proporcionar una experiencia moderna y fluida en el escritorio.

---

> [!NOTE]
> Este proyecto fue diseñado con fines educativos para mostrar la gestión de datos y el diseño de interfaces de usuario en Java.
