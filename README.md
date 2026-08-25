# DiplomadoIA2026C3

Scripts del Diplomado IA preparados para ejecutarse en el entorno Conda
`DiplomadoIA`, sin Docker.

## Preparación

```bash
conda env update -f environment.yml
conda activate DiplomadoIA
cp secrets/.env.example secrets/.env
```

Completa `secrets/.env` con las credenciales. `TensorialBase.py` construye o
sobrescribe la base Deep Lake a partir de `Anillos.pdf`; los programas de
consulta usan `deeplake_db/anillos`.

Los scripts se pueden lanzar desde cualquier directorio porque sus rutas se
resuelven con base en la ubicación del propio proyecto.
