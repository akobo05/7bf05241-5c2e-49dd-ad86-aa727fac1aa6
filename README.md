# Fotos de catálogo

Alojamiento de las fotos de producto que consume el asistente de WhatsApp (Shoppy).
La columna `url_imagen` de la plantilla de importación apunta a los enlaces `raw` de este repo.

## Cómo se arma un enlace

```
https://raw.githubusercontent.com/akobo05/fotos-catalogo-apple/main/NOMBRE-DEL-ARCHIVO.jpg
```

## Reglas de nombres

- Solo minúsculas, números y guiones. **Nunca** espacios, tildes ni paréntesis: rompen la URL.
- El nombre describe el producto, no la unidad física.
- Galerías: sufijo numerado, y la `01` es siempre la foto principal (la que va en `url_imagen`).

## Actualizar una foto

Reemplazá el archivo conservando **el mismo nombre**, y hacé commit y push. El enlace no cambia,
así que no hay que volver a importar el catálogo en Shoppy.

```bash
git add -A && git commit -m "Actualiza foto X" && git push
```

## Contenido actual

| Archivo | Producto | SKU |
|---|---|---|
| `iphone-17-pro-max-1tb-cosmic-orange.jpg` | iPhone 17 Pro Max 1TB Cosmic Orange | `APP-IP17PM-1TB-CO` |
| `iphone-17-pro-max-1tb-deep-blue.jpg` | iPhone 17 Pro Max 1TB Deep Blue | `APP-IP17PM-1TB-DB` |
| `iphone-17-pro-max-1tb-silver.jpg` | iPhone 17 Pro Max 1TB Silver | `APP-IP17PM-1TB-SI` |
| `iphone-17-pro-max-512gb-silver-openbox-01..09` | iPhone 17 Pro Max 512GB Silver Open Box (galería de 9) | `APP-IP17PM-512-SI-OB` |

## Pendiente

Faltan fotos de: AirPods 4, AirPods Max 2, Apple Watch S11 42mm y Apple Watch S11 46mm.
