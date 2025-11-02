# 📘 Proyecto: Gestión de Clientes (Programación por Capas con ADO.NET)

## 🧩 Descripción General
Este proyecto académico consiste en el desarrollo de una aplicación en **C#** utilizando **ADO.NET** y una arquitectura **por capas**, cuyo propósito es **gestionar el registro de clientes** en una empresa.  
El trabajo se realiza de forma grupal y se basa en las indicaciones de la **Unidad Nº 3 - Semana 10** y la **Rúbrica de Evaluación para Tarea Académica**.

## 🧱 Estructura por Capas
El proyecto está implementado siguiendo el modelo clásico de **tres capas**:

1. **Capa de Entidades (Entities):**  
   Contiene las clases que representan los objetos del dominio.  
   - `Cliente`: define las propiedades del cliente (DNI, Nombre, Categoría, CréditoAsignado).

2. **Capa de Datos (Data / DAL):**  
   Encargada de la conexión con la base de datos y la ejecución de operaciones CRUD utilizando **ADO.NET**.

3. **Capa de Negocio (Business / BLL):**  
   Contiene la lógica de negocio, validaciones (como evitar DNIs duplicados) y reglas de asignación de créditos según la categoría.

4. **Capa de Presentación (UI):**  
   Interfaz gráfica (Windows Forms) que permite la interacción con el usuario, mostrando los datos en un **DataGridView**.

## 👥 Entidad Principal: Cliente

| Propiedad   | Descripción                                      | Tipo de Dato | Ejemplo             |
|--------------|--------------------------------------------------|---------------|----------------------|
| DNI          | Identificador único del cliente                 | string        | "74201984"           |
| Nombre       | Nombre completo del cliente                     | string        | "María López"        |
| Categoría    | Tipo de cliente (Nuevo, Ocasional, Frecuente)   | string        | "Frecuente"          |
| CréditoAsignado | Crédito otorgado según categoría              | decimal       | 5000                 |

### 💳 Créditos por Categoría
- **Nuevo:** S/. 1000  
- **Ocasional:** S/. 2500  
- **Frecuente:** S/. 5000  

---

## ⚙️ Funcionalidades Implementadas

✅ Registrar múltiples clientes  
- No se permite registrar dos clientes con el mismo DNI.  
- El crédito se asigna automáticamente según la categoría seleccionada.

✅ Mostrar todos los clientes registrados  
- Los datos se visualizan en un **DataGridView**.  

✅ Eliminar cliente  
- Se puede eliminar un cliente seleccionado previamente en la tabla.  

✅ Ordenar clientes por crédito  
- Permite ordenar de menor a mayor según el crédito asignado.  

✅ Mostrar clientes en orden de registro  
- Permite visualizar la lista en el orden en que fueron añadidos.  

✅ Uso de **Listas (List<T>)**  
- Se utilizan listas genéricas para almacenar y manipular los clientes.

## 🧠 Tecnologías Utilizadas
- **Lenguaje:** C#  
- **Framework:** .NET  
- **Acceso a Datos:** ADO.NET  
- **Interfaz Gráfica:** Windows Forms  
- **Estructura:** Programación por capas  
- **Control de versiones:** GitHub  

## 🧩 Referencias
- Laboratorio **Lab10 - Programación por capas (ADO.NET)**  
- Contenido de la **Unidad Nº 3 - Semana 10**  
