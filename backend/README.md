# Documentación del backend SmartHome

Índice de la documentación de [`nataliachala1/smarthome-backend`](https://github.com/nataliachala1/smarthome-backend) (rama de integración `dev`). Estos documentos se trasladaron desde `docs/` y la raíz del backend en la Fase 1, con base en el commit [`3bfce85`](https://github.com/nataliachala1/smarthome-backend/tree/3bfce85af680af4a0887fe60d03aa83b482e669e).

**Actualización:** 2026-11-02 · **Responsable de revisión:** pendiente de asignar

## Arquitectura y contratos

En esta fase no se crearon páginas nuevas de arquitectura ni de API. Los contratos existentes son:

- [Contrato MQTT](iot/mqtt-contract.md) — **pendiente de validación**.
- [MQTT con TLS y namespace (HU10)](iot/mqtt-tls-namespace.md) — implementación documentada.
- La API HTTP se describe con Swagger en el propio backend cuando está habilitado (ver el README del backend).

## Seguridad

| Documento | Clasificación | Ruta anterior en backend |
|---|---|---|
| [Roles y permisos](seguridad/roles-y-permisos.md) | Implementación documentada | `docs/ROLES_Y_PERMISOS.md` |
| [Límites de solicitudes HTTP (HU09)](seguridad/rate-limiting.md) | Implementación documentada | `docs/HU09_RATE_LIMITING.md` |
| [Seguridad de sesiones y eventos Socket.IO (HU09)](seguridad/realtime-security.md) | Implementación documentada | `docs/HU09_REALTIME_SECURITY.md` |
| [Logout individual y familias de sesión (HU09)](seguridad/session-families.md) | Implementación documentada | `docs/HU09_SESSION_FAMILIES.md` |

## Consumo

| Documento | Clasificación | Ruta anterior en backend |
|---|---|---|
| [Permisos de consumo e históricos (HU16)](consumo/consumption-access.md) | Implementación documentada | `docs/HU16_CONSUMPTION_ACCESS.md` |
| [Worker de métricas de consumo](consumo/consumption-metrics-worker.md) | Pendiente de validación | `docs/CONSUMPTION_METRICS_WORKER.md` |

## MQTT / Shelly

| Documento | Clasificación | Ruta anterior en backend |
|---|---|---|
| [Contrato MQTT](iot/mqtt-contract.md) | Pendiente de validación | `docs/MQTT_CONTRACT.md` |
| [MQTT con TLS y namespace (HU10)](iot/mqtt-tls-namespace.md) | Implementación documentada | `docs/HU10_MQTT_TLS_NAMESPACE.md` |
| [Sesiones Shelly LAN-first y AP (HU16)](iot/shelly-pairing-lan-ap-sessions.md) | **Histórico con advertencia de vigencia** — el pairing automático completo no está certificado | `docs/HU16_PAIRING_AP_SESSIONS.md` |

## Operaciones

- [Worker de métricas de consumo](consumo/consumption-metrics-worker.md) (habilitación controlada) — pendiente de validación.

## Histórico

Registran decisiones y resultados de su fecha. No describen el estado actual.

| Documento | Corte original | Ruta anterior en backend |
|---|---|---|
| [Alcance del 8 de septiembre de 2026](historico/alcance-2026-09-08.md) | 2026-09-08 | `ALCANCE_2026_09_08.md` |
| [Auditoría backend y BD](historico/auditoria-backend-bd-2026-10-12.md) | 2026-10-12 | `docs/INFORME_01_AUDITORIA_BACKEND_BD_2026-10-12.md` |
| [Implementación HU09](historico/implementacion-hu09.md) | 2026-10-14 | `docs/IMPLEMENTACION_HU09.md` |
| [Reporte de avance HU09](historico/avance-hu09-2026-10-14.md) | 2026-10-14 | `docs/REPORTE_AVANCE_HU09_2026-10-14.md` |

## Contrato vigente verificado

Ninguno de estos documentos ha sido certificado como contrato vigente en esta fase. Consultar el código de la rama `dev` antes de implementar.

## Enlaces

- Backend: <https://github.com/nataliachala1/smarthome-backend/tree/dev>
- Pruebas del backend: [`src/**/*.spec.ts`](https://github.com/nataliachala1/smarthome-backend/tree/dev/src) y [`test/`](https://github.com/nataliachala1/smarthome-backend/tree/dev/test)
- Registro de QA: [qa/backend/README.md](../qa/backend/README.md)
