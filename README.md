U4S8 — Jesús Francisco Madrid Rodríguez

Proyecto Integrador: Aplicación web full-stack desarrollada como entrega final para el curso de APLICAWEB.

🚀 Demo en vivo

Visita la aplicación en producción aquí

(Nota: La aplicación está alojada en el plan gratuito de Render, por lo que el primer inicio puede tardar unos 50 segundos en cargar).

💡 Qué hace este proyecto

Este proyecto es un sistema web dinámico diseñado para la gestión de [TU TEMÁTICA AQUÍ, ej: servicios de consultoría / inventario de refacciones]. Permite a los usuarios registrados mantener un catálogo personalizado y seguro de sus registros.

Funcionalidades principales:

Gestión Completa (CRUD): Creación, lectura, actualización y eliminación de registros mediante ModelForms.

Navegación Intuitiva: Implementación de paginación para manejar grandes volúmenes de datos y un sistema de búsqueda en tiempo real.

Interfaz Responsiva: Diseño pulido y moderno estructurado enteramente con Tailwind CSS.

🛠️ Stack Técnico

Backend: Python 3, Django 5.1

Base de Datos: MySQL (alojado en la nube a través de Aiven)

Frontend: HTML5, Tailwind CSS

Despliegue (Deployment): Render (Web Service), Gunicorn, Whitenoise para archivos estáticos.

🔒 Seguridad y Aislamiento de Datos

Una de las prioridades técnicas del proyecto fue garantizar la privacidad de la información mediante el aislamiento por usuario.

¿Cómo se probó y garantizó esto?
Ejemplo de redacción: Para asegurar el aislamiento, el modelo de datos vincula cada registro directamente con el usuario activo mediante una Foreign Key. En las vistas de Django, las consultas (QuerySets) están filtradas explícitamente usando Servicio.objects.filter(usuario=request.user). De esta forma, si el "Usuario A" inicia sesión, es criptográficamente imposible que acceda, modifique o elimine por URL los datos pertenecientes al "Usuario B".
(Asegúrate de reescribir esto con la explicación que preparaste en la semana 6).

📚 Historial de Evolución (Unidades)

Este sistema fue construido de manera iterativa a lo largo de 8 semanas:

Unidad 1: Diseño de interfaz y maquetación de portafolio estático utilizando HTML5 y Tailwind CSS.

Unidad 2: Configuración del backend con Django, modelado de datos y conexión a base de datos MySQL en la nube.

Unidad 3: Desarrollo de lógica de negocio (CRUD completo), formularios dinámicos y sistema de autenticación de usuarios.

Unidad 4: Optimización de UI (búsqueda y paginación), auditoría de seguridad y despliegue final a producción.
