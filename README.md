# Landing Page — Portfolio | Federico Acosta Maneiro

## Descripción

Landing page de portafolio personal, desarrollada como Trabajo Práctico (PFO1) para la Tecnicatura en Desarrollo de Software. El sitio muestra mi presentación, mis habilidades técnicas y blandas, una sección personal sobre mis hobbies (cine y música), un formulario de contacto de demostración y un regalo al final para quien llegue hasta el fondo de la página.

Construido con **HTML5 semántico y CSS3 puro**, sin JavaScript ni frameworks, cumpliendo con los requisitos técnicos de la consigna: header/nav/main/footer, Flexbox y Grid, Google Fonts, diseño responsive, animaciones/transiciones, imágenes con `alt` y formulario con `label`.

## 🔗 Demo

**URL de Vercel:** (https://landing-portfolio-tecnicatura.vercel.app/)

**Perfil de GitHub:** [github.com/federicosd06-dev](https://github.com/federicosd06-dev)

## Decisiones de diseño

- **Estética elegida: Cyberpunk.** Antes de decidir, armé tres versiones completas del mismo sitio (River Plate, Cyberpunk y una fusión de ambas) usando variables CSS, para poder comparar visualmente antes de elegir. Me quedé con la cyberpunk: fondo oscuro, acentos en cian (`#00F0FF`) y magenta (`#FF2079`), tipografía **Orbitron** para títulos y **Space Mono** para el cuerpo de texto — buscando una estética de interfaz futurista/terminal.
- **Todo el sitio es una sola página** con navegación por anclas (`#inicio`, `#habilidades`, `#sobre-mi`, `#contacto`), pensada para un portfolio simple y directo.
- **Sin JavaScript por decisión propia**, incluso donde normalmente se usaría (menú hamburguesa responsive, apertura del easter egg): ambos se resuelven con el truco de `<input type="checkbox">` oculto + `<label>`, controlado enteramente con CSS (`:checked`).
- **Animación obligatoria de la consigna:** las tarjetas de películas y artistas favoritos usan un efecto *flip-card* en CSS puro (`perspective` + `rotateY`), mostrando una imagen al frente y una descripción al dorso al pasar el cursor o dar foco con teclado.
- **Otras transiciones/animaciones:** subrayado animado en los links del nav al hover, glow en botones e inputs al hover/focus, cursor de terminal parpadeante (`@keyframes blink`) junto a mi apellido en el hero, y la apertura animada del regalo final con `grid-template-rows` (técnica CSS-only para animar un "alto: auto").
- **Iconos de tecnologías:** integré [Devicon](https://devicon.dev/) (una librería de iconos vía CSS/font, sin JS) para mostrar el logo de cada tecnología en la sección de habilidades técnicas.
- **Accesibilidad:** todas las imágenes tienen `alt` descriptivo, el formulario tiene `label` asociado a cada campo, hay estados `:focus-visible` visibles para navegación por teclado, y los links externos que abren en pestaña nueva incluyen texto adicional para lectores de pantalla.
- **Fotos:** todas las imágenes del sitio (perfil, películas, discos, etc) son fotos propias, sin generar ni procesar con IA.

## Declaración de uso de IA

- **Herramienta usada:** Claude
- **Plan:** Gratuito.
- **Para qué la usé:** planificación del proyecto (estructura de secciones, organización de carpetas), generación del esqueleto HTML semántico y del CSS base, exploración comparativa de las 3 direcciones estéticas (River / Cyberpunk / fusión), implementación de funcionalidades puntuales sin JavaScript (menú hamburguesa, flip-cards, easter egg), integración de íconos de tecnologías, y una revisión final de accesibilidad y buenas prácticas (alt descriptivos, nombres de archivo, rutas relativas, limpieza de CSS sin uso).
- **Experiencia previa con la herramienta:** ya la había usado antes en otros proyectos personales, incluyendo una biblioteca personal de PDFs y un e-commerce que estoy construyendo actualmente.
- **Qué revisé/adapté con criterio propio:** definí yo mismo el contenido real, tomé la decisión final de la estética entre las 3 opciones generadas,y revisé cada sección del código generado para entender su funcionamiento antes de aceptarlo (en particular el mecanismo CSS-only del menú hamburguesa, el flip-card y el easter egg).

## Estructura del proyecto

```
landing-portfolio-tecnicatura/
├── index.html
├── css/
│   └── style.css
├── assets/
│   └── img/
│       ├── perfil.jpg
│       ├── peliculas/
│       └── artistas/
└── README.md
```
