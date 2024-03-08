# flutter_application_1

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

-------------------------------------------------Explicación-------------------------------------------------

* Los widgets son como los bloques de construcción fundamentales para crear la interfaz de usuario de una aplicación. 
* Mediante un widget se puede representar cada elemento visual, como botones, texto, imágenes, etc. 
* Los widgets en Flutter son inmutables, lo que significa que una vez que se crean, no se pueden modificar. Cuando se necesita realizar un cambio en la interfaz de usuario, Flutter crea un nuevo conjunto de widgets para reflejar esos cambios.

En este proyecto, utilizamos una variedad de widgets predefinidos de Flutter, como Scaffold, Row, SafeArea, NavigationRail, ElevatedButton, Text, Icon, ListView, Card, y ListTile para construir la interfaz de usuario de nuestra aplicación. Estos widgets se combinan y anidan de manera flexible para crear la estructura y el diseño deseados.

En cuanto a los estados: El estado en Flutter se refiere a cualquier dato que puede cambiar durante la vida útil de la aplicación y que afecta la representación visual de la interfaz de usuario. Dentro del proyecto se manejaron 2 tipos de
widgets, el primero es StatelessWidgets que es el widget sin estado, por medio de este widget la representación visual llega a ser inmutable y no cambia durante la vida útil de la aplicación. No almacenan ningún estado interno y se construyen únicamente a partir de los datos proporcionados en el momento de la creación. En este proyecto, el widget GeneratorPage es un ejemplo de un widget sin estado. Y el segundo es StatefulWidget que es el widget con estado, el cual por lo contrario del anterior la representación visual puede cambiar en respuesta a cambios en el estado de la aplicación. Están asociados a un objeto de estado que almacena los datos cambiantes. Cuando se actualiza el estado, Flutter reconstruye automáticamente los widgets necesarios para reflejar esos cambios. En este proyecto, el widget FavoritesPage es un ejemplo de un widget con estado.

En este proyecto, utilizamos el manejo de estado proporcionado por el paquete provider de Flutter para gestionar el estado de la aplicación de manera eficiente y escalable. El estado de la aplicación se almacena en la clase MyAppState, que extiende ChangeNotifier para notificar a los widgets cuando se producen cambios en el estado y deben volver a renderizarse.

MaterialApp: Define la aplicación Flutter con un tema material y configuraciones básicas.
ChangeNotifierProvider: Proporciona un objeto de estado compartido entre widgets hijos.
Scaffold: Implementa el diseño básico de una aplicación, incluyendo barras de aplicación y área de contenido.
NavigationRail: Ofrece una barra de navegación lateral para cambiar entre diferentes secciones de la aplicación.
ElevatedButton: Representa un botón con un diseño elevado y puede incluir un icono y un texto.
Text: Muestra texto en la interfaz de usuario con opciones de estilo, tamaño y color.
ListView: Muestra una lista de elementos en una vista de desplazamiento.
Card: Muestra un contenedor de tarjeta con sombra y esquinas redondeadas para presentar contenido organizado y visualmente atractivo.