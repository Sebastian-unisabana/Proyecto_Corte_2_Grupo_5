# StartUp — Sistema de Logística Escalado

**Proyecto Corte 2 | Programación y Decisiones**
Universidad de La Sabana | Profesor: Diego Mauricio Zuluaga Rodríguez

---

## Integrantes

| Nombre | GitHub |
|--------|--------|
| Samuel Gonzales | @samuelgonbe |
| Samuel Lozano | @desamuel2704-sys |
| Sebastián Vanoy | @Sebastian-unisabana |

---

## Descripción

Sistema de gestión de envíos y paquetería para el StartUp de Logística.
Escala el MVP del Corte 1 (Reto 1 — Logística) a una arquitectura profesional
con POO, encapsulamiento y persistencia en base de datos SQLite.

---

## Arquitectura

**Lenguaje:** Python
**Base de datos:** SQLite (archivo .db persistente)
**Paradigma:** Programación Orientada a Objetos con herencia y encapsulamiento (POO)
**Entorno:** Jupyter Notebook

**Jerarquía de clases:**

- Persona → Cliente
- Ruta → Destino
- Envio → Paquete

**Tablas y relaciones:**

- clientes (PK: id_cliente)
- destinos (PK: id_destino)
- paquetes (PK: id_paquete | FK: id_cliente, id_destino)

---

## Funcionalidades (Menú CRUD)

- Registrar clientes y destinos
- Registrar paquetes con clasificación y costo automático
- Ver manifiesto completo con JOIN (clientes + paquetes + destinos)
- Actualizar peso y destino de un paquete
- Eliminar paquetes con confirmación

---

## Estructura del Repositorio

- design/diagrama_clases.pdf — Diagrama de Clases UML
- design/modelo_ER.pdf — Modelo Entidad-Relación
- app_escalada_grupo_5.ipynb — Código fuente documentado y funcional

---

## Ejecución

1. Clonar el repositorio
2. Abrir app_escalada_grupo_5.ipynb en Jupyter Notebook o Google Colab
3. Ejecutar todas las celdas en orden
4. La base de datos base_datos_startup_grupo_5.db se crea automáticamente
