
# Fase 1. Especificación de Requisitos

## 1. Identificación de los módulos funcionales

Con el fin de facilitar el desarrollo, mantenimiento y escalabilidad del Sistema Inteligente de Movilidad Urbana, la solución se organiza en diferentes módulos funcionales. Cada uno cumple una responsabilidad específica dentro de la arquitectura, permitiendo una distribución clara de las tareas y una mejor integración entre los componentes.

### 1.1 Módulo de Gestión del Tráfico

Este módulo tiene la responsabilidad de supervisar las condiciones del tránsito en tiempo real. Para ello procesa la información recibida desde los sensores urbanos, identifica cambios en el flujo vehicular y proporciona datos actualizados sobre el estado de las vías.

### 1.2 Módulo de Gestión de Semáforos

Su función consiste en administrar el funcionamiento de los semáforos inteligentes. A partir de la información del tráfico, ajusta automáticamente los tiempos de cambio para mejorar la movilidad y reducir la congestión.

### 1.3 Módulo de Gestión de Rutas

Se encarga de calcular el recorrido más conveniente para cada usuario considerando variables como la distancia, el nivel de tráfico, los accidentes y las restricciones existentes en las vías.

### 1.4 Módulo de Gestión de Sensores

Este componente administra la información proveniente de cámaras, dispositivos GPS, sensores de velocidad y otros equipos instalados en la infraestructura vial. Además, verifica la disponibilidad y el correcto funcionamiento de dichos dispositivos.

### 1.5 Módulo de Gestión de Alertas

Su objetivo es generar y distribuir notificaciones relacionadas con accidentes, congestiones, cierres de vías o cualquier evento que pueda afectar la movilidad de los usuarios.

### 1.6 Módulo de Aplicación Móvil

Proporciona la interfaz mediante la cual los ciudadanos interactúan con el sistema. Desde la aplicación es posible consultar rutas, visualizar el estado del tráfico y recibir alertas en tiempo real.

### 1.7 Módulo de Integración Externa

Permite el intercambio de información con plataformas externas como servicios de mapas, pronósticos climáticos, sistemas de transporte público y organismos de atención de emergencias.

### 1.8 Módulo de Administración

Está orientado a la gestión general del sistema. Desde este módulo los administradores pueden controlar usuarios, configurar parámetros, registrar dispositivos y supervisar el funcionamiento de toda la plataforma.

---

# 2. Requisitos Funcionales

Los requisitos funcionales describen las acciones que el sistema debe ejecutar para cumplir con los objetivos establecidos.

## Gestión del Tráfico

- **RF01.** Supervisar continuamente el estado del tráfico en las principales vías.
- **RF02.** Identificar automáticamente zonas con alta congestión.
- **RF03.** Calcular la velocidad promedio de circulación en cada sector.
- **RF04.** Mostrar información actualizada sobre el estado de las vías.
- **RF05.** Almacenar un historial de los datos relacionados con el tráfico.

## Gestión de Semáforos

- **RF06.** Administrar los semáforos inteligentes desde el centro de control.
- **RF07.** Ajustar automáticamente los ciclos de los semáforos según el flujo vehicular.
- **RF08.** Priorizar el paso de vehículos de emergencia cuando sea necesario.
- **RF09.** Detectar fallas en los dispositivos de señalización.
- **RF10.** Permitir la intervención manual por parte de los operadores autorizados.

## Gestión de Rutas

- **RF11.** Calcular la ruta más conveniente entre un origen y un destino.
- **RF12.** Considerar el estado del tráfico durante el cálculo del recorrido.
- **RF13.** Recalcular la ruta cuando ocurra un incidente.
- **RF14.** Presentar alternativas de desplazamiento.
- **RF15.** Informar el tiempo estimado de llegada.

## Gestión de Sensores

- **RF16.** Recibir información enviada por los sensores urbanos.
- **RF17.** Validar la integridad de los datos recibidos.
- **RF18.** Detectar dispositivos que presenten fallas.
- **RF19.** Registrar la ubicación de cada sensor.
- **RF20.** Almacenar temporalmente la información para su procesamiento.

## Gestión de Alertas

- **RF21.** Emitir alertas cuando exista congestión vehicular.
- **RF22.** Informar accidentes o incidentes registrados.
- **RF23.** Notificar cierres y restricciones de las vías.
- **RF24.** Enviar las alertas a la aplicación móvil.
- **RF25.** Informar al centro de control sobre eventos relevantes.
- **RF26.** Clasificar las alertas según su nivel de prioridad.

