# Bakatá Shopify Theme

Theme de Shopify versionado para el desarrollo frontend de Bakatá.

## Themes de Shopify

- `Horizon` (`188889530592`): theme publicado actual. No debe modificarse desde este flujo.
- `Bakata Development` (`188891726048`): theme no publicado para pruebas y previews.

## Development workflow

1. Trabajar en la rama `develop`.
2. Ejecutar `git push origin develop`.
3. Shopify debe actualizar el theme de desarrollo conectado a esa rama.
4. Revisar el preview del theme no publicado.
5. Ejecutar `shopify theme check` antes de solicitar revisión.
6. Crear un Pull Request de `develop` hacia `main`.
7. Revisar y aprobar el Pull Request.
8. Hacer merge a `main` después de la aprobación.
9. Publicar manualmente en Shopify únicamente tras la validación final.

Ningún merge o push debe publicar automáticamente el theme de producción. `Horizon` permanece protegido como producción actual; `Bakata Development` es exclusivamente para pruebas.

## Shopify CLI

La tienda objetivo para la CLI es `0djnem-9x.myshopify.com`. No se guardan tokens, credenciales ni archivos de sesión en este repositorio.
