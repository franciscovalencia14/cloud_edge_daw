# Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

## 🅰️ Tarea A — Niveles de cloud (IaaS/PaaS/SaaS)

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

---

## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)

### Diagrama (Mermaid)
```mermaid
graph TD
    Frontend[Usuario / Frontend] --> API[API / Servidor de Aplicación]
    API --> Logic[Procesamiento / Lógica de Negocio]
    Logic --> DB[BBDD / Storage Cloud]
    Logic --> External[Servicios externos / Cloud APIs]
    DB --> Backup[Backup / Almacenamiento seguro]