## Aplicación Móvil

- **RF27.** Permitir al usuario indicar el punto de origen y destino.
- **RF28.** Mostrar el recorrido recomendado.
- **RF29.** Presentar el estado del tráfico en tiempo real.
- **RF30.** Recibir notificaciones relacionadas con la movilidad.
- **RF31.** Permitir que los usuarios reporten incidentes.

## Integración Externa

- **RF32.** Conectarse con plataformas de mapas y geolocalización.
- **RF33.** Consultar información meteorológica.
- **RF34.** Obtener datos del transporte público.
- **RF35.** Compartir información con organismos de emergencia.
- **RF36.** Gestionar errores cuando un servicio externo no esté disponible.

## Administración del Sistema

- **RF37.** Gestionar usuarios registrados.
- **RF38.** Administrar roles y permisos.
- **RF39.** Registrar nuevos sensores y dispositivos.
- **RF40.** Configurar parámetros generales del sistema.
- **RF41.** Registrar las acciones realizadas por los administradores.
- **RF42.** Consultar información histórica mediante reportes.

---

# 3. Requisitos No Funcionales

Además de las funcionalidades principales, el sistema debe cumplir una serie de características de calidad que garanticen un funcionamiento confiable.

## Disponibilidad

- **RNF01.** El sistema deberá mantener una disponibilidad mínima del 99,9 %.

## Rendimiento

- **RNF02.** El tiempo de respuesta para consultar rutas no debe superar los dos segundos.
- **RNF03.** Los datos recibidos desde los sensores deberán procesarse en un máximo de cinco segundos.

## Escalabilidad

- **RNF04.** La arquitectura deberá permitir incorporar nuevos módulos y servicios sin afectar el funcionamiento existente.
- **RNF05.** El sistema deberá soportar el crecimiento de usuarios y dispositivos conectados.

## Seguridad

- **RNF06.** Toda la comunicación deberá realizarse mediante mecanismos seguros.
- **RNF07.** El acceso estará restringido únicamente a usuarios autorizados.
- **RNF08.** La información almacenada deberá protegerse frente a accesos no autorizados.

## Tolerancia a Fallos

- **RNF09.** El sistema deberá continuar operando ante la falla de alguno de sus componentes.
- **RNF10.** Se deberán implementar mecanismos de respaldo y recuperación de la información.

## Interoperabilidad

- **RNF11.** La plataforma deberá integrarse correctamente con servicios externos.

## Mantenibilidad

- **RNF12.** La arquitectura deberá facilitar futuras actualizaciones y tareas de mantenimiento.

## Usabilidad

- **RNF13.** La interfaz deberá ser intuitiva y sencilla para cualquier usuario.
- **RNF14.** Las notificaciones deberán presentarse de forma clara y comprensible.

## Auditabilidad

- **RNF15.** El sistema deberá registrar los eventos importantes para facilitar auditorías y revisiones posteriores.

---

# 4. Priorización de Requisitos

## Alta Prioridad

- Monitoreo del tráfico en tiempo real.
- Procesamiento de la información proveniente de sensores.
- Detección de incidentes y congestiones.
- Cálculo de rutas óptimas.
- Gestión de semáforos inteligentes.
- Generación de alertas.
- Garantizar la seguridad y disponibilidad del sistema.

## Prioridad Media

- Integración con servicios climáticos.
- Consulta de información histórica.
- Elaboración de reportes administrativos.
- Integración con sistemas de transporte público.
- Configuración de notificaciones personalizadas.

## Baja Prioridad

- Funciones avanzadas de personalización.
- Análisis estadísticos especializados.
- Integración futura con nuevas plataformas tecnológicas.

---

# 5. Criterios de Aceptación

El sistema será considerado funcional cuando sea capaz de:

- Procesar correctamente la información enviada por los sensores.
- Mostrar el estado del tráfico en tiempo real.
- Detectar incidentes y niveles de congestión.
- Calcular rutas eficientes entre dos ubicaciones.
- Actualizar automáticamente los recorridos cuando cambien las condiciones del tráfico.
- Enviar alertas tanto a los usuarios como al centro de control.
- Administrar correctamente los semáforos inteligentes.
- Cumplir con los niveles definidos de seguridad, disponibilidad y rendimiento.
