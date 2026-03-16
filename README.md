# Diseño de Arquitectura de Soluciones: Sistema de Banca por Internet BP

[![Architecture: C4 Model](https://img.shields.io/badge/Architecture-C4_Model-blue.svg)](https://c4model.com/)
[![Cloud: Azure](https://img.shields.io/badge/Cloud-Microsoft_Azure-0089D6.svg?logo=microsoft-azure&logoColor=white)](https://azure.microsoft.com/)
[![Backend: .NET](https://img.shields.io/badge/Backend-.NET_Core-512BD4.svg?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
[![Status: Completed](https://img.shields.io/badge/Status-Completed-success.svg)]()

> Propuesta técnica integral desarrollada como prueba técnica para el rol de Arquitecto de Soluciones / Backend Developer.

## Resumen Ejecutivo
Este repositorio contiene la documentación oficial y el diseño arquitectónico propuesto para el nuevo **Sistema de Banca por Internet de la entidad BP**. 

La solución está orientada a garantizar el estricto cumplimiento normativo bancario, asegurar alta disponibilidad (HA) e implementar un ecosistema seguro bajo el principio de "Confianza Cero" (Zero Trust), soportando operaciones críticas como transferencias interbancarias y consultas en tiempo real.

## Entregable Principal

* **[`Prueba_Tecnica_Arquitectura_BP_Diego_Cuaycal.pdf`](./Prueba_Tecnica_Arquitectura_BP_Diego_Cuaycal.pdf)**: Documento principal con la resolución completa del caso de estudio, diagramas y justificaciones.

### Estructura del Documento
1. **Decisiones Arquitectónicas:** Justificación profunda del stack tecnológico elegido.
2. **Seguridad y Onboarding:** Flujos de validación biométrica y gestión de identidades.
3. **Capa de Integración y Datos:** Orquestación de microservicios y persistencia de alta velocidad.
4. **Modelado C4:** Diagramas de Contexto (Nivel 1), Contenedores (Nivel 2) y Componentes (Nivel 3).
5. **Consideraciones Normativas:** Estrategias de resiliencia, auditoría y escalabilidad.

## Stack Tecnológico y Patrones Propuestos

El diseño estructurado en el documento se fundamenta rigurosamente en las siguientes decisiones técnicas:

* **Frontend & Mobile:** `Angular` (Arquitectura robusta y escudos OWASP) y `Flutter` (Rendimiento AOT para Onboarding biométrico).
* **Backend Core:** `.NET (C#)` (Orquestación asíncrona y precisión transaccional).
* **Cloud & IA:** `Microsoft Azure` (API Management, Cosmos DB y servicios cognitivos con Azure Face API).
* **Patrones de Arquitectura:** `Microservicios`, `API Gateway`, `API Composition` (Agregador de cliente), `Cache-Aside` (Redis) y `Publish-Subscribe` (Azure Service Bus).
* **Seguridad y Resiliencia:** `OAuth 2.0 + PKCE`, delegación de identidad (`FIDO2/WebAuthn`) y tolerancia a fallos mediante `Circuit Breaker`.

## Autor

**Ing. Diego Cuaycal**
*Ingeniero de Software*

* **Portafolio:** [dev-portfolio-diego.vercel.app](https://dev-portfolio-diego.vercel.app/)
* **GitHub:** [@DiegoCuaycal](https://github.com/DiegoCuaycal)

---
*Documentación estructurada bajo estándares de ingeniería de software para evaluación técnica.*
