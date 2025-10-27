# Proyecto Segundo Corte – Infraestructura Virtualizada y Monitoreo Centralizado

**Autor:**  
Mariana Lombana y Rodian 

---

## Índice

1. [Descripción General](#descripción-general)  
2. [Objetivos](#objetivos)  
   - 2.1 [Objetivo General](#objetivo-general)  
   - 2.2 [Objetivos Específicos](#objetivos-específicos)  
3. [Arquitectura del Proyecto](#arquitectura-del-proyecto)  
   - 3.1 [Nodo Central Administrador](#nodo-central-administrador)  
   - 3.2 [Dependencias de la Empresa Simulada](#dependencias-de-la-empresa-simulada)  
4. [Red y Conectividad](#red-y-conectividad)  
5. [Tecnologías y Herramientas Utilizadas](#tecnologías-y-herramientas-utilizadas)  
6. [Metodología y Desarrollo](#metodología-y-desarrollo)  
   - 6.1 [Instalación y Configuración](#instalación-y-configuración)  
   - 6.2 [Monitoreo y Análisis de Sistemas](#monitoreo-y-análisis-de-sistemas)  
   - 6.3 [Despliegue de Aplicaciones Web](#despliegue-de-aplicaciones-web)  
   - 6.4 [Dashboard Centralizado](#dashboard-centralizado)  


---

## Descripción General

El proyecto “Segundo Corte” tiene como finalidad principal **integrar conocimientos teóricos y prácticos de administración de sistemas operativos, redes y virtualización**, a través de la implementación de una infraestructura empresarial simulada.  

La empresa simulada cuenta con varias dependencias, cada una con **máquinas virtuales o contenedores**, que permiten practicar la gestión de hardware, software, procesos y tráfico de red. Todo esto se centraliza mediante un **nodo administrador**, que facilita la coordinación, monitoreo y seguridad de la infraestructura.

El proyecto combina **herramientas de DevOps y NetOps**, fomentando la aplicación de buenas prácticas en entornos corporativos y académicos, incluyendo versionamiento, documentación y despliegue de contenedores en Docker Hub.

---

## Objetivos

### Objetivo General
Diseñar, implementar y documentar una **infraestructura virtualizada y monitoreada centralmente**, que permita la administración eficiente de los recursos de múltiples dependencias en un entorno simulado empresarial.

### Objetivos Específicos
- Implementar máquinas virtuales y contenedores para cada dependencia.  
- Configurar subredes privadas y controladas que permitan comunicación segura entre dependencias.  
- Analizar el hardware, procesos, almacenamiento y tráfico de red mediante comandos especializados.  
- Desarrollar un dashboard centralizado en Grafana para la visualización de métricas en tiempo real.  
- Documentar todo el proyecto en GitHub, incluyendo scripts, diagramas y evidencias visuales.  
- Publicar contenedores personalizados en Docker Hub para replicabilidad.

---

## Arquitectura del Proyecto

### Nodo Central Administrador
- **Sistema Operativo:** Debian  
- **Función:** Servidor principal que administra todas las dependencias, controla la comunicación de subredes, ejecuta monitoreo centralizado y gestiona logs y métricas de los sistemas.  

### Dependencias de la Empresa Simulada

1. **Recursos Humanos**  
   - Máquinas virtuales: Arch Linux / Manjaro  
   - Función: Monitoreo de hardware, procesos activos, gestión de archivos y análisis de almacenamiento.  

2. **Tecnología**  
   - Máquinas virtuales: Rocky Linux / Kali Linux  
   - Función: Administración de servicios, procesos críticos y gestión de redes internas.  

3. **Financiera**  
   - Contenedores: Garuda Linux / Ubuntu / Alpine  
   - Función: Gestión de archivos, almacenamiento y monitoreo del tráfico interno de contenedores.  

4. **Ventas y Comercio**  
   - Contenedores: Fedora / Alma Linux  
   - Función: Despliegue de aplicaciones web para clientes, pruebas de seguridad y auditoría de servicios.

---

## Red y Conectividad

- Cada dependencia se encuentra en su propia **subred virtual**, controlada por el nodo administrador.  
- La comunicación entre subredes está **limitada y monitoreada**, asegurando que solo los servicios autorizados puedan interactuar.  
- Se implementaron redes privadas virtuales para **aislamiento seguro** de cada área y para prácticas de análisis de tráfico y seguridad.  

---

## Tecnologías y Herramientas Utilizadas

- **Sistemas Operativos:** Debian, Arch Linux, Rocky Linux, Garuda, Fedora, Kali Linux, Alma Linux  
- **Virtualización y Contenedores:** QEMU/KVM, Docker  
- **Monitoreo y Visualización:** Grafana, Netdata, Lynis  
- **Análisis de Sistemas:** `top`, `htop`, `lshw`, `dmidecode`, `ncdu`, `rsync`, `lsof`  
- **Aplicaciones Web:** Streamlit  
- **Control de Versiones:** Git y GitHub  
- **Repositorio de Contenedores:** Docker Hub  

---

## Metodología y Desarrollo

### Instalación y Configuración
- Instalación de sistemas operativos en máquinas virtuales y contenedores.  
- Configuración de redes internas y asignación de direcciones IP estáticas.  
- Implementación de usuarios, permisos y servicios esenciales para cada dependencia.

### Monitoreo y Análisis de Sistemas
- Uso de comandos y herramientas para inspección de hardware, procesos y logs.  
- Análisis de tráfico de red y almacenamiento mediante herramientas nativas y contenedores especializados.  
- Generación de reportes periódicos para cada dependencia.

### Despliegue de Aplicaciones Web
- Implementación de aplicaciones de ejemplo en Streamlit para la dependencia de Ventas y Comercio.  
- Configuración de puertos y auditoría de seguridad mediante `nmap` y `lynis`.  
- Integración de la aplicación web con el nodo administrador para monitoreo centralizado.

### Dashboard Centralizado
- Configuración de Grafana para visualizar métricas de CPU, memoria, almacenamiento y red.  
- Creación de paneles personalizados para cada dependencia y servicios críticos.  
- Integración de alertas y logs centralizados para control eficiente del entorno.

