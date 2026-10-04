# Bakatá Shopify Theme

Theme de Shopify versionado para el desarrollo frontend de Bakatá.

## Themes de Shopify

- `Horizon` (`188889530592`): theme publicado actual en producción. No se modifica directamente desde este flujo.
- `bakata-shopify-theme/main` (`188891922656`): theme no publicado conectado a la rama `main`.
- `bakata-shopify-theme/develop` (`188891988192`): theme no publicado conectado a la rama `develop`; es el entorno principal de desarrollo y preview.
- `Bakata Development` (`188891726048`): theme no publicado independiente/auxiliar. No es el destino principal del flujo GitHub.

## Development workflow

1. Trabajar en la rama `develop`.
2. Hacer commit y push a `develop`.
3. Shopify sincroniza automáticamente los cambios con `bakata-shopify-theme/develop`.
4. Revisar el preview del theme no publicado.
5. Ejecutar `shopify theme check` antes de solicitar revisión.
6. Crear un Pull Request de `develop` hacia `main`.
7. Revisar y aprobar el Pull Request.
8. Hacer merge a `main`.
9. Shopify sincroniza `main` con `bakata-shopify-theme/main`.
10. Publicar manualmente en Shopify únicamente tras la validación final.

Ningún push o merge debe publicar automáticamente el theme de producción. `Horizon` permanece como producción hasta que se decida publicar manualmente el theme conectado a `main`.

## Shopify CLI

La tienda objetivo para la CLI es `0djnem-9x.myshopify.com`. No se guardan tokens, credenciales ni archivos de sesión en este repositorio.
