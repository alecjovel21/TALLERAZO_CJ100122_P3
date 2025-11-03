🔧 Tallerazo Móvil: Aplicación de Gestión de Citas y Diagnóstico (SPA Híbrida)
Tallerazo Móvil es un prototipo funcional de una aplicación web de página única (SPA) diseñada para talleres de mecánica. Su objetivo es mejorar la experiencia del cliente (UX) al permitir el autodiagnóstico, la gestión de citas y el contacto con sucursales de forma rápida y segura.

El proyecto está construido bajo una arquitectura web ligera, ideal para ser empaquetada como una aplicación móvil (APK) mediante tecnologías híbridas (Capacitor/Cordova).

🚀 Características Principales
Autenticación Segura (OTP Real): El acceso se realiza mediante un código de un solo uso (OTP) enviado por correo electrónico a través de EmailJS, garantizando la seguridad del cliente sin contraseñas.

Diagnóstico Rápido: Los usuarios pueden ingresar síntomas de fallas en su vehículo para recibir una sugerencia de servicio automatizada (lógica simple en el cliente).

Agendamiento de Citas: Módulo para registrar citas con fecha y taller preferido (usando localStorage para persistencia simulada).

Ubicación de Sucursales: Muestra las distintas ubicaciones de los talleres en un mapa interactivo (usando la librería Leaflet).

Asistente Virtual (Opcional): Integración con Dialogflow Messenger para soporte y respuestas automatizadas.

Análisis Económico (Integración Adicional): Incluye un panel para calcular y visualizar costos de inversión (CAPEX) y costos operativos (OPEX) relacionados con la contratación de personal o proyectos.
Componente,Tecnología / Servicio,Rol
Frontend/Core,"HTML5, CSS3 (Estilos Oscuros/Modernos), JavaScript ES6+",Interfaz de usuario y lógica de navegación (Router SPA).
Autenticación (OTP),EmailJS,Servicio Serverless para el envío de códigos de seguridad por correo electrónico.
Seguridad,Hashing SHA-256 (Client-side),Se utiliza para almacenar el código OTP de forma segura antes de la verificación.
Geolocalización,Leaflet.js / OpenStreetMap,Renderizado del mapa de sucursales.
Datos / Estado,"JavaScript Objects, sessionStorage, localStorage",Base de datos simulada y gestión de la sesión y el historial.
