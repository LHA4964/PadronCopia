# Padrón de Habitantes

Este proyecto es una aplicación simple para gestionar un padrón de habitantes. La aplicación está estructurada en varios paquetes y clases que permiten agregar, mostrar y almacenar información sobre los habitantes.

## Guía de Instalación

Para instalar el proyecto, sigue estos pasos:

1. Clona el repositorio desde GitHub:

   ```bash
   git clone <enlace-de-tu-repositorio>

2. Navega al directorio del proyecto:

   cd Padron

3. Compila los archivos Java:

   javac -d bin src/**/*.java

4. Ejecuta la aplicación:

   java -cp bin aplicacion.Principal

## Estructura del Proyecto

El proyecto está dividido en los siguientes paquetes:

- **dominio**: Contiene las clases `Habitante` y `OficinaPadron`.
- **aplicacion**: Contiene la clase `Principal`.
- **presentacion**: Contiene la clase `InterfazUsuario`.

### Clases y Métodos

#### dominio.Habitante

Clase que representa un habitante.

- **Atributos:**
  - `String nombre`
  - `String apellido1`
  - `String apellido2`

- **Métodos:**
  - `Habitante(String nombre, String apellido1, String apellido2)`
  - `void setNombre(String nombre)`
  - `void setApellido1(String apellido1)`
  - `void setApellido2(String apellido2)`
  - `String getNombre()`
  - `String getApellido1()`
  - `String getApellido2()`
  - `String toString()`

#### dominio.OficinaPadron

Clase que representa una oficina de padrón de habitantes.

- **Atributos:**
  - `ArrayList<Habitante> habitantesPadron`

- **Métodos:**
  - `void annadir(Habitante habitante)`
  - `ArrayList<Habitante> getHabitantesPadron()`
  - `int calcularNumeroHabitantes()`
  - `String toString()`

#### aplicacion.Principal

Clase principal que inicia la aplicación.

- **Métodos:**
  - `main(String[] args)`

#### presentacion.InterfazUsuario

Clase que representa la interfaz de usuario.

- **Atributos:**
  - `OficinaPadron padron`
  - `Scanner sc`

- **Métodos:**
  - `boolean ejecutar(String[] instruccion)`
  - `String[] leerInstruccion()`
  - `void leerPadron()`
  - `void escribirPadron()`
  - `InterfazUsuario()`

## Ejecución

Para ejecutar la aplicación, compila y ejecuta la clase `Principal` en el paquete `aplicacion`.

## Uso

Las instrucciones disponibles en la interfaz de usuario son:

- `mostrar`: Muestra el padrón de habitantes.
- `ayuda`: Muestra las opciones disponibles.
- `añadir <nombre> <apellido1> <apellido2>`: Añade un nuevo habitante.
- `salir`: Guarda el padrón y finaliza la aplicación.

## Diagrama UML

El siguiente diagrama muestra la estructura del proyecto:

![Diagrama UML](path_to_uml_diagram.png)

## Requisitos

- Java SE Development Kit (JDK) 8 o superior.

## Autor

Este proyecto fue creado por Luis Holgado.

## Licencia

Este proyecto está bajo la Licencia Apache. Puedes ver el archivo [LICENSE](LICENSE) para más detalles.
