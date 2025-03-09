
**Documentación Técnica**
**1. Desarrollo del Proyecto**
 Esta sección debe incluir los aspectos técnicos del sistema para que otros desarrolladores, ingenieros o equipos de mantenimiento puedan entenderlo y replicarlo.

**1.1 Introducción y Alcance.**
Objetivo del Proyecto.
El Timbre Digital Inteligente es un dispositivo IoT que permite una comunicación bidireccional en tiempo real entre el usuario y los visitantes. Integra videollamadas, reconocimiento facial, detección de movimiento y alertas de seguridad para mejorar el control del acceso al hogar.
**Alcance.**

El sistema ofrece las siguientes funcionalidades:
Comunicación en tiempo real mediante llamadas, audio y video.
Acceso remoto desde una aplicación móvil.
Acceso y visibilidad remota.
Registro de visitantes y eventos de seguridad en la nube.

**No cubre:**
Integración con cerraduras electrónicas (opcional en futuras versiones).
Control sobre redes WiFi de terceros.
Asistente de voz por IA.

**Público Objetivo**
El sistema está dirigido a:
Usuarios residenciales que buscan mejorar la seguridad del hogar.
Empresas o negocios que necesitan un control de acceso.
Personas que desean monitorear y gestionar visitantes de forma remota.

**Metodología Utilizada.**
Se sigue un enfoque basado en Desarrollo Ágil (Scrum), con iteraciones quincenales para pruebas y mejoras continuas.

**Tecnologías Utilizadas**
**Hardware:**
 ESP32 con cámara
Micrófono integrado
Sensores de movimiento PIR
Módulo WiFi/Bluetooth

**Software:**
Frontend: React Native y Angular (para aplicación móvil)
Backend: Node.js con Express.js
Base de datos: MongoDB 
Protocolos de comunicación:
JS WEB TOKENS
WebSockets para videollamadas y notificaciones
HTTPS para la seguridad en la transmisión de datos


**1.2 Arquitectura del Sistema.**
Aquí se explica cómo están conectados los distintos componentes del sistema.
•Diagrama de componentes del sistema.
•Botón ioT = API = Notificación = FrontEnd(Web/Móvil)
Bajo API va mongoATLAS.

**Diagrama de arquitectura**
•Sensores/Actuadores: Micrófono, cámara, Buzzer, Infrarrojo.
•Dispositivo IoT: Microcontrolador, ESP32-CAM, módulo de comunicación.
•Servidores en la Nube (Almacenamiento y Procesador): MongoDB, Mysql(Almacenamiento eventos de timbre, registros, usuario).
•API REST: Node.js, peticiones entre dispositivos IoT y App Móvil.
•Dashboard: monitoreo y control de interfaz accesible de navegador para visualizar registro, configuraciones de alertas y gestión de usuario
•App de Usuario: Interacción con usuario, notificaciones cuando alguien toca el timbre, acceso video /audio y control de puerta.

**1.3 Requerimientos funcionales y no funcionales.**


