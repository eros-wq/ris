# RIS

Sitio de consulta de reportes, propuestas y plan de acción de Meta Ads para RIS.

## Contenido

- `index.html`: página principal.
- `reporte-semanal.html`: reporte semanal de Meta con filtro de fechas, frente a las metas del flow.
- `flow-general.html`: propuesta del flow general de medios, octubre 2026 a junio 2027.
- `ris-meta-credit-action-plan.html`: informe y plan de acción.
- `data/ris_meta_daily.js`: datos diarios de Meta que lee el reporte semanal.
- `assets/`: recursos visuales y estilos del sitio.

## Uso local

Abre `index.html` en un navegador para acceder al informe.

## Convención de nombres

Los archivos de contenido usan `kebab-case`. Los documentos estándar de GitHub conservan sus nombres convencionales, por ejemplo `README.md`.

## Actualizar el reporte semanal

Los datos se generan desde el repositorio Meta-Ads-CLI:

```
.venv/bin/python scripts/clients/ris/build_ris_weekly.py --out ../GitHub/ris/data/ris_meta_daily.js
```
