# 🍳 Chef Recetas (Recetas Estrella)

> **Chef Recetas** es una aplicación de escritorio desarrollada en **C# (Windows Forms)** bajo el patrón de arquitectura **Modelo-Vista-Controller (MVC)**. El sistema está diseñado para centralizar y optimizar la administración de recetas culinarias, permitiendo un control estructurado de categorías, ingredientes individuales, pasos detallados de preparación y almacenamiento de imágenes (fotografías) en formato binario directo en la base de datos.

Este sistema (también denominado *Recetas Estrella*) permite gestionar usuarios, categorías, ingredientes y recetas de manera sencilla y organizada, brindando una herramienta útil, robusta y limpia para almacenar y consultar información gastronómica de forma eficiente.

### ✨ Características Principales
* **Gestión Integral de Recetas:** Registro completo que incluye tiempos de preparación, porciones y niveles de dificultad (`fácil`, `media`, `difícil`).
* **Control de Almacenamiento BLOB:** Carga y lectura dinámica de archivos de imagen tanto para los ingredientes como para el resultado final de los platillos.
* **Módulo de Autenticación Seguro:** Acceso restringido mediante inicio de sesión con encriptación de contraseñas en SHA-256 a nivel de servidor.
* **Arquitectura MVC Separada por Capas:** Estructura limpia que independiza la interfaz de usuario (*Views*), la lógica de negocio (*Controllers*), el mapeo de objetos (*Models*) y el acceso a datos (*DAL*).
* **Persistencia de Datos Relacional:** Conectividad directa y eficiente con un servidor MySQL mediante el conector nativo `MySql.Data`.

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![.NET 8](https://img.shields.io/badge/.NET_8.0-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white)
![Windows Forms](https://img.shields.io/badge/Windows_Forms-0078D6?style=for-the-badge&logo=windows&logoColor=white)

---

## 👥 Integrantes del Equipo

El desarrollo e implementación de este proyecto fue realizado en conjunto por los siguientes integrantes:

| Nombre Completo | Número de Control | Roles |
| :--- | :---: | :---: |
| 👩‍💻 CHAVIRA RUÍZ JAZMÍN | `24580007` | Desarrollo & BD |
| 👩‍💻 DURÁN TOLENTINO AMANDA NOHEMÍ | `24580009` | Desarrollo & BD |
| 👩‍💻 GARCÍA ESPINOZA ANDREA | `24580011` | Desarrollo & BD |
| 🧑‍💻 ROMERO RAMÍREZ ALEXANDER | `24580028` | Desarrollo & BD |
| 👩‍💻 VILLAREAL VILLALOBOS NAIBY ADRIANA | `24580914` | Desarrollo & BD |

---

## 🚀 Instrucciones de Instalación

### Requisitos Previos

**Hardware Mínimo:**
* **Procesador:** Intel Core i3 o superior.
* **Memoria RAM:** 4 GB o superior.
* **Almacenamiento:** Espacio libre en disco de al menos 500 MB.

**Software Requerido:**
* **Sistema Operativo:** Windows 10 o superior.
* **IDE:** Visual Studio (.NET 8.0 o superior instalado).
* **Gestor de BD:** MySQL Server y MySQL Workbench.

---

### Pasos para Importar la BD y Configurar la Cadena de Conexión

Esta aplicación se distribuye a través de un archivo de solución (`.sln`). El usuario final solo necesita abrirlo en Visual Studio para compilar y ejecutar el código fuente.

1. **Descargar el proyecto:** Descarga la solución completa de *Recetas Estrella* y el script de la base de datos correspondiente de este repositorio.
2. **Importar la Base de Datos:**
   * Abre **MySQL Workbench** e ingresa a tu instancia local.
   * Abre y **ejecuta el script SQL** proporcionado para generar las tablas, relaciones y procedimientos iniciales.
3. **Configurar la Cadena de Conexión:**
   * Abre la solución (`.sln`) en **Visual Studio** (abre el tercer archivo de la lista principal para cargar todos los módulos del código).
   * Desde el *Explorador de Soluciones*, localiza la sección de configuración de acceso a datos (*DAL*) o los archivos del servidor.
   * Modifica la cadena de conexión con la liga, usuario y contraseña de tu servidor local `root`.
   * *Recomendación:* Puedes agregar las credenciales del administrador directamente en tu base de datos local para mantener la configuración por defecto y evitar alterar el código de conexión en MySQL.
4. **Compilación y Ejecución:**
   * Verifica que las dependencias de `MySql.Data` estén correctamente cargadas.
   * Compila y ejecuta la aplicación desde Visual Studio.
   * Inicia sesión con una cuenta de usuario previamente registrada o ingresa con los datos de la cuenta de administrador global.

---

## 📺 Liga al Video de Demostración

Puedes visualizar el comportamiento dinámico del recetario en nuestro video de referencia:

[![Ver Video de Demostración](https://img.youtube.com/vi/O4_nyyX341k/0.jpg)](https://youtu.be/O4_nyyX341k?si=e6xa_d6t6HGBrK1h)

🔗 **Enlace directo al video:** [https://youtu.be/O4_nyyX341k?si=e6xa_d6t6HGBrK1h](https://youtu.be/O4_nyyX341k?si=e6xa_d6t6HGBrK1h)

---

## 📸 Capturas de Pantalla Principales de la Aplicación

### Módulo de Login Inicial y Seguridad
<p align="center">
  <img width="367" height="331" alt="Login inicial 1" src="https://github.com/user-attachments/assets/2787d175-3acb-4534-92a6-1baa390ab21e" />
  <img width="369" height="332" alt="Login inicial 2" src="https://github.com/user-attachments/assets/e0cce7e5-5002-4e7c-9e9d-172b82df798d" />
</p>

### Registro de Nuevos Usuarios
<p align="center">
  <img width="336" height="330" alt="Registro de usuario" src="https://github.com/user-attachments/assets/81897f47-6638-4fb7-bd76-ac8d631baa29" />
</p>

### Gestión de Módulos (Vistas Principales y BLOBs)
<p align="center">
  <img width="1365" height="714" alt="Panel de Recetas" src="https://github.com/user-attachments/assets/38b1bc7e-ceef-4b8d-8fa3-914bb3d0077c" />
  <img width="1365" height="714" alt="Control de Categorías" src="https://github.com/user-attachments/assets/735f7069-587b-45e7-acf0-cbaadcdf6210" />
</p>

### Administración de Ingredientes y Pasos de Preparación
<p align="center">
  <img width="1365" height="718" alt="Edición de Ingredientes" src="https://github.com/user-attachments/assets/81982a01-6aee-4e8a-a761-4fd1b7b28777" />
  <img width="743" height="373" alt="Visualización Detallada" src="https://github.com/user-attachments/assets/90e5b6c9-9b87-4ef3-823a-866d32cbee6e" />
  <img width="1364" height="716" alt="Muestreo General" src="https://github.com/user-attachments/assets/16197992-a21b-402c-8436-a8b6c7c55be7" />
</p>

---

## 📊 Diagrama ER de la Base de Datos

Estructura relacional de las tablas y mapeo de objetos para el almacenamiento del catálogo de platillos y credenciales protegidas:

<p align="center">
  <img width="451" height="551" alt="Diagrama entidad-relacion" src="https://github.com/user-attachments/assets/3df74716-88bb-4290-a7a9-cd89bc4f4d9d" />
</p>
