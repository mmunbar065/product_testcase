# Caso Practico Entrevista Product Owner

Este repositorio contiene un caso práctico anonimizado desarrollado por Marta Muñoz Barrios, diseñado para demostrar competencias clave en la gestión técnica de producto (Technical Product Management) dentro de un entorno de comercio electrónico y alta transaccionalidad.
El objetivo de este proyecto es ilustrar cómo se aborda el ciclo de vida de una funcionalidad compleja de backend y la gestión de crisis en producción, desde la definición de la oportunidad de negocio hasta la solución técnica y la observabilidad.


**📄 Resumen del Contenido**
**Caso 1: Modificación de Reservas Temporales (RT)**
Problema: El sistema actual cancelaba la reserva temporal al modificar el carrito, liberando stock y generando riesgo de pérdida de unidades para el usuario.
Solución Propuesta: Implementación de una lógica de actualización (updateReservation) que mantiene la reserva activa y renueva el TTL (Time-to-Live) tras una modificación exitosa, mejorando la tasa de conversión y la experiencia de usuario.


**Caso 2: Gestión de Incidencia (Caída de Conversión)**

**Escenario:** Detección de una caída en la conversión a pedido confirmado y aumento de latencia en los endpoints de refresh y confirm.

**Estrategia de Resolución:**
1. Detección: Monitoreo de tasas de error 5xx y saturación de recursos (CPU, conexiones DB) mediante herramientas como Grafana o Elastic APM.
2. Mitigación: Rollback inmediato de despliegues recientes, escalado temporal de infraestructura y activación de mecanismos de bypass.
3. Coordinación: Comunicación basada en datos con stakeholders y ejecución de análisis post-mortem para evitar regresiones.

👤**Sobre la Autora**
Marta Muñoz Barrios es Product & Delivery Manager con más de 8 años de experiencia liderando el desarrollo de productos digitales en sectores como IoT, Energía y Telco. Especializada en traducir necesidades de negocio en soluciones técnicas efectivas, integración de APIs y metodologías Ágiles.

<img width="1391" height="781" alt="image" src="https://github.com/user-attachments/assets/9e239afa-adb1-4707-a138-0c3d67df336b" />
<img width="1408" height="795" alt="image" src="https://github.com/user-attachments/assets/551dec46-4176-47cf-9cbb-f3b84a3711a0" />
<img width="1397" height="788" alt="image" src="https://github.com/user-attachments/assets/97fad657-047c-4454-b864-6a1fb7844c68" />
<img width="1372" height="778" alt="image" src="https://github.com/user-attachments/assets/abe3362b-d165-417e-8843-494b0439dd3f" />
<img width="1411" height="797" alt="image" src="https://github.com/user-attachments/assets/0bdb5b0c-07e2-4f24-bcff-0fc8dbe01c8b" />




