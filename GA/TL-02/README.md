# GA-TL-02 - FORM · Taller de entrevista estructurada y design thinking

**ISR-401 · UTEQ · Software 4.º nivel · SPA 2026–2027**

**PFC:** Plataforma de ventas con módulo de recomendación basado en IA para establecimientos eléctricos.

## Equipo

- Cedeño Avila Winston Damian
- Paca Pilataza Luis Alberto
- Rivera Suarez Jonathan Javier

## Estructura

- `main.tex`: archivo principal.
- `referencias.bib`: referencias en estilo IEEE.
- `figuras/`: mapa de empatía (PNG y fuente editable).
- `evidencias/manifiesto.md`: nombre, fecha, duración y SHA-256 de las evidencias del ensayo. Los originales no se publican.

## Compilación

Requisitos: TeX Live 2023 o superior (o MiKTeX) con `IEEEtran`, `biblatex` (estilo `biblatex-ieee`), `biber`, `babel` (español), `csquotes`, `booktabs`, `tabularx`, `graphicx`, `hyperref` y `xurl`.

Desde la carpeta `GA/TL-02`:

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

Resultado: `main.pdf`.
