# Fase 2. Análisis del Sistema
## Identificación de actores

- El Sistema Inteligente de Movilidad Urbana requiere la participación de diferentes actores que interactúan con la plataforma para intercambiar información, administrar el sistema o consultar datos relacionados con la movilidad. Cada uno desempeña una función específica que contribuye al correcto funcionamiento de la solución.

### Actor 1. Usuario (Conductor o peatón)

- Corresponde a las personas que utilizan la aplicación para consultar el estado del tráfico, obtener recomendaciones de rutas y recibir avisos sobre accidentes, congestiones u otras novedades que puedan afectar su desplazamiento.

### Actor 2. Red de sensores urbanos

- Está conformada por dispositivos como cámaras, sensores de velocidad, GPS y otros equipos instalados en distintos puntos de la ciudad. Estos dispositivos recopilan información en tiempo real y la transmiten al sistema para su procesamiento.

### Actor 3. Centro de monitoreo

Es la entidad responsable de supervisar el comportamiento del sistema, analizar las condiciones del tránsito, administrar los semáforos inteligentes y coordinar acciones cuando se presentan incidentes o emergencias.

### Actor 4. Aplicación móvil

- Es la plataforma mediante la cual los ciudadanos acceden a los servicios del sistema. A través de ella pueden consultar rutas, visualizar el estado de las vías y recibir información actualizada sobre la movilidad.

### Actor 5. Sistemas externos

- Incluye los diferentes servicios que complementan el funcionamiento de la plataforma, como aplicaciones de mapas, información meteorológica, sistemas de transporte público y entidades encargadas de la atención de emergencias.

## Funcionalidades principales

El Sistema Inteligente de Movilidad Urbana debe ofrecer las siguientes funcionalidades principales:

- Supervisar el tráfico en tiempo real.
- Recibir y analizar la información generada por los sensores urbanos.
- Identificar accidentes, congestiones y otros eventos que afecten la movilidad.
- Administrar el comportamiento de los semáforos inteligentes.
- Calcular las rutas más convenientes para los usuarios.
- Modificar las rutas sugeridas cuando cambien las condiciones del tránsito.
- Generar y enviar alertas sobre incidentes o cierres de vías.
- Compartir información con aplicaciones móviles y plataformas externas.
- Almacenar los datos recopilados para consultas y análisis posteriores.
- Facilitar al centro de monitoreo la administración general del sistema.
- Problemas que resuelve el sistema

## La implementación de este sistema pretende contribuir a la solución de diversos problemas relacionados con la movilidad urbana, entre ellos:

- Altos niveles de congestión en las principales vías.
- Aumento en los tiempos de desplazamiento.
- Falta de sincronización entre los semáforos.
- Demoras en la identificación de accidentes o incidentes.
- Información insuficiente para conductores y peatones.
- Lentitud en la respuesta frente a situaciones de emergencia.
- Aprovechamiento ineficiente de la infraestructura vial.
- Escasa integración entre los diferentes sistemas de movilidad.
- Restricciones del sistema

# Durante el diseño de la arquitectura es importante considerar una serie de restricciones que garanticen el correcto funcionamiento del sistema.

## Restricciones de tiempo real

- La información del estado del tráfico debe procesarse y actualizarse continuamente para que los usuarios dispongan de datos precisos y oportunos.

## Restricciones de disponibilidad

- La plataforma debe mantenerse operativa la mayor parte del tiempo, debido a que es un servicio de uso continuo para ciudadanos y entidades encargadas de la movilidad.

## Restricciones de rendimiento

- El sistema debe soportar un alto volumen de usuarios conectados y procesar simultáneamente la información generada por numerosos sensores sin afectar su desempeño.

## Restricciones de seguridad

-  Se deben implementar mecanismos que protejan la información almacenada y transmitida, evitando accesos no autorizados y garantizando la confidencialidad de los datos.

## Restricciones de escalabilidad

- La arquitectura debe permitir la incorporación de nuevos sensores, usuarios o servicios sin requerir modificaciones importantes en la plataforma.

## Restricciones de interoperabilidad

- El sistema debe ser compatible con otras soluciones tecnológicas, facilitando el intercambio de información con aplicaciones de mapas, sistemas de transporte y organismos de atención de emergencias.

## Restricciones de mantenimiento

- La solución debe diseñarse de manera que permita realizar actualizaciones, correcciones y mejoras sin afectar el funcionamiento de los demás componentes del sistema.