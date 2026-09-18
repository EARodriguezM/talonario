# Talonario para Yera

Una página de cumpleaños: una nota, tres boletas y una P.D.
En vivo en <https://earodriguezm.github.io/talonario/>.

## Revelar una sorpresa

Las boletas **Nº 002** y **Nº 003** están en papel kraft con el sello
*Pendiente*. Cuando llegue el momento de una, abre `index.html`, busca su
`<article>` y cambia cuatro cosas:

| qué | de | a |
|---|---|---|
| el papel | `class="ticket kraft"` | `class="ticket papa"` |
| el sello | `<span class="stamp esperando">Pendiente</span>` | `<span class="stamp lista">Válida ya</span>` |
| el nombre | `<h2 class="title">Sorpresa</h2>` | el regalo de verdad |
| el texto | `<p class="what">` y `<p class="fine">` | de qué se trata y la letra menuda |

Deja el título corto (una o dos palabras): está en una tipografía grande y en
un teléfono se parte feo si es largo.

Después:

```bash
git commit -am "revelada la 002"
git push
```

GitHub Pages republica en ~1 minuto. Si no tienes el repo a mano, también
puedes editar `index.html` directamente en github.com con el lápiz.

## Archivos

- `index.html` — la página completa, con el CSS dentro. Sin dependencias
  aparte de las tipografías de Google.
- `preview.png` — la tarjeta que aparece al pegar el link en WhatsApp
  (1200×630). Si cambias mucho la página, vale la pena regenerarla.

Tipografías: Alfa Slab One en los títulos, Fraunces en la nota y la P.D.,
Courier Prime en los seriales y la letra menuda. La página lleva
`robots: noindex`, así que no sale en buscadores; el link hay que pasarlo.
