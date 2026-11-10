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
| Taller 2 | Comparación AWS vs. Azure y propuesta de infraestructura cloud para la empresa VAR (operación actual y expansión a cuatro estados). | [`Taller 2/`](./Taller%202) | En preparación |

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

Apoyo interno del grupo para ensayar. **No forma parte del `.zip` de la
entrega** (el docente no lista HTML entre los formatos aceptados), pero está
alineado con las mismas 10 diapositivas.

| Archivo | Descripción |
|---------|-------------|
| `5b - Presentacion interactiva - Taller 1.html` | Versión interactiva de la presentación, 10 diapositivas (se abre en el navegador). |
| `5c - Guion de la presentacion - Taller 1.pdf` | Guion slide por slide e integrante (15 páginas): 2 diapositivas y 2 minutos por persona, 10:00 en total, con la pregunta probable del docente en cada diapositiva, banco de preguntas y recomendaciones de exposición. |

### Reparto de la exposición

| Integrante | Bloque | Slides | Tiempo |
|------------|--------|--------|--------|
| Benjamín Peña | Apertura, el problema y los requerimientos | 1 – 2 | 2:00 |
| Francisco Morales | Dimensionamiento, cableado y normativas | 3 – 4 | 2:00 |
| Julián Pacheco | Arquitectura lógica y diseño físico | 5 – 6 | 2:00 |
| Martín Burgos | Red inalámbrica, backbone y segmentación | 7 – 8 | 2:00 |
| Matías Muñoz | Presupuesto y conclusiones | 9 – 10 | 2:00 |

## Resumen de la solución

- **960 salidas** de telecomunicaciones Categoría 6A (192 por piso).
- **15 switches** de acceso de 48 puertos PoE+ y un **núcleo redundante** de capa 3.
- **30 Access Points** WiFi 6 (6 por piso), dimensionados por criterio de capacidad.
- **Backbone** de fibra óptica multimodo OM4 de 12 hilos por piso.
- **Inversión total estimada:** $ 207.104.695 CLP ($ 517.762 por usuario).

## Taller 2 — Contenido de la entrega

El archivo a subir es **`GRUPO6_Trabajo2_8485.zip`**, con el formato de nombre
exigido en el enunciado (`GRUPOX_Trabajo2_8485.zip`): repositorio LaTeX
(código, figuras e imágenes) más el PDF exportado, la planilla de costos (E2) y
la presentación de la defensa (E3).

| Archivo | Descripción |
|---------|-------------|
| `GRUPO6_Trabajo2_8485.zip` | Entrega completa comprimida. |
| `Entrega2_GRUPO6_NRC8485.pdf` | Informe técnico compilado (portada, índice, 9 secciones, declaración de uso de IA, referencias APA 7 y 3 anexos). |
| `Informe LaTeX/` | Fuente del informe: `Entrega2_GRUPO6_NRC8485.tex`, `referencias.bib` (biblatex-apa) y `figuras/` (TikZ y logo). Se compila con `latexmk -xelatex`. |
| `Planilla de costos - AWS vs Azure.xlsx` | Tarifas unitarias con fuente y fecha, los dos escenarios con fórmulas (cantidad × tarifa), la Matriz comparativa 2 y la sensibilidad con reservas de 1 año. |
| `Entrega2_GRUPO6_NRC8485.html` | Presentación de la defensa: 11 diapositivas 16:9, un solo archivo (← → navegar, F pantalla completa, N notas del orador). |
| `Planos y diagramas/` | Diagramas exportados del informe. |

### Planos y diagramas

| Archivo | Representa |
|---------|-----------|
| `1 - Arquitectura propuesta en AWS (mx-central-1).png` | Arquitectura recomendada: VPC en 3 zonas, ALB + WAF, EC2 Auto Scaling, RDS PostgreSQL Multi-AZ, S3 y copia de respaldos a una región secundaria. |
| `2 - Costos mensuales por escenario.png` | Costo mensual de AWS y Azure en ambos escenarios, pagando por uso y con reserva de 1 año. |
| `3 - Cronograma de implementacion (Gantt).png` | Las 6 fases de la implementación en 16 semanas. |

### Material complementario

Apoyo interno del grupo para ensayar. **No forma parte del `.zip` de la entrega.**

| Archivo | Descripción |
|---------|-------------|
| `Guion de la presentacion - Taller 2.pdf` | Guion lámina por lámina e integrante (4 páginas): 10:00 en total, con la pregunta probable del docente en cada lámina y un banco de preguntas. |

### Reparto de la exposición

| Integrante | Bloque | Slides | Tiempo |
|------------|--------|--------|--------|
| Benjamín Peña | Apertura, caso y supuestos; cierre | 1 – 2 y 11 | 0:00 – 1:30 y 9:30 – 10:00 |
| Francisco Morales | Comparación de servicios (Matriz 1) | 3 – 4 | 1:30 – 3:30 |
| Martín Burgos | Costos en dos escenarios (Matriz 2) | 5 – 6 | 3:30 – 5:30 |
| Julián Pacheco | Arquitectura y recomendación | 7 – 8 | 5:30 – 7:30 |
| Matías Muñoz | Migración, riesgos y continuidad | 9 – 10 | 7:30 – 9:30 |

### Resumen de la propuesta

- **Supuestos:** México; hoy la CDMX y, en la expansión, Nuevo León, Jalisco, Querétaro y Puebla. De 50 a 110 empleados, de 200 a 600 cuentas, de 0,45 a 2 TB y de 60.000 a 200.000 transacciones al mes. 99,9 %, RPO 15 min y RTO 4 h.
- **Costos** (regiones de México, USD, pago por uso, 10-11-2026): AWS US$ 489/mes hoy y US$ 1.033 en la expansión; Azure US$ 555 y US$ 1.169. Con reserva de 1 año la diferencia baja a ~1 %.
- **Recomendación:** AWS en `mx-central-1` como proveedor único (matriz ponderada 4,80 frente a 4,30), sobre todo por la continuidad: Mexico Central no tiene región pareada para el geo-respaldo de PostgreSQL en Azure.
- **Implementación:** migración por etapas con replicación (DMS + DataSync) en 16 semanas, 8 riesgos con mitigación, rollback de 2 h y 7 KPI.
