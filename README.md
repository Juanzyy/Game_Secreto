# Game_Secreto

Proyecto Flutter del juego "Adivina el número".

## Historial de modificaciones

### 2026-02-23
- Se cambió la paleta visual principal a azul agua marina usando `Colors.teal`.
- Se actualizó el tema general y los componentes visuales relacionados (degradados, iconos y botones) para mantener consistencia.
- Se agregó un botón de `Pista` que revela si el número secreto es par o impar.
- Cada uso de la pista descuenta 1 intento extra; si llega a 0, el juego termina.
- Se agregó un `LinearProgressIndicator` para mostrar visualmente los intentos restantes.
- El indicador cambia de color según el estado: verde → amarillo → rojo.
- Se agregó un historial de intentos con `ListView` compacto para ver los números ya probados.
- Los intentos se colorean para distinguir si estuvieron muy altos o muy bajos.
- Se agregó una animación de rebote en el ícono cuando el jugador acierta el número.
- El contenedor del mensaje principal ahora usa `AnimatedContainer` para cambiar de tamaño suavemente.
- Se implementó sistema de récord con `SharedPreferences` que guarda la menor cantidad de intentos.
- El récord se muestra en la interfaz y se conserva entre sesiones.
- Se agregó selector de dificultad con `SegmentedButton`:
  - **Fácil**: números 1-50 con 7 intentos.
  - **Difícil**: números 1-200 con 4 intentos.
