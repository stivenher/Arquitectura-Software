# Fase 4. Análisis Arquitectónico

## Importancia de utilizar múltiples vistas arquitectónicas

Durante el diseño de una solución de software resulta insuficiente representar todo el sistema mediante un único diagrama, ya que cada perspectiva permite analizar aspectos distintos de su funcionamiento. El uso de múltiples vistas arquitectónicas facilita comprender tanto la estructura como el comportamiento del sistema, permitiendo que desarrolladores, analistas y demás interesados interpreten la solución desde el punto de vista que más se ajuste a sus necesidades.

En el caso del Sistema Inteligente de Movilidad Urbana, las diferentes vistas ayudan a representar la interacción de los usuarios con la plataforma, la organización de los módulos internos, el flujo de ejecución de los procesos y la relación entre los principales componentes del ecosistema. Gracias a ello, el diseño resulta más claro y sencillo de comprender antes de iniciar la implementación.

---

## Descripción de las vistas arquitectónicas

### Vista de Casos de Uso

Esta vista identifica los servicios que ofrece el sistema y muestra la relación existente entre los actores y las funcionalidades disponibles. Su principal objetivo es representar los requerimientos funcionales desde la perspectiva del usuario y de los sistemas externos que interactúan con la plataforma.

### Vista Lógica

La vista lógica describe la estructura interna de la aplicación, organizando el software en módulos o componentes independientes. Esta representación facilita comprender cómo se distribuyen las responsabilidades dentro del sistema y cómo colaboran entre sí para cumplir los procesos definidos.

### Vista de Procesos

La vista de procesos refleja la secuencia de actividades que se ejecutan cuando ocurre una determinada operación. A través del diagrama de secuencia es posible observar el intercambio de mensajes entre los diferentes componentes hasta completar una solicitud realizada por el usuario.

### Vista Conceptual

La vista conceptual proporciona una visión global del sistema. En ella se representan los elementos principales de la solución, como usuarios, sensores, servicios externos y el sistema central, permitiendo comprender de forma sencilla la relación existente entre todos ellos.

---

## Relación entre las diferentes vistas

Aunque cada vista analiza el sistema desde una perspectiva distinta, todas se complementan para ofrecer una representación completa de la arquitectura.

La vista de casos de uso permite identificar las funcionalidades principales y los actores involucrados. Posteriormente, la vista lógica muestra cómo dichas funcionalidades son implementadas mediante componentes internos. La vista de procesos explica la comunicación que existe entre estos componentes durante la ejecución de una tarea específica, mientras que la vista conceptual ofrece una representación general de todo el entorno donde opera el sistema.

La integración de estas perspectivas facilita el análisis, el desarrollo y el mantenimiento de la solución, ya que permite comprender tanto el comportamiento como la estructura de la arquitectura propuesta.

---

## Vista con mayor nivel de complejidad

Entre las vistas desarrolladas, la de procesos representó el mayor desafío. Para construirla fue necesario analizar cuidadosamente el orden en que intervienen los diferentes componentes y definir correctamente la secuencia de mensajes intercambiados entre ellos.

Sin embargo, este ejercicio permitió comprender con mayor profundidad la forma en que los módulos colaboran para responder a las solicitudes de los usuarios, fortaleciendo el entendimiento del comportamiento interno del sistema.

---

# Conclusiones

- El desarrollo de este proyecto permitió comprender que la arquitectura de software constituye una etapa fundamental dentro del diseño de cualquier sistema, ya que facilita la organización de sus componentes y establece una base sólida para su construcción y evolución.

- La elaboración de las diferentes vistas arquitectónicas demostró que cada una aporta información específica sobre el sistema. En conjunto ofrecen una comprensión mucho más completa que la obtenida mediante un único diagrama.

- La definición de los requisitos funcionales y no funcionales permitió establecer las características que debe cumplir la solución para garantizar aspectos esenciales como el rendimiento, la seguridad, la disponibilidad y la escalabilidad.

- El Sistema Inteligente de Movilidad Urbana representa una alternativa tecnológica que puede contribuir a optimizar el tránsito en las ciudades mediante el procesamiento de información en tiempo real, el análisis de datos provenientes de sensores y la automatización de procesos relacionados con la movilidad.

- Finalmente, la utilización de herramientas de modelado y documentación, como Mermaid y GitHub, facilita la representación de la arquitectura del sistema y mejora la organización de la información durante el desarrollo del proyecto.