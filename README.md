# 🧪 API Testing Portfolio - CRUD JSONPlaceholder

Colección de pruebas automatizadas de API REST desarrollada en **Postman**, aplicando buenas prácticas de QA Automation, parametrización de entornos, aserciones en JavaScript y validación de contratos mediante JSON Schema.

---

## 🛠️ Tecnologías y Herramientas Utilizadas
* **Postman:** Interfaz principal para diseño y ejecución de requests.
* **JavaScript:** Utilizado para la escritura de aserciones automatizadas en la pestaña de Tests.
* **JSON Schema:** Validación de contratos y tipos de datos en las respuestas.
* **JSONPlaceholder API:** Entorno público simulado para pruebas CRUD.

---

## 📂 Estructura de la Colección
La colección incluye los 4 métodos HTTP principales validados bajo un enfoque integral:

1. **GET - Consultar Post por ID:** Valida código `200 OK`, tiempo de respuesta y estructura del JSON.
2. **POST - Crear Nuevo Post:** Valida código `201 Created` y la correcta asignación de un nuevo ID por parte del servidor.
3. **PUT - Actualizar Post Completo:** Valida código `200 OK` y la modificación exitosa del recurso utilizando variables.
4. **DELETE - Eliminar Post por ID:** Valida código `200 OK` y respuesta vacía tras la baja del registro.

---

## ⚙️ Características Técnicas Implementadas
* **Variables de Entorno (`Environment`):** Parametrización de la `base_url` para facilitar la escalabilidad a otros ambientes (QA/Prod).
* **Variables de Colección:** Manejo dinámico del `postId` compartido entre peticiones.
* **Aserciones Automatizadas:** Verificación de códigos de estado, propiedades específicas y tiempos de respuesta.
* **Validación de Contrato (JSON Schema):** Asegura que la API devuelva estrictamente los tipos de datos esperados (`number`, `string`, etc.).
* **Collection Runner:** Ejecución automatizada en cadena de toda la suite con un resultado exitoso de **10/10 tests aprobados**.

---

## 🚀 Cómo utilizar este proyecto

1. Descargá o cloná este repositorio.
2. Abrí **Postman**, hacé clic en **Import** y seleccioná los archivos `.json` ubicados en este repositorio (tanto la colección como el entorno).
3. Seleccioná el entorno **`QA - JSONPlaceholder`** en la esquina superior derecha de Postman.
4. Abrí el **Collection Runner** en Postman y ejecutá la suite completa para ver todas las pruebas pasando en verde.
