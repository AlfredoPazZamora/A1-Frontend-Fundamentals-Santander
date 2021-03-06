# Grid con 3 columnas iguales

## REQUISITOS
- Tener Git Bash si usas Windows.
- Tener conocimientos de CSS (Flexbox)

## INSTRUCCIONES

Queremos indicar que nuestra grid va a contener 3 columnas del mismo ancho 
relativo al espacio disponible en la pantalla. ¿Cómo lo lograrías usando la 
función `repeat(cantidad, tamaño)`?

<details>
  <summary>Posible Solución</summary>

```css
.features {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

</details>







# Grid 2 filas con alto de `330px`

## REQUISITOS
- Tener Git Bash si usas Windows.
- Tener conocimientos de CSS (Flexbox)
- Conocer el modelo de caja 

## INSTRUCCIONES

Regresa la cantidad de columnas a las que realmente necesitamos (2) y agrega
la cantidad de filas que usaremos (2) teniendo en cuenta que el alto será de
`330px`. Una vez logrado, ¿cómo se te ocurre que podrías usar la unidad de `fr`
para indicar el alto de las filas?

<details>
  <summary>Posible Solución</summary>

```css
.features {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 330px);
}
```

Una forma de poder usar la unidad `fr` para asignar el alto de las filas sería
indicando un tamaño fijo al elemento contenedor, en nuestro caso, podríamos 
hacer:

```css
.features {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  height: 660px;
  grid-template-rows: repeat(2, 1fr);
}
```

</details>

