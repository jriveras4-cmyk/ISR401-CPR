# GA-TL-02 - FORM · Taller de entrevista estructurada y Design Thinking

**ISR-401 · UTEQ · Software, 4.º nivel «B» · SPA 2026–2027**

**PFC de referencia:** Plataforma de punto de venta (POS) con módulo de recomendación para establecimientos eléctricos.

## Equipo CPR

- Cedeño Avila Winston Damian
- Paca Pilataza Luis Alberto
- Rivera Suarez Jonathan Javier

## Documentos

- `main.tex`: guion y documento principal de la actividad (en desarrollo).
- `referencias.bib`: referencias para el informe principal, en formato IEEE.
- `consentimiento_informado.tex`: fuente LaTeX del protocolo de consentimiento, de una carilla.
- `consentimiento_informado.pdf`: formulario **en blanco** de una página A4, con encabezado institucional, separadores dorados y tabla verde, compilado desde LaTeX.
- `figuras/`: mapa de empatía y fuente editable (pendientes).
- `evidencias/manifiesto.md`: plantilla de registro de fecha, duración y SHA-256 del audio; completar **solo después** del ensayo.

El formulario es para el **roleplay académico de aproximadamente 10 minutos**. Explica el propósito, la participación voluntaria, la opción separada de grabar audio, el tratamiento de las notas y el derecho a retirarse. No incluye datos de una empresa, cliente o participante real.

**No se publicarán en este repositorio versiones firmadas, audios ni datos identificables.** Los originales, cuando existan, deberán conservarse en un espacio institucional privado accesible al docente. El formulario en blanco sí puede estar en GitHub.

## Compilación del informe principal

Se necesita TeX Live o MiKTeX con `IEEEtran`, `biblatex` (estilo `ieee`), `biber`, `babel` para español, `csquotes`, `booktabs`, `tabularx`, `graphicx`, `hyperref` y `xurl`.

Desde `GA/TL-02`:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

**El archivo `main.pdf` todavía no figura en el repositorio y debe compilarse y revisarse cuando se completen las secciones faltantes.**

## Compilación independiente del consentimiento

Desde la misma carpeta:

```bash
pdflatex -interaction=nonstopmode -halt-on-error consentimiento_informado.tex
```

El resultado es `consentimiento_informado.pdf` (una página A4). Este formulario independiente no sustituye el `main.pdf` requerido para el cierre de la actividad.

## Pendiente para terminar GA-TL-02

- Realizar y documentar el ensayo de entrevista con consentimiento real.
- Elaborar el mapa de empatía a partir de las respuestas obtenidas.
- Redactar el problema centrado en el usuario («¿Cómo podríamos ...?»).
- Registrar las preguntas defectuosas y sus versiones corregidas.
- Completar el manifiesto con datos y hash auténticos, guardar las pruebas originales en privado y generar `main.pdf` desde LaTeX.
- Revisar la declaración de uso de IA en el documento principal para que describa con exactitud la asistencia recibida.

**Cierre indicado en la guía del PDF:** sábado 21 de noviembre de 2026 a las 23:59. Verificar las indicaciones vigentes del SGA del paralelo B.
