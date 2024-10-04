# DIGIFRAMEWORK

Repositorio para crear un framework para Diseño de Interfaces Web (DIW) de 2º de DAW.

### Colaboradores:
David Peñalver <br>
Vanessa Esteve <br>
Alex Almohano <br>
Javier Fernández <br> <br>

### Estructura:

```plaintext
01 utilities/
  ├── _colors.scss
  ├── _variables_sass.scss

02 base/
  ├── _reset.scss
  ├── _fonts.scss

03 layout/
  ├── _l-columns.scss
      ├── _l-columns–1.scss
      ├── _l-columns–2.scss
      ├── _l-columns–3.scss
      ├── _l-columns–4.scss
      ├── _l-columns–5.scss
      ├── _l-columns–6.scss
      ├── _l-columns–7.scss
      ├── _l-columns–8.scss
      ├── _l-columns–9.scss
      ├── _l-columns–10.scss
      ├── _l-columns–11.scss
      ├── _l-columns–12.scss
  ├── _l-flex.scss
      ├── _l-flex–direction–row.scss
      ├── _l-flex–direction–column.scss
      ├── _l-flex–wrap–wrap.scss
      ├── _l-flex–wrap-no-wrap.scss
      ├── _l-justify-content–flex-start.scss
      ├── _l-justify-content–flex-end.scss
      ├── _l-justify-content–center.scss
      ├── _l-justify-content–space-between.scss
      ├── _l-justify-content–space-around.scss
      ├── _l-justify-content–space-evenly.scss
      ├── _l-align-items–flex-start.scss
      ├── _l-align-items–flex-end.scss
      ├── _l-align-items–center.scss
      ├── _l-align-items–stretch.scss
      ├── _l-align-items–baseline.scss
      ├── _l-flex-grow–X.scss
      ├── _l-flex-shrink.scss
      ├── _l-flex-basis.scss

04 components/
  ├── _c-button.scss
  ├── _c-ul.scss
  ├── _c-ol.scss
  ├── _c-nav.scss
  ├── _c-aside.scss
  ├── _c-main.scss
  ├── _c-img.scss
  ├── _c-video.scss
  ├── _c-form.scss
      ├── _c-form–input.scss
      ├── _c-form-label.scss
  ├── _c-block-quote.scss
      ├── _c-block-quote–text.scss
      ├── _c-block-quote–img.scss
  ├── _c-separator.scss
  ├── _c-text.scss
      ├── _c-text–align-center.scss
  ├── _c-title.scss
      ├── _c-title–size-xxl.scss
      ├── _c-title–size-xl.scss
      ├── _c-title–size-l.scss
      ├── _c-title–size-m.scss
      ├── _c-title–size-s.scss
      ├── _c-title–size-xs.scss
  ├── _c-badge.scss  // Incluye estilos para color, bg, y height

05 pages/
  // Aquí se incluirán estilos específicos de las páginas, si es necesario.

06 global/
  ├── _g-padding.scss
      ├── _g-padding–left.scss
      ├── _g-padding–right.scss
      ├── _g-padding–bottom.scss
      ├── _g-padding–top.scss
      ├── _g-padding–vertical.scss
      ├── _g-padding–horizontal.scss
  ├── _g-margin.scss
      ├── _g-margin–left.scss
      ├── _g-margin–right.scss
      ├── _g-margin–bottom.scss
      ├── _g-margin–top.scss
  ├── _g–height.scss
  ├── _g–width.scss
  ├── _g–border.scss
      ├── __g-border–type-dotted.scss
      ├── __g-border–type-dashed.scss
      ├── __g-border–type-solid.scss
      ├── __g-border–type-double.scss
      ├── __g-border–type-groove.scss
      ├── __g-border–type-ridge.scss
      ├── __g-border–type-inset.scss
      ├── __g-border–type-outset.scss
      ├── __g-border–type-none.scss
      ├── __g-border–type-hidden.scss
      ├── __g-border–color-X.scss
      ├── __g-border–radius-X.scss
      ├── __g-border–size-X.scss
  ├── _g-color.scss
  ├── _g-background-color.scss
  ├── _g-font.scss
      ├── _g-font–size.scss
      ├── _g-font–family.scss
      ├── _g-font–weight.scss
  ├── _g-justify.scss
      ├── _g-justify–left.scss
      ├── _g-justify–center.scss
      ├── _g-justify–right.scss
```

### Explicación del Framework:

1. **Estructura de carpetas y archivos**:
   - **01 utilities**: Aquí se guardan todas las variables, colores, y configuraciones globales que serán utilizadas a lo largo del proyecto, como `variables_sass` y `colors`.
   - **02 base**: Archivos que son esenciales para dar un punto de partida, como el `reset.scss` y las configuraciones de fuentes (`fonts.scss`).
   - **03 layout**: Archivos relacionados con el diseño y disposición del contenido. Incluye configuraciones de columnas (`_l-columns`) y de flexbox (`_l-flex`).
   - **04 components**: Componentes reutilizables, como botones, listas (`_ul`, `_ol`), formularios, etc.
   - **05 pages**: Estilos específicos para cada página si se necesita una personalización a nivel de vista.
   - **06 global**: Contiene utilidades globales que se aplican a múltiples partes del proyecto, como márgenes, padding, y propiedades de fuente y borde.

2. **Nombres y BEM**:
   - Se sigue un sistema de nombres similar a BEM, que facilita la lectura y entendimiento de los estilos. 
   - Los prefijos como `_g-`, `_c-`, `_l-` ayudan a diferenciar fácilmente si se trata de un componente global, de un layout o un componente específico.

3. **Archivos Desglosados**:
   - Para componentes como `flex` y `columns`, cada opción de configuración se desglosa en un archivo separado, facilitando la modularidad y el mantenimiento del código.
   - Los archivos `_l-flex–direction–row.scss` o `_l-columns–1.scss` son específicos y hacen que los estilos sean fáciles de modificar y entender.

4. **Modularidad**:
   - Tener todos los estilos divididos en archivos específicos ayuda a mantener un proyecto escalable y organizado.
   - Los nombres específicos permiten importar solo las partes que se necesiten, mejorando la performance.

