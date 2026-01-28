# Modelo de Datos: Cómics y Personajes

## Elementos elegidos
- **comic**: Representa una obra de cómic.
- **personaje**: Representa un personaje dentro de un cómic.

## Características
### Comic
- `id`: Identificador único (ID)
- `publicado`: Si se ha publicado (opcional)
- `titulo`: Nombre del cómic
- `autor`: Autor del cómic

### Personaje
- `id`: Para definir el personaje (ID)
- `ref`: Para referenciarlo desde un cómic (IDREF)
- `nombre`: Nombre del personaje
- `rol`: Papel dentro del cómic (opcional)

## Relaciones
- Un `comic` puede tener varios `personajes`.
- Cada `personaje` dentro de un `comic` hace referencia (`IDREF`) a un `personaje` definido con `id`.
- Se usa `ID` y `IDREF` para garantizar integridad referencial.

## Opcionalidad
- `imagen`: Puede no aparecer.
- `rol` y `descripcion`: Atributos opcionales.
