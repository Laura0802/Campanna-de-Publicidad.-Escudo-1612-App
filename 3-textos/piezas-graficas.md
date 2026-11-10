# Piezas gráficas — Escudo 1612

Doce piezas listas para publicar. Formato **PNG** para subir directamente y **SVG** para editar
o reutilizar.

## Qué hay

| Archivo | Tamaño | Uso |
|---|---|---|
| `reel-01-espejo.png` | 1080×1920 | Portada del reel del lunes (día 1) |
| `carrusel-d04-01…07.png` | 1080×1080 | Carrusel de las seis violaciones (día 4) |
| `estatico-cita-1612.png` | 1080×1080 | Estático con la cita (día 4 o refuerzo) |
| `reel-08-fuentes.png` | 1080×1920 | Portada del reel de cierre (día 8) |
| `historia-recordatorio.png` | 1080×1920 | Historia con botón (uso diario) |
| `tarjeta-enlace.png` | 1200×630 | Miniatura para el enlace en X y LinkedIn |

En `preview/` están las mismas piezas a 720 px, solo para revisarlas rápido.

## Sistema visual

- **Fondo papel `#F7F5F1`**, nunca negro. Retícula muy tenue, marca de agua del escudo al 2,8 %.
- **Tinta `#1F4568`** para titulares. Texto secundario `#5B7893`.
- **Acentos**: azul `#0B7FB8`, cian `#00B9FF`, verde `#0F7B4F`, rojo `#B42318`, ámbar `#B8651A`,
  morado `#7A4FBF`. Cada diapositiva usa **un** acento, nunca varios.
- **Tipografía**: Sora (titulares) y JetBrains Mono (etiquetas y pies). Si no están instaladas,
  cae a Segoe UI y Consolas sin romper la composición.
- **El escudo** aparece tres veces como marca: cabecera (44 px), portada de reel (210 px) y
  sello en la historia (230 px). Siempre con el mismo archivo `assets/logo-mark.png`, ya recortado
  y con fondo transparente.

## Estructura fija

Todas las piezas comparten la misma retícula, y eso es lo que hace que la cuenta se vea coherente:

1. **Cabecera**: escudo + `ESCUDO 1612` + `CONSEJO DE SEGURIDAD · ONU`, con la etiqueta de la
   pieza a la derecha (`REEL · 25 S`, `03/07`).
2. **Antetítulo** en mono, versalitas y mucho interletraje.
3. **Titular** grande, dos o tres líneas como máximo, con barra de acento vertical.
4. **Cuerpo** corto, 29 px.
5. **Pie**: URL + firma.

## Zonas seguras

- **Reels e historias**: deja libres los **220 px superiores** y los **250 inferiores**. Ahí van la
  barra de progreso, el usuario y el cajón de respuesta. El contenido importante va en el centro.
- **Cuadrícula del perfil**: recorta a cuadrado desde el centro. Los titulares están dentro del
  80 % central para que no se corten.

## Cómo editar

**Cambiar un texto suelto:** abre el `.svg` con un editor de texto (Bloc de notas, VS Code), busca
la frase y cámbiala. Los SVG son texto plano; no necesitas Illustrator.

**Cambiar todo el carrusel:** edita el array `carrusel` en `tools/gen-piezas.mjs` y ejecuta:

```bash
node tools/gen-piezas.mjs
```

Se regeneran los 12 SVG y sus PNG en `campana/piezas/`.

**Si tocas los colores**, están todos en el objeto `C` al principio del mismo archivo. Cámbialo
ahí y no pieza por pieza.

## Antes de subir

- [ ] El texto cabe y no se corta en la vista previa del móvil.
- [ ] La primera diapositiva del carrusel se entiende sola: es la que decide si deslizan.
- [ ] No hay dos acentos distintos en la misma pieza.
- [ ] El escudo no queda tapado por la interfaz de la plataforma.
- [ ] En historias, el botón de enlace va por encima del área del CTA de la imagen.
