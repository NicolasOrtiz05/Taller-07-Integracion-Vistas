# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 7 - Taller-07-Integracion-Vistas

## 👥 Integrantes del equipo
- Edwin Alejandro Gutierrez Rodriguez edwingutro@unisabana.edu.co
- Samuel Espitia Cruz samuelescr@unisabana.edu.co
- Nicolas Stiven Ortiz Cortes nicolasorco@unisabana.edu.co
  
# 🧠 Descripción general del trabajo

El objetivo del taller fue integrar múltiples vistas arquitectónicas —proceso, negocio, aplicaciones, infraestructura y seguridad— para modelar el funcionamiento del proceso de **Adquisiciones Institucionales** en la Universidad de La Sabana.  
El ejercicio buscó representar de forma integrada cómo interactúan las unidades solicitantes, la jefatura de adquisiciones, los proveedores, los sistemas corporativos (ERP, portal de servicios, INSPEKTOR, SharePoint), y la infraestructura tecnológica que sostiene todo el proceso.

El trabajo se desarrolló partiendo de los flujos actuales del proceso, identificando los actores involucrados y consolidando los diagramas en un solo modelo visual coherente.

---

# 🔧 Proceso de desarrollo

El equipo inició revisando el proceso administrativo modelado en BPMN, lo cual permitió identificar las tareas principales del ciclo de adquisiciones: solicitud, aprobación, validación, cotización y entrega.

A partir de este proceso se tomaron las siguientes decisiones:

- **Modelar primero la vista de negocio**, basada en actividades y actores.
- Integrar gradualmente la **vista de aplicaciones**, destacando:
  - Portal de Servicios  
  - Siga Financiero ERP  
  - Gestor de Proveedores  
  - INSPEKTOR para validación DataIFLT  
  - Excel/SharePoint como soporte documental  
- Posteriormente agregar la **vista de infraestructura**, identificando:
  - Oracle Cloud como plataforma principal del ERP  
  - Firewall institucional  
  - Red del campus  
  - Active Directory  
- Se construyó el diagrama integrado en **Draw.io**, ajustando colores, conexiones y posiciones para mantener claridad visual.

El desarrollo fue iterativo, ajustando los componentes conforme se validaba su rol dentro del proceso.

---

# 🧩 Análisis del modelo propuesto

### ✔ Estructura del modelo

El diagrama se organiza en secciones que representan:

1. El flujo del proceso (BPMN).  
2. La interacción entre unidades administrativas (solicitante, decano, adquisiciones).  
3. Los sistemas que soportan el proceso (ERP, portal, INSPEKTOR, SharePoint).  
4. La infraestructura tecnológica (Oracle Cloud, red corporativa, firewall).  

### ✔ Representación de necesidades del cliente

El modelo refleja adecuadamente la operación del área de Adquisiciones, incluyendo:

- Recepción centralizada de solicitudes desde el **Portal de Servicios**.  
- Validación y control financiero en **Siga ERP**.  
- Validación de proveedores mediante **INSPEKTOR**.  
- Comunicación entre unidades solicitantes, adquisiciones y proveedores.  
- Infraestructura segura para acceso y procesamiento mediante firewall y herramientas institucionales.

---

# 📈 Diagrama final entregado

![Diagrama vistas](viatas-integrada.png)

---

# 📋 Tabla de actores, entidades o componentes

| Nombre del elemento        | Tipo             | Descripción                                                 | Responsable |
|----------------------------|------------------|-------------------------------------------------------------|-------------|
| Unidad Solicitante         | Actor            | Genera la solicitud de bienes o servicios                   | Área usuaria |
| Decano / Director de Unidad | Actor           | Revisa, aprueba o condiciona las solicitudes                | Dirección académica |
| Jefatura de Adquisiciones  | Actor            | Gestiona proveedores, validaciones y cotizaciones           | Adquisiciones |
| Proveedores                | Actor            | Envían cotizaciones y entregan bienes o servicios           | Externo |
| Portal de Servicios        | Aplicación       | Módulo de recepción y radicación de solicitudes             | TI |
| Siga Financiero ERP        | Aplicación       | Control presupuestal y financiero de adquisiciones          | Área financiera |
| Gestor de Proveedores      | Aplicación       | Gestión documental y validación preliminar de proveedores   | Adquisiciones |
| INSPEKTOR / DataIFLT       | Servicio externo | Validación de listas restrictivas y cumplimiento            | Cumplimiento |
| Excel / SharePoint         | Repositorio      | Archivo local de solicitudes, reportes y validaciones       | Usuarios internos |
| Firewall institucional     | Infraestructura   | Protege la red corporativa y regula tráfico con Internet    | TI |
| Red del Campus             | Infraestructura   | Conectividad institucional para los sistemas internos       | TI |
| Active Directory           | Infraestructura   | Autenticación centralizada del personal universitario       | TI |
| Oracle Cloud               | Infraestructura   | Plataforma donde residen ERP y portal institucional         | TI |

---



## 🔍 Investigación complementaria
### Tema investigado:
(Ej: Buenas prácticas BPMN, comparación TOGAF vs C4, principios de seguridad STRIDE, etc.)

### Resumen:
Describa en 2–3 párrafos lo investigado, citando fuentes cuando sea necesario. Incluya cómo se relaciona con el taller.

## 📚 Referencias
- [1] Apellido, Nombre. *Título*. Año. URL o DOI.
- [2] Fuente oficial BPMN: https://www.omg.org/spec/BPMN/

---

_Este documento hace parte de la entrega del taller 7 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
