# CLAUDE.md — Guía del proyecto (léeme primero)

Este repositorio documenta y soporta la operación de **flipping inmobiliario** en
Colombia (compra, remodelación y reventa de inmuebles). Aquí guardamos
certificados, análisis jurídicos, minutas y plantillas para **perfeccionar cada
vez más nuestras promesas y contratos**.

> ⚠️ **Disclaimer permanente:** todo lo de este repo es **apoyo informativo, NO
> asesoría legal ni tributaria**. Cada documento es un **borrador** que debe
> revisar un abogado/notaría/contador. Incluir siempre este aviso en los
> documentos generados.

## Idioma y contexto
- Todo en **español** (Colombia). Marco legal: Código Civil (C.C.), Código de
  Comercio (C.Co), Estatuto Tributario (E.T.), Ley 1579/2012 (registro),
  Ley 258/1996 (afectación), Ley 70/1931 (patrimonio de familia),
  Ley 1537/2012 (VIS/VIP).

## Cómo está organizado el repo
- `TABLERO.md` → **la foto de todo**: semáforo por apartamento, pendientes con
  fecha y dueño, el reloj (días corridos y **fecha límite para publicar en
  venta**), plata y riesgos. **Abrirlo primero en cada sesión y actualizarlo
  cada viernes.**
- `flipping-NN-<nombre-corto>/` → una carpeta por operación. Dentro:
  - `seguimiento.md` — ficha viva del apto: reloj, papeles, plata, riesgos,
    próximas acciones y bitácora (plantilla: `plantillas/09-...`).
  - `certificado-tradicion-<matricula>.md` — transcripción del folio.
  - `analisis-juridico-y-saneamiento.md` — limitaciones y cómo levantarlas.
  - `tributario-y-estructuracion.md`, `modelo-margen-y-renta.md` — números e impuestos.
  - `evitar-doble-escrituracion.md` — estructura de cesión.
  - minutas y `*-DEFINITIVO.docx` — documentos para firmar/revisar.
- `plantillas/` → versiones **genéricas y reutilizables** (úsalas como punto de
  partida para cada nuevo flip).
- `base-conocimiento-legal.md` → el "qué aprendimos" condensado, con artículos.
- `codigo_civil_colombia.txt` → copia parcial (solo título preliminar).

## Flujo de trabajo (git)
- Rama de desarrollo: `claude/relaxed-mccarthy-84zrkd`.
- Tras cada cambio: **commit + push** a esa rama (con reintentos si falla la red).
- No crear PR salvo que la usuaria lo pida.

## Convenciones al redactar documentos
1. Empezar con el **disclaimer** de borrador.
2. **Campos por completar** entre corchetes `[ ]`.
3. Identificar el inmueble por **matrícula** + descripción (torre/apto/área/coef.).
4. Para minutas de **venta/poder de inmuebles**: siempre **escritura pública**
   (no autenticado).
5. Entregar en **Word** cuando se pida (ver "Herramientas del entorno").

## Playbook estándar de un flip (orden recomendado)
1. **Certificado de tradición** → transcribir y revisar **anotaciones**
   (limitaciones al dominio).
2. **Sanear el folio** antes de escriturar:
   - VIP/subsidio (Ley 1537/2012): registrar el **retiro/autorización de ISVIMED**
     (prohibición de transferencia 10 años + derecho de preferencia).
   - **Patrimonio de familia**: cancelación **notarial** si los hijos son mayores;
     **judicial** (juez de familia) si hay menores.
   - **Afectación a vivienda familiar**: levantamiento por **escritura** con ambos
     cónyuges/compañeros; **judicial** si uno no comparece. ⚠️ Revisar el **estado
     civil** vs. el beneficiario que figura en el folio.
3. **Promesa de compraventa** robusta (ver `plantillas/00-checklist-promesa…`).
4. Si el vendedor no puede asistir: **poder especial por escritura pública**.
5. Para evitar **doble escrituración**: **cesión de posición contractual**
   (una sola escritura) — declarando el margen.
6. **Escriturar y registrar** en la ORIP; sacar **certificado nuevo** limpio.

## Ritmo de seguimiento (para no perder el hilo)
- **Cada viernes:** actualizar `TABLERO.md` + la `seguimiento.md` de cada flip
  (mover ⬜→✅, re-fechar lo que se corrió, subir a 🔴 lo que lleve 2 semanas
  quieto) y hacer **commit + push**.
- **Regla del reloj:** objetivo de **150 días** entre promesa de compra y
  escritura de venta. Comercializar toma **45–60 días** → el apto debe estar
  **publicado 60 días antes** de la fecha de venta objetivo. Esa es la fecha que
  más se vigila.
- **Firmado ≠ registrado:** en las fichas hay dos casillas separadas; el folio
  solo queda limpio con la **inscripción en la ORIP** (guardar el nº de turno).

## Checklist por operación
- [ ] Ficha `seguimiento.md` creada desde `plantillas/09-ficha-seguimiento-flip.md`
      y fila añadida en `TABLERO.md`.
- [ ] Certificado de tradición transcrito y anotaciones analizadas.
- [ ] Limitaciones identificadas (VIP/ISVIMED, patrimonio, afectación, embargos).
- [ ] Plan de saneamiento con responsables y fechas.
- [ ] Promesa/otrosí con: precio, forma de pago, arras/cláusula penal, entrega,
      **saneamiento como condición**, paz y salvos, **reparto de gastos**,
      facultad de **designar tercero/cesión**.
- [ ] Poder (si aplica) por escritura pública, blindado.
- [ ] Estructura tributaria definida (PN vs SAS; cesión vs doble escritura).
- [ ] Soportes de costos (facturas de remodelación) archivados.

## Aprendizajes clave (resumen — detalle en `base-conocimiento-legal.md`)
- **Tracto sucesivo** (Ley 1579/2012 art. 3 f): solo el **titular inscrito**
  enajena → en la cesión, vende el vendedor original al tercero (una escritura).
- **Las anotaciones solo se cancelan al REGISTRAR** en la ORIP, no al firmar.
- **Poder irrevocable**: posible si se confiere **también en interés del
  apoderado** (Art. 1279 C.Co); pero el civil **se extingue con la muerte**
  (Art. 2189 C.C.) salvo pacto mercantil de **subsistencia** (Art. 1280 C.Co).
  Autocontratación requiere **autorización expresa** (Art. 2170 C.C. / 838 C.Co).
- **Flipping = renta ordinaria** (inventario, <2 años), no ganancia ocasional.
  Persona natural aprovecha el **0% hasta 1.090 UVT** (tabla Art. 241 E.T.).
- **Remodelación = costo** que baja el impuesto, **solo con título + facturas**.
- **Habitualidad** (varios flips) → **comerciante**: matrícula mercantil,
  contabilidad, revisar **ICA**. A volumen moderado, **PN paga menos que SAS**;
  la SAS se justifica por **protección patrimonial**, no por impuestos.
- **No** ayudar a esconder el margen (evasión/simulación). Sí optimizar **costos
  transaccionales** legalmente (cesión).

## Herramientas del entorno (tips para sesiones futuras)
- **Leer PDFs**: usar `pdfminer.six`. Si falla con `_cffi_backend`, correr
  `pip install --force-reinstall cffi` y reintentar. (No hay poppler.)
- **Markdown → Word**: hay `python-docx` (instalar con pip) y `libreoffice`.
  Existe un convertidor reutilizable en `/tmp/md2docx.py` (recrearlo si el
  contenedor se recicló): maneja títulos, negritas, tablas, listas y citas.
