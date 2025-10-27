
# Incidentes de seguridad
## Unidad 1: Principios generales de la ciberseguridad
**Ciclo de Especialización de FP en Ciberseguridad en Entornos de las Tecnologías de la Información**

![](assets/AnalisisRiesgos.png "Análisis de Riesgos")

---

# ANÁLISIS DE RIESGOS

## Índice

[**Introducción**](#0.-introducción)

[**Alcance del análisis**](#0.-introducción)

[**2. Identificación de los activos**](#2.-identificación-de-los-activos)

[**3. Amenazas que pueden afectar a los activos**](#3.-amenazas-que-pueden-afectar-a-los-activos)

[**4. Identificar vulnerabilidades y salvaguardas**](#4.-identificar-vulnerabilidades-y-salvaguardas)

[4.1. Identificación de salvaguardas (Medidas y controles de seguridad)](#4.1-identificación-de-salvaguardas-\(medidas-y-controles-de-seguridad\))

[4.2. Vulnerabilidades/Debilidades](#4.2-vulnerabilidades/debilidades)

[**5. Evaluación y cálculo del riesgo**](#5.-evaluación-y-cálculo-del-riesgo)

[**6. Medidas complementarias que permitan materializar la protección de los activos.**](#6.-medidas-complementarias-que-permitan-materializar-la-protección-de-los-activos.)

[**7. Conclusión**](#7.-conclusión)

[**8. Bibliografía/Webgrafía**](#8.-bibliografía/webgrafía)


---


## Introducción {#0.-introducción}

- Grupo e integrantes:Grupo 4, Jose Luis Godoy, Manuel Maye, Hugo Flores, Juan Pérez
- Presentación del ejercicio.
  Mejorar la seguridad de una empresa que se ha visto afectada por un ataque de ransomware, identificar las vulnerabilidades y reforzar al máximo todas las brechas de seguridad
- Contexto de la empresa: Somos una empresa que se dedica a mantener la integridad y la seguridad de la red, los sistemas y la información confidencial.
- Objetivo de la empresa: Aumentar y mejorar la seguridad de nuestra empresa
- Departamentos:
- Departamento de facturación y ventas
- Departamento de compras
- Departamento de comunicación y RRSS
- Departamento de TIC
- Departamento de RRHH
- Departamento de Delivery
- Departamento de Mantenimiento
- Departamento Legal
- Instalaciones/Sedes: 2 sedes: 1 edificio principal (sede principal) y 1 planta de otro edificio.
- Servicios TIC:
- Gestión de servicios de infraestructura tecnológica: servidores, redes, equipos informáticos y comunicaciones.
- Administración y mantenimiento de software y aplicaciones informáticas vitales para la empresa.
- Gestión de la seguridad de la información, que abarca medidas técnicas, organizativas y procedimentales para proteger la confidencialidad, integridad y disponibilidad de los datos y sistemas.
- Soporte a usuarios internos y externos en el uso de tecnologías y sistemas.
- Gestión de accesos, identidades y privilegios de usuarios.
- Control y monitoreo de incidentes de seguridad, incluyendo detección, respuesta y mitigación.
- Planificación y ejecución de planes de continuidad del negocio y recuperación ante desastres.
- Gestión y control de las comunicaciones internas y externas, incluyendo servicios de correo electrónico, acceso remoto y comunicaciones móviles.
- Implementación y mantenimiento de protocolos de seguridad como cifrado y autenticación.
- Gestión del ciclo de vida de los activos TIC, incluyendo adquisición, instalación, actualización y retirada.
- Coordinación de la formación y sensibilización del personal en temas de ciberseguridad.

- Calendario de realización y seguimiento y revisión del análisis.
Aquí está la tabla convertida a formato Markdown:[1]

| Fase | Frecuencia | Responsable |
|------|-----------|-------------|
| Análisis inicial completo | Al arrancar el PDS | Responsable Seguridad |
| Revisión periódica | Anual | Equipos TIC y Seguridad |
| Revisión tras incidentes | Cuando sucedan | Equipos afectados |
| Actualización de activos | Semestral/anual | Administración/TIC |
| Informe a dirección | Anual y tras cambios | Responsable Seguridad |

Seguimiento y revisión continua
El sistema implementado debe contemplar revisiones periódicas que incluyan:
- Actualización del inventario de activos, amenazas y vulnerabilidades.
- Evaluación del impacto de nuevos incidentes o cambios tecnológicos.
- Revisión de la eficacia de las medidas de seguridad implantadas.
- Reajuste de los criterios de aceptación del riesgo.

## 1. Alcance del análisis  {#1.-alcance-del-análisis}
El alcance del análisis en esta empresa debe definirse teniendo en cuenta su estrategia empresarial de transformación digital, la diversidad de sus departamentos y el tipo de activos involucrados.
Estrategia empresarial y su impacto

La empresa está inmersa en una estrategia de transformación digital que tiene como objetivo realizar la mayoría de los trabajos a través de internet, apoyándose en la página web y utilizando redes sociales para ampliar su presencia y captar clientes.

El cambio estratégico afecta directamente a
- La dependencia de servicios en la nube y proveedores externos (página web, tienda online, almacenamiento).​
- La gestión y protección de datos sensibles de clientes, proveedores y operaciones internas.
- La necesidad de asegurar la continuidad operativa y la protección frente a incidentes que puedan afectar a la disponibilidad, integridad y confidencialidad de la información.​

Departamento o área a analizar
- Todos los departamentos que participan en la gestión, procesamiento y almacenamiento de información crítica: TIC, facturación y ventas, compras, RRHH, comunicación y RRSS, delivery, legal, mantenimiento y consejo de administración.
- Las dos sedes físicas, sus sistemas internos , los servidores, conexiones de red, router, wifi y servicios en la nube.
- Los servicios y activos externalizados: página web/tienda online, servicios en la nube, proveedores subcontratados de seguridad física y ciberseguridad.


## 2. Identificación de los activos  {#2.-identificación-de-los-activos}

Activos principales identificados
- Puestos de trabajo: Ordenadores personales, impresoras y teléfonos fijos.
- Dispositivos móviles: Portátiles, teléfonos móviles y tabletas, fundamentales para el trabajo remoto, el acceso a información en movilidad y la comunicación con clientes y proveedores.​
- Sistemas de almacenamiento externo: Discos duros externos y pendrives, empleados para transportar información sensible o realizar copias de seguridad locales.​
- Servidores locales: Incluyen servidores de correo electrónico, servidores de archivos y aplicaciones, esenciales para la gestión interna, el almacenamiento y procesamiento de la información.​

Infraestructura de red
- Servicios en la nube: Espacios para almacenamiento y aplicaciones
- Página web y tienda online: Canales principales de captación de clientes y prestación de servicios, alojados en proveedores externos.​

Información y datos:
- Datos personales de clientes y proveedores.
- Información financiera, contractual y de gestión interna.
- Propiedad intelectual.
- Documentación y registros, tanto en formato físico como digital, que sustentan los procesos de la empresa y cumplen requisitos legales.​

Razonamiento y prioridades
- Estos activos han sido seleccionados por su impacto directo en la operativa diaria, la continuidad del negocio y el cumplimiento normativo.
- Sin estos activos, la empresa no podría prestar servicio alguno o se expondría a sanciones legales y pérdidas económicas severas.
- Muchos de estos activos están distribuidos en dos sedes, por tanto su protección afecta a toda la organización.
- El uso de servicios en la nube y la externalización de la web amplía la superficie de riesgo más allá del perímetro físico de la empresa.​


## 3. Amenazas que pueden afectar a los activos {#3.-amenazas-que-pueden-afectar-a-los-activos}

1. Amenazas Intencionadas y Maliciosas
. Acceso no autorizado
- Hacking y código malicioso (malware): Ataques de hackers, virus, ransomware o spyware que buscan robar, destruir o secuestrar información.​
- Espionaje industrial: Intentos de obtener información confidencial.
- Robo, fraude y vandalismo
- Ataques terroristas o sabotaje
  
2. Amenazas de Origen Humano (Accidentales)
- Error de usuario: Un empleado que elimina un archivo importante por accidente, introduce datos incorrectos o cae en una estafa de phishing.
- Divulgación de información: Revelar información confidencial sin mala intención.
- Instalación de software no autorizado.
  
3. Amenazas Ambientales y Físicas
- Desastres naturales
- Interrupción de servicios esenciales
- Desastres por causas humanas​

4. Fallos Técnicos y Operacionales
- Mal funcionamiento del equipo.
- Errores de software (bugs).
- Fallo en los enlaces de comunicación.


## 4. Identificar vulnerabilidades y salvaguardas {#4.-identificar-vulnerabilidades-y-salvaguardas}

Vulnerabilidades identificables en activos de la empresa:
- Equipos con antivirus no actualizado o sin soporte del fabricante.
- Ausencia o insuficiencia de políticas de seguridad documentadas.
- Falta de control sobre la seguridad de la página web externa.
- Uso de dispositivos móviles sin medidas adecuadas de protección, como cifrado o gestión remota.
- Existencia de puntos de acceso WiFi sin controles adecuados.
- Copias de seguridad básicas, centralizadas sin estrategias de redundancia ni respaldo en la nube.

Salvaguardas actuales y recomendables para los activos:
- Antivirus actualizado y gestionado por personal especializado.
- Firewall segmentado según departamentos para limitar accesos internos.
- Gestión contractual formal de la seguridad física y servicios externos que cubren control de accesos y vigilancia.
- Procedimientos documentados para copias de seguridad, recomendando también validaciones periódicas y almacenamiento en ubicaciones separadas.
- Implementación de políticas de seguridad formalizadas, incluyendo gestión de accesos, uso aceptable de dispositivos y control de actualizaciones.
- Para la página web externa, establecer acuerdos de nivel de servicio (SLA) que incluyan revisiones periódicas de seguridad y parcheo.
- Implantación de medidas móviles como cifrado de dispositivos, autenticación fuerte y soluciones MDM (Mobile Device Management).


### 4.1. Identificación de salvaguardas (Medidas y controles de seguridad)  {#4.1-identificación-de-salvaguardas-(medidas-y-controles-de-seguridad)}

> Apóyate y consulta el archivo: 2.1. Control ISO 27002.pdf y 2.2. Control ISO 27002 Ampliado.pdf

### 4.2. Vulnerabilidades/Debilidades {#4.2-vulnerabilidades/debilidades}

> Apóyate y consulta el archivo: 3.2 Listado de Amenazas y Vulnerabilidades ISO27000.pdf y 3.3 Margerit

## 5. Evaluación y cálculo del riesgo {#5.-evaluación-y-cálculo-del-riesgo}

Para cada par activo-amenaza, estimaremos la probabilidad de que la amenaza impacte sobre el negocio: probabilidad x impacto.

Decidir el umbral a partir del cual se aceptará el riesgo.

## 6. Medidas complementarias que permitan materializar la protección de los activos. {#6.-medidas-complementarias-que-permitan-materializar-la-protección-de-los-activos.}

Tomar una estrategia para tratar el riesgo y obtener riesgo residual tras aplicar estrategia.  
Iniciativas para implantar controles o salvaguardas.

## 7. Conclusión {#7.-conclusión}

## 8. Bibliografía/Webgrafía {#8.-bibliografía/webgrafía}
