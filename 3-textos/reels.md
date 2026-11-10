# Reels — Escudo 1612

Dos reels montados, listos para subir. Sin fondo negro: los planos oscuros usan el azul profundo
de la app (`#12395E`) y los claros el papel (`#F7F5F1`).

## Archivos

| Archivo | Duración | Tamaño | Uso |
|---|---|---|---|
| `reel-01-espejo.mp4` | 25 s | 0,29 MB | Día 1 · «¿Y si fuera tu hijo?» |
| `reel-08-fuentes.mp4` | 20 s | 0,19 MB | Día 8 · «Nada de esto es inventado» |

Los dos son **1080×1920 (9:16 exacto), 30 fps, H.264, con audio AAC original**.

## Música

Compuesta y sintetizada para estos reels, así que **es tuya**: no hay reclamación de copyright ni
dependes de la biblioteca de Instagram.

| Reel | Composición | Carácter |
|---|---|---|
| 1 | La menor, 80 bpm. Apertura con una nota grave y pad; arpegio suspensivo en la pregunta; Do mayor cuando aparece el escudo; pulso y bajo al entrar la determinación; descenso a Re menor en la duda; Fa mayor en la subida; cierre en **La mayor** (tercera picarda) con campana | Tensión que se resuelve en alivio |
| 8 | Do mayor. Ostinato de piano, bajo y campana al enumerar las resoluciones, melodía en la segunda mitad, vacío antes del cierre y acorde final con campana | Sereno y documental |

La música está escrita **por cues**: cada cambio de plano del vídeo coincide con un cambio armónico o
rítmico. No es un fondo continuo, es una banda sonora que respira con la imagen. Instrumentos
sintetizados: piano aditivo, pad de cuerdas, bajo, pulso, shaker y campana.

Niveles medidos: pico **−1,7 dB** en los dos, media **−17,9 dB** (reel 1) y **−14,9 dB** (reel 8).

**No le añadas música de Instagram encima:** se mezclaría con la tuya y sonaría a barullo. Si
prefieres usar audio en tendencia por alcance, silencia este o vuelve a exportar el reel sin audio
— pero entonces pierdes el control del tono y la música cambia según el país.

Portadas: `piezas/reel-01-espejo.png` y `piezas/reel-08-fuentes.png`.

## Estructura del reel 1 (25 s)

| Entrada | Qué se ve |
|---|---|
| 0,0–2,2 | Fondo azul. Antetítulo: `UNA PREGUNTA INCÓMODA` |
| 2,2–6,6 | `¿Y si el niño del que habla la ONU fuera tu hijo?` · 74 px, tres líneas |
| 6,6–9,8 | Papel. Escudo + `Existe un grupo del Consejo de Seguridad dedicado solo a esto` |
| 9,8–13,2 | Azul. `DESDE 2005` + `Se llama Escudo 1612` |
| 13,2–18,0 | Papel. `No vas a arreglar el mundo en 25 segundos` / `Pero puedes entender cómo se decide` |
| 18,0–21,2 | Azul. Escudo + `Gratis. Sin registro. Sin conexión.` |
| 21,2–25,0 | Papel. Cierre de marca: escudo, `ESCUDO 1612`, URL |

Los tres primeros segundos son deliberadamente sobrios: solo texto sobre azul. Es el gancho, y
funciona porque no promete nada todavía.

## Estructura del reel 8 (20 s)

| Entrada | Qué se ve |
|---|---|
| 0,0–3,0 | `Nada de esto es inventado` + escudo |
| 3,0–7,6 | `RESOLUCIONES DEL CONSEJO DE SEGURIDAD` · `1539 · 1612 · 1882 · 1998` |
| 7,6–12,0 | `Cada dato remite a un documento oficial` |
| 12,0–16,2 | `No es una opinión sobre la guerra` / `Es el marco legal que la ONU se dio a sí misma` |
| 16,2–20,0 | Cierre de marca + URL |

## Cómo publicarlos

1. Sube el `.mp4` como reel desde la app de Instagram.
2. **Portada**: elige la imagen `reel-01-espejo.png` / `reel-08-fuentes.png` en «Editar portada».
3. **Audio**: ya va incluido. No añadas música de Instagram encima.
4. **Texto**: usa el que está en `piezas-y-enlaces.md` (ya lleva el enlace y los hashtags).
5. **Enlace**: en el pie, «enlace en la biografía», o sticker de enlace si lo publicas también
   como historia.

## Lo que estos reels no tienen

**No hay grabación de pantalla de la app.** Estos dos son tipográficos: el mensaje va en el texto,
no en la interfaz. Si quieres mostrar la app en movimiento, graba 4–6 segundos de pantalla del
simulador y móntalos entre las entradas 3 y 4 del reel 1, en CapCut o en el editor de Instagram.
Es la única pieza que falta y la que más ayuda a que alguien lo pruebe.

## Regenerar o cambiar textos

Todo el guion vive en `tools/gen-reels.mjs`, en los arrays `reel1` y `reel8`. Cada entrada tiene
`start`, `end`, `dark`, `title`, `sub`, `size` y `shield`. Después:

```bash
node tools/gen-reels.mjs
```

Se renderizan los frames, se codifican los dos MP4 y se borran los temporales. Tarda menos de un
minuto.

## Antes de publicar

- [ ] Has visto el reel entero en el móvil, no solo en el ordenador.
- [ ] El texto se lee sin sonido (todo el texto va incrustado, no hay subtítulos que activar).
- [ ] La portada es la correcta y no queda cortada en la cuadrícula del perfil.
- [ ] No aparece ninguna imagen de menores reales.
- [ ] El enlace del pie lleva su UTM (`utm_content=reel_simulador`).
