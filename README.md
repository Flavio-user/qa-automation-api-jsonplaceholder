# API Testing Portfolio - CRUD JSONPlaceholder

## Descripción

Colección de pruebas automatizadas de API REST desarrollada en **Postman**, aplicando buenas prácticas de QA Automation, parametrización de entornos, aserciones en JavaScript y validación de contratos mediante **JSON Schema**.

## Tecnologías y Herramientas

- **Postman:** Interfaz principal para diseño y ejecución de requests.
- **JavaScript:** Utilizado para la escritura de aserciones automatizadas.
- **JSON Schema:** Validación de contratos y tipos de datos en las respuestas.
- **JSONPlaceholder API:** Entorno público simulado para pruebas CRUD.

## Cobertura de Pruebas y Buenas Prácticas

### Estructura de la Colección (`CRUD Posts - JSONPlaceholder`)
La colección incluye los 4 métodos HTTP principales validados bajo un enfoque integral:
1. **GET - Consultar Post por ID:** Valida código `200 OK`, tiempo de respuesta y estructura del JSON.
2. **POST - Crear Nuevo Post:** Valida código `201 Created` y la correcta asignación de un nuevo ID por parte del servidor.
3. **PUT - Actualizar Post Completo:** Valida código `200 OK` y la modificación exitosa del recurso utilizando variables.
4. **DELETE - Eliminar Post por ID:** Valida código `200 OK` y respuesta vacía tras la baja del registro.

### Buenas Prácticas y Características Implementadas
- **Variables de Entorno (`QA - JSONPlaceholder`):** Parametrización de `base_url` para facilitar la escalabilidad a otros ambientes (QA/Prod).
- **Variables de Colección:** Manejo dinámico del `postId` compartido entre peticiones.
- **Aserciones Automatizadas:** Verificación de códigos de estado, propiedades específicas y tiempos de respuesta.
- **Validación de Contrato (JSON Schema):** Asegura que la API devuelva estrictamente los tipos de datos esperados (`number`, `string`, etc.).
- **Collection Runner:** Ejecución automatizada en cadena de toda la suite con resultado de `10/10` tests aprobados.

## Ejemplo de Caso de Prueba

**Escenario:** Crear un nuevo post (`POST - Crear Nuevo Post`) y validar respuesta y contrato.

1. Seleccionar el entorno **`QA - JSONPlaceholder`** (`base_url`).
2. Enviar la petición `POST` hacia `{{base_url}}/posts` con el payload JSON correspondiente.
3. Ejecutar las aserciones automatizadas sobre el response.
4. **Resultado esperado:** El servidor responde con código `201 Created`, asigna un `id` al recurso creado y la estructura cumple con el JSON Schema esperado.

## Evidencia de Ejecución

### Ejecución completa de la colección (Collection Runner - 10/10 Passed)

<img width="1919" height="1032" alt="Captura de pantalla 2026-11-25 165219" src="https://github.com/user-attachments/assets/927260ac-f9d1-40da-b2aa-39700811d924" />

### Validación de contrato (JSON Schema) y aserciones en JavaScript

<img width="1919" height="1033" alt="Captura de pantalla 2026-11-25 165117" src="https://github.com/user-attachments/assets/0c824440-6e7d-45e4-990b-73d82d43f352" />

## Cómo Ejecutar el Proyecto

1. Descargue o clone este repositorio.
2. Abra Postman, haga click en **Import** y seleccione los archivos `.json` ubicados en este repositorio (tanto la colección como el entorno).
3. Seleccione el entorno **`QA - JSONPlaceholder`** en la esquina superior derecha de Postman.
4. Abra el **Collection Runner** en Postman y ejecute la suite completa para ver todas las pruebas pasando en verde.

## Autor

- **Flavio Matías Baldini** – QA Automation Tester
- **LinkedIn:** 
