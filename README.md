# # Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

## 🅰️ Tarea A — Niveles de cloud (IaaS/PaaS/SaaS)
Crea una tabla con 10 servicios reales. Incluye enlace oficial y justifica responsabilidades.

| Servicio | Proveedor | Nivel (IaaS/PaaS/SaaS) | Enlace oficial | ¿Qué gestiona el proveedor? | ¿Qué gestiona el equipo/usuario? |
|---------|----------|-------------------------|----------------|-----------------------------|----------------------------------|
| Amazon EC2 | AWS | IaaS | [AWS EC2](https://aws.amazon.com/ec2/) | Hardware, red, virtualización, seguridad física | Sistema operativo, aplicaciones, datos |
| Google Compute Engine | Google Cloud | IaaS | [GCE](https://cloud.google.com/compute) | Hardware, red, virtualización | SO, apps, configuración |
| Microsoft Azure Virtual Machines | Microsoft | IaaS | [Azure VM](https://azure.microsoft.com/en-us/services/virtual-machines/) | Infraestructura física y virtual | SO, apps, seguridad a nivel software |
| Heroku | Salesforce | PaaS | [Heroku](https://www.heroku.com/) | Servidores, runtime, networking | Código de aplicación, dependencias |
| Google App Engine | Google Cloud | PaaS | [GAE](https://cloud.google.com/appengine) | Infraestructura, runtime, escalabilidad automática | Aplicación, configuración |
| Microsoft Azure App Service | Microsoft | PaaS | [Azure App Service](https://azure.microsoft.com/en-us/services/app-service/) | Servidores, runtime, balanceo de carga | Código, entorno de ejecución |
| Gmail | Google | SaaS | [Gmail](https://mail.google.com/) | Infraestructura, software, seguridad, mantenimiento | Uso de la cuenta, configuración de preferencias |
| Microsoft 365 | Microsoft | SaaS | [Microsoft 365](https://www.microsoft.com/microsoft-365) | Aplicaciones, almacenamiento, actualizaciones | Archivos, usuarios, configuración |
| Dropbox | Dropbox Inc. | SaaS | [Dropbox](https://www.dropbox.com/) | Infraestructura, almacenamiento, seguridad | Archivos, organización de carpetas |
| Slack | Salesforce | SaaS | [Slack](https://slack.com/) | Aplicación, servidores, seguridad, mantenimiento | Mensajes, canales, integraciones |

## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)
Incluye un diagrama (ASCII/Mermaid/imagen) y una explicación breve.

### Diagrama
flowchart LR
    U[Usuario / Navegador] --> F[Frontend Web<br>(WordPress.com)]
    F --> A[API / Backend Cloud<br>(Funciones + Servicios)]
    A --> D[(Base de Datos<br>Cloud)]
    A --> S[(Almacenamiento<br>de Archivos)]
    D --> A
    S --> A
    A --> F


### Explicación (8–12 líneas)
El usuario accede a la aplicación desde su navegador, interactuando con el frontend alojado en la nube (por ejemplo, WordPress.com).
El frontend envía solicitudes HTTP a una API alojada en la infraestructura cloud.
La API gestiona la lógica de negocio y valida las peticiones recibidas.
Cuando se requiere información persistente, la API consulta o actualiza la base de datos cloud.
Los archivos estáticos o multimedia se almacenan en servicios de almacenamiento en la nube.
La infraestructura cloud permite escalado automático según la carga de usuarios.
Los servicios cloud garantizan alta disponibilidad y tolerancia a fallos.
Finalmente, la API devuelve la respuesta procesada al frontend, que la muestra al usuario.
### Mapeo de funciones cloud a componentes (mínimo 3)
Procesamiento → Backend cloud que ejecuta la lógica de negocio (servicios gestionados / serverless).
Ejecución → Plataforma cloud que ejecuta la API y el frontend (entornos gestionados).
Almacenamiento → Base de datos cloud y almacenamiento de objetos para archivos.
Intercambio → APIs REST sobre HTTP/HTTPS para la comunicación entre frontend y backend.

## 📚 Fuentes (enlaces oficiales)
https://cloud.google.com/learn/what-is-cloud-computing
https://aws.amazon.com/what-is-cloud-computing/
https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/
https://wordpress.com/support/
