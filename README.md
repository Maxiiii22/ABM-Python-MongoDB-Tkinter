# 📋 **Sistema de Gestión de Empleados**

Este proyecto es una **aplicación de escritorio para la gestión de empleados**, desarrollada en **Python** utilizando las bibliotecas **CustomTkinter**, **Tkinter**, y **MongoDB** como base de datos. Permite realizar operaciones básicas de **ABM (Alta, Baja y Modificación)** sobre un registro de empleados.

![Vista previa de la aplicación](Vista-previa.jpg)

---

## 🧰 **Funcionalidades Principales**

- **Agregar (Alta) empleados**: Ingreso de nombre, apellido y edad. Se genera automáticamente un ID.
- **Modificar empleados**: Búsqueda por ID, edición de los campos, y guardado de los cambios.
- **Eliminar empleados**: Eliminación de un registro existente por ID.
- **Visualización en tiempo real**: Muestra todos los empleados en una tabla (`TreeView`), con filtro en tiempo real por ID, nombre, apellido o edad.
- **Interfaz moderna**: Utiliza `CustomTkinter` para una interfaz más estética y funcional.

---

## 🧠 **Tecnologías utilizadas**

- **Python 3**
- **Tkinter**: Biblioteca para crear interfaces gráficas de usuario (GUI).
- **CustomTkinter**: Estilo moderno para los botones y cuadros de texto.
- **MongoDB**: Base de datos NoSQL para almacenar los registros de empleados.
- **ttk.Treeview**: Widget de Tkinter para mostrar datos en formato de tabla.

---

## 🗃️ **Estructura de la Base de Datos**

La base de datos **MongoDB** contiene una colección llamada `empleados` con los siguientes campos:

```javascript
{
    "_id": <ObjectId>,          // ID único del empleado (autogenerado)
    "nombre": <String>,         // Nombre del empleado
    "apellido": <String>,       // Apellido del empleado
    "edad": <Integer>           // Edad del empleado
}
