# Tablero de actividades - Sistema de Ventas

Equipo: Juan César Retuerto Ibañez - U23208480 | Alberto Joel Ramirez Ponte - U23249035

Estados posibles: `Por hacer`, `En progreso`, `Bloqueada`, `Hecha`.
Prioridades: `Alta`, `Media`, `Baja`.

## Tablero

| ID | Actividad | Responsable | Estado inicial | Prioridad | Fecha de entrega | Criterio de cierre | Evidencia | Depende de |
|----|-----------|-------------|----------------|-----------|------------------|--------------------|-----------|------------|
| A01 | Definir alcance y requisitos del sistema de ventas | Juan | En progreso | Alta | 2026-10-15 | Lista de requisitos revisada por ambos integrantes | `docs/requisitos.md` | - |
| A02 | Diseñar modelo de datos (clientes, productos, ventas, detalle) | Alberto | Por hacer | Alta | 2026-10-17 | Diagrama entidad-relación revisado y aprobado | `docs/modelo-datos.md` | A01 |
| A03 | Crear repositorio y ramas main / develop | Juan | En progreso | Alta | 2026-10-14 | Repositorio publicado con ramas main y develop | URL del repositorio | - |
| A04 | Módulo de clientes (registrar y listar) | Juan | Por hacer | Media | 2026-10-22 | Registrar y listar funcionan sin errores | Commit en `feature/clientes` | A02, A03 |
| A05 | Módulo de productos (registrar, listar y stock) | Alberto | Por hacer | Media | 2026-10-22 | Registrar y listar funcionan, el stock se guarda | Commit en `feature/productos` | A02, A03 |
| A06 | Módulo de ventas (registrar venta con detalle y total) | Juan | Bloqueada | Alta | 2026-10-27 | Una venta guarda cliente, productos y total correcto | Commit en `feature/ventas` | A04, A05 |
| A07 | Cálculo de IGV y total de la venta | Alberto | Bloqueada | Media | 2026-10-28 | Total con IGV coincide con el cálculo manual | Captura de la prueba | A06 |
| A08 | Validaciones (stock insuficiente, datos vacíos) | Juan | Por hacer | Media | 2026-10-29 | Los casos inválidos muestran un mensaje y no se guardan | Commit de validaciones | A05, A06 |
| A09 | Reporte de ventas por fecha | Alberto | Por hacer | Baja | 2026-10-30 | El reporte lista las ventas de un rango de fechas | Captura del reporte | A06 |
| A10 | Pruebas funcionales de los casos principales | Alberto | Por hacer | Alta | 2026-11-02 | Casos de prueba ejecutados sin fallos | `docs/pruebas.md` | A06, A07, A08 |
| A11 | Manual de uso en el README | Alberto | Por hacer | Baja | 2026-11-03 | README explica cómo registrar clientes, productos y ventas | `README.md` actualizado | A10 |
| A12 | Revisión cruzada del código (pull request) | Juan | Por hacer | Media | 2026-11-04 | Pull request revisado y fusionado a develop | Enlace del pull request | A10 |
| A13 | Demo y sustentación final | Juan y Alberto | Por hacer | Alta | 2026-11-06 | Demo ejecutada ante el docente | Historial de commits y repositorio final | A11, A12 |

## Vista rápida (respuestas en menos de 60 segundos)

**¿Qué se está haciendo?**
- A01 Definir alcance y requisitos (Juan)
- A03 Crear repositorio y ramas (Juan)

**¿Quién lo hace?**
- Juan: A01, A03, A04, A06, A08, A12 y A13
- Alberto: A02, A05, A07, A09, A10, A11 y A13

**¿Qué está bloqueado?**
- A06 Módulo de ventas: bloqueada hasta terminar A04 (clientes) y A05 (productos).
- A07 Cálculo de IGV: bloqueada hasta terminar A06 (ventas).
- Dependientes: A08, A09, A10, A11, A12 y A13 avanzan en cadena según la columna "Depende de".

**¿Qué se termina primero?**
1. A03 Crear repositorio y ramas (2026-10-14)
2. A01 Definir alcance y requisitos (2026-10-15)
3. A02 Diseñar modelo de datos (2026-10-17)
