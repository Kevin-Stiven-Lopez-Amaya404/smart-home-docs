# Registro QA — Backend

Registro de verificación de la documentación del backend.

**Actualización:** 2026-11-02 · **Responsable de revisión:** pendiente de asignar

## Fase 1 — Traslado de documentación desde `smarthome-backend`

- SHA de origen (`smarthome-backend/dev`): `3bfce85af680af4a0887fe60d03aa83b482e669e`
- SHA base de `smart-home-docs/main`: `f4d1fe99db500077d46db0be3ceee6d1ee1092dd`
- Los enlaces a código del backend se fijaron al SHA de origen; los enlaces a `smarthome-database` se fijaron a su rama `dev` en `39416a5c42d35f988689061ffca8a79f7fa21002`.

### Tabla de verificación

SHA-256 calculado sobre el original y sobre la copia antes de cualquier edición (iguales en 13/13). Después de copiar solo se cambiaron enlaces y se agregó la nota de Estado documental donde corresponde.

| Origen | Destino | Bytes | SHA-256 original = copia | Enlaces internos actualizados | Nota de estado | Revisión de secretos |
|---|---|---|---|---|---|---|
| `docs/CONSUMPTION_METRICS_WORKER.md` | `backend/consumo/consumption-metrics-worker.md` | 1491 | `8550801bf5b0515b…` ✔ | 0 | Sí (2026-10-28) | Revisado: URL con marcadores `<secret>`, sin valores reales |
| `docs/HU09_RATE_LIMITING.md` | `backend/seguridad/rate-limiting.md` | 7409 | `c9e7faf6a0e1f4fe…` ✔ | 0 | No | Revisado: sin secretos |
| `docs/HU09_REALTIME_SECURITY.md` | `backend/seguridad/realtime-security.md` | 9793 | `514c48a061be0228…` ✔ | 1 | No | Revisado: sin secretos |
| `docs/HU09_SESSION_FAMILIES.md` | `backend/seguridad/session-families.md` | 8553 | `b3f2d7e4c090eded…` ✔ | 2 | No | Revisado: sin secretos |
| `docs/HU10_MQTT_TLS_NAMESPACE.md` | `backend/iot/mqtt-tls-namespace.md` | 9656 | `e877fcb628032635…` ✔ | 0 | No | Revisado: sin secretos |
| `docs/HU16_CONSUMPTION_ACCESS.md` | `backend/consumo/consumption-access.md` | 8199 | `e6b591cc8b272fad…` ✔ | 0 | No | Revisado: UUID sintético de fixture y `127.0.0.1`, sin secretos |
| `docs/HU16_PAIRING_AP_SESSIONS.md` | `backend/iot/shelly-pairing-lan-ap-sessions.md` | 8472 | `01aaba59ce7a4877…` ✔ | 0 | Sí (2026-10-19) | Revisado: IP `192.168.33.1` es la IP por defecto del AP Shelly, sin datos de hogares |
| `docs/IMPLEMENTACION_HU09.md` | `backend/historico/implementacion-hu09.md` | 6786 | `d727f3824b8ff661…` ✔ | 5 | Sí (2026-10-14) | Revisado: sin secretos |
| `docs/INFORME_01_AUDITORIA_BACKEND_BD_2026-10-12.md` | `backend/historico/auditoria-backend-bd-2026-10-12.md` | 86324 | `80b6a4a1ab7ebadc…` ✔ | 40 | Sí (2026-10-12) | Revisado: sin secretos |
| `docs/MQTT_CONTRACT.md` | `backend/iot/mqtt-contract.md` | 7469 | `0b482b0f97137e28…` ✔ | 1 | Sí (2026-10-15) | Revisado: sin secretos |
| `docs/REPORTE_AVANCE_HU09_2026-10-14.md` | `backend/historico/avance-hu09-2026-10-14.md` | 11209 | `87555648c87f8d6e…` ✔ | 7 | Sí (2026-10-14) | Revisado: sin secretos |
| `docs/ROLES_Y_PERMISOS.md` | `backend/seguridad/roles-y-permisos.md` | 3524 | `062fdcbc3c4f43c9…` ✔ | 0 | No | Revisado: sin secretos |
| `ALCANCE_2026_09_08.md` | `backend/historico/alcance-2026-09-08.md` | 5254 | `2eb753eebe422b20…` ✔ | 0 | Sí (2026-09-08) | Revisado: contiene una URL de BD de prueba sintética en `127.0.0.1` (fixture desechable), sin secretos reales |

**Resultado:** 13/13 documentos copiados e íntegros.

### Pendiente de completar

- [ ] URL del PR documental y commit de merge en `smart-home-docs`.
- [ ] Verificación de enlaces públicos de destino después del merge.
- [ ] URL del PR del backend, SHA final y responsable de revisión.
- [ ] Registro de la protección de `dev` (reglas efectivas o bloqueo documentado).
