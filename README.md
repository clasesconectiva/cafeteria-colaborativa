# ☕ Cafetería Colaborativa

¡Bienvenidos al taller práctico de Java y trabajo colaborativo con Git y GitHub!

Este proyecto es una aplicación de consola en Java diseñada para gestionar pedidos de una cafetería. Fue estructurado para desarrollarse en **1 hora** aplicando flujo de trabajo colaborativo mediante ramas, *Pull Requests* y revisión de código[cite: 1, 2].

---

## 📐 Diagrama de Clases UML

Consulte la arquitectura del sistema para la implementación de los módulos:

![Diagrama de Clases UML](docs/diagrama_clases.png)

---

## 👥 Roles y Asignación de Módulos

| Módulo / Archivo | Estudiante / Usuario | Tarea Específica |
| :--- | :--- | :--- |
| **`Producto.java`** | *@usuario1* | Atributos, constructor y getters. |
| **`Menu.java` (Parte 1)** | *@usuario2* | Arreglo `Producto[]`, inicialización y `mostrarMenu()`. |
| **`Menu.java` (Parte 2)** | *@usuario3* | Método `buscarProducto(int id)`. |
| **`Pedido.java` (Parte 1)** | *@usuario4* | Estructura de arreglos, constructor y `agregarProducto()`. |
| **`Pedido.java` (Parte 2)** | *@usuario5* | Métodos `mostrarPedido()` y `calcularTotal()`. |
| **`GestorPedido.java` (Parte 1)** | *@usuario6* | Atributos, constructor y método `crearPedido()`. |
| **`GestorPedido.java` (Parte 2)** | *@usuario7* | Métodos `mostrarPedido()` y `mostrarTotal()`. |
| **`Main.java`** | *@usuario8* | Menú principal por consola y flujo `do/while`. |
| **Líder Técnico** | *@usuario9* | Gestión del repositorio, revisión de PRs e integración. |

> **Nota:** Todos los desarrolladores son responsables de validar las entradas de consola en sus respectivos métodos y realizar las pruebas unitarias de su módulo antes de enviar el Pull Request.

---

## 🛠️ Reglas de Desarrollo

1. **Uso exclusivo de arreglos primitivos (`[]`):** No se permite el uso de `ArrayList` ni otras colecciones de Java API.
2. **Sin persistencia ni librerías externas:** Aplicación puramente en memoria basada en Java SE estándar.
3. **Flujo de Git:**
   - Queda prohibido hacer `push` directo sobre la rama `main`.
   - Cada estudiante creará su rama siguiendo el patrón: `feature/nombre-modulo` (ej. `feature/producto`).
   - Todos los cambios deben integrarse a `main` a través de un **Pull Request (PR)** revisado por el Líder Técnico.

---

## 🚀 Compilación y Ejecución

Para compilar y ejecutar el proyecto localmente desde la terminal:

```bash
# Compilar clases desde la raíz del proyecto
javac src/*.java -d bin/

# Ejecutar la aplicación
java -cp bin Main
