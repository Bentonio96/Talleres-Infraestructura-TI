# Talleres — Infraestructura TI

Repositorio de entregas de los talleres del ramo **Infraestructura TI**
(UNAB — último semestre) · **NRC 8485** · **Grupo 6**.

## Integrantes

Benjamín Peña Díaz · Francisco Morales Díaz · Julián Pacheco Muñoz ·
Martín Burgos Vega · Matías Muñoz Parraguirre

Docente: Eduardo Correa Marchant

## Talleres

| Taller | Descripción | Entrega | Estado |
|--------|-------------|---------|--------|
| Taller 1 | Diseño y presupuesto de una infraestructura de red para un edificio corporativo de 5 pisos y 400 usuarios. | [`Taller 1/`](./Taller%201) | Entregado |

> Los siguientes talleres se irán agregando a esta tabla a medida que se completen.

## Taller 1 — Contenido de la entrega

El archivo a subir es **`Entrega1_GRUPO6_NRC8485.zip`**, con el formato de
nombre exigido por el docente (`Entrega1_GRUPOX_NRC8485.zip`). El informe y la
presentación comparten el mismo nombre base, tal como se solicita.

| Archivo | Descripción |
|---------|-------------|
| `Entrega1_GRUPO6_NRC8485.zip` | Entrega completa comprimida. |
| `Entrega1_GRUPO6_NRC8485.docx` / `.pdf` | Informe técnico (Word y PDF), con referencias en formato APA 7. |
| `Entrega1_GRUPO6_NRC8485.pptx` | Presentación de la propuesta — 10 diapositivas (máximo exigido). |
| `Presupuesto - materiales, cantidades y costo total.xlsx` | Detalle de materiales y equipamiento, cantidades, valores unitarios y costo total estimado, más la memoria de cálculo y la comparación de alternativas de cableado. |
| `Planos y diagramas/` | Planos y diagramas de la solución física y lógica, incluida la ubicación y distribución de los Access Points. |

### Planos y diagramas

| Archivo | Representa |
|---------|-----------|
| `1 - Plano de piso tipo - cableado estructurado (solucion fisica).png` | Solución física: salidas, canalizaciones y cuarto de telecomunicaciones. |
| `2 - Topologia logica de la red (solucion logica).png` | Solución lógica: jerarquía de dos capas, núcleo redundante y segmentación por VLAN. |
| `3 - Elevacion del edificio y del rack.png` | Backbone vertical entre los cinco pisos y elevación del rack tipo. |
| `4 - Ubicacion y distribucion de los Access Points.png` | Ubicación, distribución y cobertura de los Access Points por piso. |
| `5 - Analisis economico del presupuesto.png` | Distribución del costo por categoría y comparación económica de alternativas. |

### Material complementario

Apoyo interno del grupo. **No forma parte del `.zip` de la entrega** y
corresponde a la versión extendida previa de la presentación.

| Archivo | Descripción |
|---------|-------------|
| `5b - Presentacion interactiva - Taller 1.html` | Versión interactiva de la presentación (se abre en el navegador). |
| `5c - Guion de la presentacion - Taller 1.html` | Guion de apoyo para exponer la presentación. |

## Resumen de la solución

- **960 salidas** de telecomunicaciones Categoría 6A (192 por piso).
- **15 switches** de acceso de 48 puertos PoE+ y un **núcleo redundante** de capa 3.
- **30 Access Points** WiFi 6 (6 por piso), dimensionados por criterio de capacidad.
- **Backbone** de fibra óptica multimodo OM4 de 12 hilos por piso.
- **Inversión total estimada:** $ 207.104.695 CLP ($ 517.762 por usuario).
