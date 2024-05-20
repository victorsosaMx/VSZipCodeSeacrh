# VSZipCodeSearch

VSZipCodeSearch es un proyecto para buscar información detallada de un código postal en México utilizando la API de Copomex. Este proyecto proporciona un formulario donde los usuarios pueden ingresar un código postal y recibir información sobre asentamientos, tipo de asentamiento, municipio, estado, ciudad y país.

## Características

- **Búsqueda de Código Postal:** Permite a los usuarios ingresar un código postal y obtener información relacionada.
- **Selección de Asentamiento:** Muestra una lista de asentamientos asociados al código postal ingresado.
- **Información Detallada:** Proporciona detalles sobre el tipo de asentamiento, municipio, estado, ciudad y país.
- **Interfaz Amigable:** Utiliza Bootstrap para una apariencia y experiencia de usuario mejoradas.

## Uso

1. **Ingreso del Código Postal:** El usuario ingresa un código postal en el campo correspondiente.
2. **Selección del Asentamiento:** Aparece una lista desplegable con los asentamientos correspondientes al código postal. Si el usuario selecciona "Otro", puede ingresar manualmente el asentamiento.
3. **Visualización de Información:** La información detallada sobre el tipo de asentamiento, municipio, estado, ciudad y país se muestra automáticamente en los campos correspondientes.

## Instrucciones

### Requisitos Previos

- **API de Copomex:** Necesita un token válido de la API de Copomex.
- Puede obtenerlo registrándose en [Copomex](https://www.copomex.com).

### Instalación

1. **Clonar el Repositorio:**
   - Navegar al directorio del proyecto y abrir el archivo `VSZipCodeSearch.html` en su navegador web.

### Configuración

- **Token de API:**
  - Reemplace el valor de `const token = 'pruebas';` en el archivo `VSZipCodeSearch.html` con su propio token obtenido de Copomex.

### Documentación del Código

- **lookupCP(event):** Función que busca información del código postal ingresado y actualiza la lista de asentamientos.
- **updateFields(cp, validResponses, selectedAsentamiento):** Actualiza los campos del formulario con la información del asentamiento seleccionado.
- **clearFields():** Limpia los campos del formulario cuando no hay resultados válidos.

### Uso del Proyecto

1. **Ejecutar el Proyecto:** Abra `VSZipCodeSearch.html` en su navegador.
2. **Ingresar Código Postal:** Ingrese un código postal válido en el campo correspondiente.
3. **Seleccionar Asentamiento:** Seleccione un asentamiento de la lista o ingréselo manualmente si selecciona "Otro".
4. **Ver Información:** Los detalles del asentamiento, municipio, estado, ciudad y país se mostrarán automáticamente.

### Documentación del Código

- **lookupCP(event):** Función que busca información del código postal ingresado y actualiza la lista de asentamientos.
  - **Parámetro:** `event` - El evento que desencadena la búsqueda.
  - **Descripción:** Esta función toma el valor ingresado en el campo del código postal, valida que tenga una longitud de 5 caracteres, y realiza una solicitud a la API de Copomex. Si la respuesta es válida, llena el campo de asentamientos y maneja la selección del usuario.

- **updateFields(cp, validResponses, selectedAsentamiento):** Actualiza los campos del formulario con la información del asentamiento seleccionado.
  - **Parámetros:**
    - `cp` - El código postal ingresado.
    - `validResponses` - Las respuestas válidas obtenidas de la API.
    - `selectedAsentamiento` - El asentamiento seleccionado por el usuario.
  - **Descripción:** Esta función toma los datos del asentamiento seleccionado y actualiza los campos de tipo de asentamiento, municipio, estado, ciudad y país con la información correspondiente.

- **clearFields():** Limpia los campos del formulario cuando no hay resultados válidos.
  - **Descripción:** Esta función resetea todos los campos del formulario a sus valores iniciales y desactiva el campo de entrada de asentamiento adicional.

### Uso del Proyecto

1. **Ejecutar el Proyecto:** Abra `VSZipCodeSearch.html` en su navegador.
2. **Ingresar Código Postal:** Ingrese un código postal válido en el campo correspondiente.
3. **Seleccionar Asentamiento:** Seleccione un asentamiento de la lista o ingréselo manualmente si selecciona "Otro".
4. **Ver Información:** Los detalles del asentamiento, municipio, estado, ciudad y país se mostrarán automáticamente.


## Licencia

Este proyecto está licenciado bajo la [MIT License](LICENSE).
