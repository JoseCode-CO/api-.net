Análisis del template para APIs de .NET
Cuando ejecutamos el comando dotnet new webapi el CLI de dotnet nos crea un proyecto listo para ejecutar y realizar pruebas, veamos que contiene este proyecto.



Untitled

Program.cs: Este archivo contiene la clase principal del programa, que es el punto de entrada para la aplicación. También contiene la lógica para iniciar el host de la aplicación y configurar el enrutamiento.
Controllers: Este directorio contiene los controladores de la API. Cada controlador es responsable de manejar una o varias solicitudes HTTP y devolver una respuesta.
appsettings.json: Este archivo contiene la configuración de la aplicación, como las opciones de conexión a la base de datos y las opciones de configuración personalizadas.
Properties: Este directorio contiene información sobre el proyecto, como la información de versión y la información de compilación.
Models: Este directorio contiene los modelos de datos utilizados por la API. Los modelos representan los datos que se manejan en la API, como los recursos que se están exponiendo.
Patron MVC
MVC es el acrónimo de Model-View-Controller, que es un patrón de arquitectura de software utilizado en desarrollo de aplicaciones. Se utiliza para separar la lógica de negocios, la lógica de presentación y la lógica de control en componentes independientes.

Modelo (Model): Es la capa de datos y lógica de negocios de la aplicación. Se encarga de representar los datos y las operaciones que se realizan sobre ellos.
Vista (View): Es la capa de presentación, se encarga de mostrar los datos al usuario y de recibir su entrada.
Controlador (Controller): Es la capa de control, que se encarga de coordinar las acciones entre el modelo y la vista. Recibe las solicitudes del usuario a través de la vista y actúa sobre el modelo para realizar las acciones necesarias.
Patron MXC en Nuestra API
En el template de proyecto *Web API en .NET*, la arquitectura MVC se aplica para separar la lógica de la aplicación en diferentes componentes sin hacer uso de las Vistas:

Modelos: Los modelos representan los datos que se manejan en la API, como los recursos que se están exponiendo. Estos modelos se almacenan en el directorio Models.
Controladores: Los controladores son la capa de control de la aplicación y se encargan de manejar las solicitudes HTTP y devolver las respuestas correspondientes. Los controladores se almacenan en el directorio Controllers.
Vistas: En una API de Web, no hay vistas en el sentido tradicional, ya que no se muestra una interfaz gráfica de usuario. En su lugar, los controladores devuelven datos en formato JSON o XML para su uso por parte de las aplicaciones cliente.
