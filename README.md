# 🎂 Invitación de cumpleaños de Fernando — temática de bloques

Invitación digital interactiva hecha **solo con HTML, CSS y JavaScript** (sin librerías ni imágenes externas). Funciona en celular y computadora.

## ¿Qué hace?

- **Pantalla de inicio:** un bloque de pasto en 3D. Al tocarlo **2 veces** se agrieta, se rompe y se activa el sonido.
- **Portada:** el suelo, los árboles, “¡FELIZ CUMPLE!” y el nombre se construyen bloque por bloque. Después se llena una barra de experiencia que muestra la edad (nivel).
- **Datos de la fiesta:** un cartel de madera que se arma con bloques, con la fecha, la hora y el lugar.
- **Cuenta regresiva** en bloques de piedra.
- **Inventario de la fiesta:** pastel, taquiza, piñata, brincolín, música y sorpresas.
- **Confirmación por WhatsApp:** el invitado escribe su nombre y cuántos van, y se abre WhatsApp con el mensaje listo. También hay botones para **Cómo llegar** (Google Maps) y **Agregar al calendario** (Google Calendar).
- **Pastel interactivo:** al soplar las velas sale confeti y suena “Happy Birthday” en versión de 8 bits.
- Todos los sonidos y la música se generan en el navegador con Web Audio API; las texturas y los íconos se dibujan con `<canvas>`.

## Cómo editar los datos

Abre `index.html` y busca el bloque `CONFIG` al inicio del `<script>`:

```js
const CONFIG = {
  nombre: "Fernando",
  edad: 10,
  fecha: "2026-12-05",       // AAAA-MM-DD
  horaInicio: "16:00",
  horaFin: "21:00",
  lugar: "Jardín de Eventos El Bloque",
  direccion: "Calle Hidalgo 120, Centro, Cocula, Jalisco",
  mapsUrl: "",               // opcional: enlace exacto de Google Maps
  whatsapp: "",              // opcional: 52 + 10 dígitos
  ...
};
```

> Los datos actuales son de ejemplo.

## Publicarla con GitHub Pages

1. En el repositorio ve a **Settings → Pages**.
2. En **Source** elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
3. Guarda. En uno o dos minutos la invitación quedará en:
   `https://fernandojavascrip21-dot.github.io/invitacion-minecraft/`

Ese enlace es el que se comparte por WhatsApp.

## Probarla localmente

Abre `index.html` directamente en el navegador; no necesita servidor ni instalación.
