# Bryan Ramírez Palacios
## Arquitecto de Soluciones Cloud y Gestor de Proyectos Tecnológicos

Soy un ingeniero apasionado por diseñar, desplegar y gestionar arquitecturas de nube robustas, escalables y seguras. Mi objetivo es combinar mi experiencia técnica en una amplia gama de tecnologías de vanguardia con una mentalidad estratégica para liderar proyectos complejos y entregar soluciones de alto impacto que impulsen el éxito del negocio. Busco constantemente traducir los desafíos técnicos en resultados medibles y valoro la resolución de problemas a través de la experimentación y el aprendizaje continuo.

## 🚀 Tecnologías y Herramientas

### Lenguajes de Programación
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### Frameworks y Librerías
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

### Cloud & DevOps
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)

### Bases de Datos
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)

### Big Data
![Hadoop](https://img.shields.io/badge/Hadoop-66CCFF?style=for-the-badge&logo=apachehadoop&logoColor=black)

## 📋 Proyecto Portfolio

A continuación se presentan algunos de los proyectos que demuestran mi experiencia en el diseño de arquitecturas, la implementación de soluciones en la nube y la gestión de despliegues complejos.

### 1. PredictHealth: Ecosistema SaaS para la Gestión Proactiva de la Salud

**Descripción:** Se diseñó y desarrolló la arquitectura para una plataforma de Software como Servicio (SaaS) orientada a transformar la gestión de enfermedades crónicas. El sistema integra datos clínicos, de estilo de vida (wearables) y GPS para generar mapas de riesgo personalizados mediante IA.

**Arquitectura y Resultados:**
- Implementé una arquitectura de microservicios desacoplada y orientada a eventos para garantizar alta disponibilidad y escalabilidad
- Se orquestaron servicios de backend en Python/FastAPI y se gestionaron bases de datos heterogéneas (PostgreSQL para datos transaccionales, Redis como caché y bus de mensajes, Hadoop para procesamiento de Big Data en el entrenamiento de modelos de IA y Firebase para sincronización en tiempo real)
- El resultado es una plataforma robusta, centrada en el médico y diseñada bajo principios de seguridad y ética, capaz de procesar múltiples fuentes de datos para la detección temprana de riesgos de salud

### 2. Blindando Aplicaciones con AWS WAF

**Descripción:** Este proyecto demostró la importancia de la seguridad en la nube mediante la protección de una aplicación web vulnerable a ataques de inyección SQL.

**Arquitectura y Resultados:**
- Se contrastaron dos arquitecturas: una insegura con un contenedor ECS expuesto directamente a internet y una segura utilizando AWS WAF junto a un Application Load Balancer (ALB)
- **Resultado Objetivo:** El ataque de inyección SQL (' OR '1'='1') fue exitoso en la arquitectura insegura. En la arquitectura protegida, el mismo ataque fue interceptado y bloqueado por AWS WAF, devolviendo un código de estado 403 Forbidden
- Se validó una estrategia de defensa en profundidad, aislando el contenedor en una subred privada y utilizando Security Groups para microsegmentación, demostrando un diseño de infraestructura seguro y resiliente

### 3. Arquitectura de Contenedores en AWS con Kubernetes (Prueba de Concepto)

**Descripción:** Se diseñó una arquitectura distribuida y resiliente para una aplicación crítica utilizando Amazon EKS, AWS Fargate, Amazon SQS y ElastiCache. Se ejecutó una Prueba de Concepto (POC) para validar los componentes clave.

**Resultados y Lecciones Aprendidas:**
- **Éxito Parcial:** Se logró desplegar exitosamente una aplicación base con dos réplicas en un clúster de EKS, validando la auto-reparación de pods
- **Desafíos Identificados:** La creación automática del Elastic Load Balancer (ELB) y el Horizontal Pod Autoscaler (HPA) fallaron durante las pruebas de carga
- **Lecciones Clave:** Este ejercicio subrayó la criticidad de una correcta configuración de networking (etiquetado de subredes) y permisos (IAM) en AWS. El fracaso parcial se convirtió en una valiosa experiencia de aprendizaje sobre la importancia de la validación incremental en arquitecturas complejas

### 4. Despliegue de un Clúster de Kubernetes en AWS desde Cero

**Descripción:** Se construyó y administró un clúster de Kubernetes funcional sobre instancias EC2 de AWS (Ubuntu Server), desplegando una aplicación web multicontenedor (WordPress con MySQL).

**Resultados y Habilidades Demostradas:**
- **Infraestructura Funcional:** Se configuró con éxito un clúster de dos nodos (maestro y trabajador) con containerd, kubeadm y Calico como CNI
- **Despliegue Persistente:** Se implementó WordPress utilizando Deployments, Services, Secrets y PersistentVolumes para garantizar la persistencia de los datos de la base de datos MySQL
- **Resolución de Problemas Complejos:** Durante el proyecto, se diagnosticaron y resolvieron problemas críticos, incluyendo el uso de repositorios de paquetes de Kubernetes obsoletos, incompatibilidades con manifiestos de Calico y un estado corrupto en el volumen persistente de MySQL. Esto demostró una fuerte capacidad para la depuración sistemática en entornos de orquestación

### 5. Sistema de Microservicios para una Joyería

**Descripción:** Se implementó un sistema de comercio electrónico basado en una arquitectura de microservicios para desacoplar las responsabilidades del negocio.

**Arquitectura y Resultados:**
- El sistema se compuso de cuatro servicios independientes: un frontend SPA (Single Page Application), un microservicio de Productos (Flask, XML), un microservicio de Pedidos (Flask, JSON) y un microservicio de Facturas (Flask, XML con XSLT)
- **Resultado Objetivo:** Se logró un sistema completamente funcional donde el frontend orquesta llamadas asíncronas a los diferentes microservicios, gestiona un carrito de compras y genera facturas, con todos los pedidos persistiendo en una base de datos MariaDB. El proyecto validó la capacidad de integrar servicios que consumen y producen diferentes formatos de datos (JSON y XML)

## 📊 Estadísticas de GitHub

![Bryan's GitHub stats](https://github-readme-stats.vercel.app/api?username=tuusuario&show_icons=true&theme=radical)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=tuusuario&layout=compact&theme=radical)

## 📫 Contacto

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/bryramirezp/)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tu.email@example.com)

---
⭐️ From [bryramirezp](https://github.com/tuusuario)
