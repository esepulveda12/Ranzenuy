# Migracion de home a Shopify Liquid

Se creo una version de la home en formato Shopify Online Store 2.0 usando secciones y bloques editables.

## Archivos creados

- sections/ranzen-home-conversion.liquid
- templates/page.ranzen-home.json
- sections/ranzen-collection-conversion.liquid
- templates/collection.ranzen.json
- sections/ranzen-product-conversion.liquid
- templates/product.ranzen.json
- sections/ranzen-blog-conversion.liquid
- templates/blog.ranzen.json
- sections/ranzen-article-conversion.liquid
- templates/article.ranzen.json

## Como usar en tu tema Shopify

1. Copia el archivo sections/ranzen-home-conversion.liquid dentro de la carpeta sections de tu tema.
2. Copia el archivo templates/page.ranzen-home.json dentro de templates.
3. En Shopify Admin, crea una pagina (por ejemplo Home Ranzen).
4. Asigna la plantilla page.ranzen-home a esa pagina.
5. Para categorias/colecciones, asigna collection.ranzen en cada coleccion.
6. Para productos, asigna product.ranzen en los productos que quieras migrar.
7. Para blog, asigna blog.ranzen en el blog principal.
8. Para notas de blog, asigna article.ranzen en los articulos.
9. Abre el editor de temas y configura:
   - logo
   - links del menu
   - chips de categorias
   - slides del hero
   - coleccion destacada

## Importante

- Esta conversion reemplaza logica de WordPress (Elementor, WooCommerce, plugins) por objetos nativos de Shopify.
- Los links de categorias, productos e imagenes se deben volver a conectar en el editor.
- Si quieres una migracion 1:1 de cada modulo original, hay que crear secciones adicionales por cada bloque del sitio original.
- Los nombres de plantillas .json pueden variar segun tu tema; si Shopify no permite uno, se puede renombrar sin afectar la logica.
