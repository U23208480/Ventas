# Tablero de Actividades - Sistema de Ventas

Equipo: Juan César Retuerto Ibañez - U23208480 | Alberto Joel Ramirez Ponte - U23249035

El tablero Kanban está en GitHub Projects (columnas Pendiente, En progreso, Bloqueado y Completado) y cada tarjeta corresponde a un issue del repositorio.

## Actividades

| ID | Actividad | Responsable | Estado | Prioridad | Inicio | Entrega | Criterio de cierre | Evidencia | Depende de |
|----|-----------|-------------|--------|-----------|--------|---------|--------------------|-----------|------------|
| A01 | Diseñar modelo de base de datos de ventas | Alberto | Completado | Alta | 28/09/2026 | 05/10/2026 | Diagrama ER aprobado por el equipo | Diagrama ER v1.0 | - |
| A02 | Desarrollar módulo de registro de clientes | Juan | En progreso | Alta | 06/10/2026 | 15/10/2026 | CRUD de clientes funcional con validaciones | Código en repositorio + pruebas unitarias | - |
| A03 | Implementar autenticación y control de acceso | Juan | En progreso | Alta | 09/10/2026 | 18/10/2026 | Login funcional con roles definidos | Capturas de pantalla + código | - |
| A04 | Crear catálogo de productos | Alberto | Pendiente | Media | 13/10/2026 | 20/10/2026 | Listado de productos con precio y stock | Módulo desplegado en staging | - |
| A05 | Desarrollar carrito de compras | Alberto | Pendiente | Alta | 16/10/2026 | 25/10/2026 | Usuario puede agregar y eliminar productos | Pruebas de flujo completo | A04 |
| A06 | Implementar proceso de checkout y pedidos | Juan | Bloqueado | Alta | 21/10/2026 | 28/10/2026 | Pedido generado correctamente con número de orden | Registro de pedido en BD | A05 |
| A07 | Integrar pasarela de pagos | Alberto | Bloqueado | Alta | 26/10/2026 | 02/11/2026 | Pago procesado y confirmado exitosamente | Transacción de prueba exitosa | A06 |
| A08 | Generar reportes de ventas por período | Juan | Pendiente | Media | 29/10/2026 | 05/11/2026 | Reporte exportable en PDF/Excel | Reporte generado con datos reales | - |
| A09 | Desarrollar panel de control (dashboard) | Alberto | Pendiente | Media | 01/11/2026 | 08/11/2026 | KPIs visibles en tiempo real | Capturas del dashboard funcional | - |
| A10 | Implementar notificaciones por correo | Juan | Pendiente | Baja | 04/11/2026 | 10/11/2026 | Email enviado al confirmar pedido | Log de emails enviados | - |
| A11 | Realizar pruebas de integración del sistema | Alberto | Pendiente | Alta | 06/11/2026 | 15/11/2026 | 0 errores críticos en suite de pruebas | Reporte de pruebas QA | A07 |
| A12 | Desplegar sistema en producción | Juan | Pendiente | Alta | 11/11/2026 | 20/11/2026 | Sistema accesible en URL de producción | URL de producción + checklist de deploy | A11 |

## Vista rápida (respuestas en menos de 60 segundos)

**¿Qué se está haciendo?**
- A02 Registro de clientes (Juan)
- A03 Autenticación y control de acceso (Juan)

**¿Quién lo hace?**
- Juan: A02, A03, A06, A08, A10 y A12
- Alberto: A01, A04, A05, A07, A09 y A11

**¿Qué está bloqueado?**
- A06 Checkout y pedidos: espera a A05 (carrito de compras).
- A07 Pasarela de pagos: espera a A06 (checkout y pedidos).
- Dependientes en cadena: A05 espera a A04, A11 espera a A07 y A12 espera a A11.

**¿Qué se termina primero?**
1. A02 Registro de clientes (15/10/2026)
2. A03 Autenticación y control de acceso (18/10/2026)
3. A04 Catálogo de productos (20/10/2026)
