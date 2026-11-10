# Enlaces y lectura de datos

## Enlaces de la campaña

Todos apuntan a la aplicación con parámetros para identificar la pieza de origen.

| Pieza | Enlace |
|---|---|
| Instagram · bio | `https://laura0802.github.io/Escudo-1612-App/?utm_source=instagram&utm_medium=bio` |
| Instagram · reel 1 | `…?utm_source=instagram&utm_medium=social&utm_campaign=conciencia_2026&utm_content=reel_espejo` |
| Instagram · carrusel violaciones | `…?utm_source=instagram&utm_medium=social&utm_campaign=conciencia_2026&utm_content=carrusel_violaciones` |
| Instagram · estático | `…?utm_source=instagram&utm_medium=social&utm_campaign=conciencia_2026&utm_content=estatico_1612` |
| Instagram · carrusel proceso | `…?utm_source=instagram&utm_medium=social&utm_campaign=conciencia_2026&utm_content=carrusel_proceso` |
| Instagram · reel 8 | `…?utm_source=instagram&utm_medium=social&utm_campaign=conciencia_2026&utm_content=reel_fuentes` |
| X · hilo mandato | `…?utm_source=x&utm_medium=social&utm_campaign=conciencia_2026&utm_content=hilo_mandato` |
| X · hilo límites | `…?utm_source=x&utm_medium=social&utm_campaign=conciencia_2026&utm_content=hilo_limites` |
| LinkedIn · post | `…?utm_source=linkedin&utm_medium=social&utm_campaign=conciencia_2026&utm_content=post_proceso` |

## Qué mirar en GA4

| Pregunta | Dónde |
|---|---|
| ¿De dónde viene la gente? | Informes → Adquisición → Adquisición de tráfico |
| ¿Llegan al mecanismo? | Informes → Interacción → Páginas y pantallas → `/consenso` |
| ¿Leen? | Informes → Interacción → Eventos → `scroll_90` |
| ¿Salen a comprobar las fuentes? | Eventos → `outbound_click` |
| ¿Qué pieza funciona? | Explorar → Exploración libre, con `utm_content` registrado como dimensión personalizada |

## Registro diario

| Día | Pieza | Alcance | Guardados | Compartidos | Sesiones | Llegadas a /consenso |
|---|---|---|---|---|---|---|
| 1 | Reel espejo | | | | | |
| 2 | Hilo mandato | | | | | |
| 3 | Carrusel violaciones | | | | | |
| 4 | Hilo límites | | | | | |
| 5 | Estático 1612 | | | | | |
| 6 | Post LinkedIn | | | | | |
| 7 | Carrusel proceso | | | | | |
| 8 | Reel fuentes | | | | | |

## Notas

- Los informes de GA4 tardan entre 24 y 48 horas en consolidarse. El mismo día de la publicación,
  usa **Tiempo real**.
- Los bloqueadores de anuncios impiden registrar la visita.
- La atribución asigna la sesión al último clic no directo: alguien que ve el reel y luego entra
  escribiendo la dirección aparecerá como `(direct) / (none)`.
