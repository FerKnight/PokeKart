# PokeKart

Proyecto base para un videojuego de carreras arcade 3D estilo Mario Kart 8, con temática Pokémon y una primera pista funcional de referencia: Bosque Verde.

## Estado actual

Esta primera versión entrega una base jugable, estable y reutilizable para continuar el desarrollo del juego:

- estructura de proyecto con Vite + Three.js
- pista en bucle de referencia con entorno 3D
- kart del jugador y siete rivales controlados por IA
- controles de aceleración, frenado, dirección y cámara
- sistema de vueltas, temporizador y posición
- HUD mínimo funcional
- instalación como PWA con manifest y service worker básico

## Requisitos

- Node.js 18+
- npm

## Instalación

```bash
npm install
```

## Ejecución en desarrollo

```bash
npm run dev -- --host
```

La aplicación estará disponible normalmente en `http://localhost:5173`.

## Producción

```bash
npm run build
npm run preview -- --host
```

## Estructura del proyecto

```text
.
├── index.html
├── package.json
├── public/
│   ├── manifest.webmanifest
│   └── sw.js
├── src/
│   ├── main.js
│   └── style.css
└── vite.config.js
```

## Controles

- Acelerar: `W` o `↑`
- Frenar / marcha atrás: `S` o `↓`
- Izquierda: `A` o `←`
- Derecha: `D` o `→`

## Próximos pasos sugeridos

1. introducir un roster real de Pokémon con modelos 3D y karts con identidad visual
2. ampliar el circuito a pistas con geometrías distintas
3. mejorar física de conducción y IA
4. añadir sistema de copas, puntos y desbloqueos
5. añadir minimapa, objetos, HUD más completo y soporte offline más robusto

## Nota

Esta base no sustituye la validación visual ni la calidad final esperada del proyecto. Sirve como cimiento técnico funcional sobre el que continuar con la producción del juego.
