<h1 align="center">Gerard Morales</h1>
<p align="center">
  <strong>Systems · AI · Cybersecurity</strong><br>
  Software development and my own projects · ASIX @ Institut Tecnològic de Barcelona<br>
  Barcelona, Catalonia, Spain
</p>

<p align="center">
  <a href="#english">English</a> · <a href="#español">Español</a> · <a href="https://www.linkedin.com/in/gerard-morales/">LinkedIn</a>
</p>

---

<h2 id="english" align="center">English</h2>

I learn by taking things apart. I started with hardware — pulling machines apart, building
them back up, working out what was behind each part — and moved through networks, systems
administration and IT support in a real professional environment. Along the way I started
building things of my own, which is what **[WebProDev](https://github.com/LockerDocx/Webprodev)**
is: my studio for web development, custom software and AI integration.

Right now I study **first year of ASIX with a cybersecurity profile at ITB**, while keeping
the projects running. I am looking for opportunities in systems administration, IT support,
web/software development and AI integration — in Barcelona or remote, and I am open to
relocating and to working in English.

### Featured — AI Agent for Firefox

**[`firefox-ai-agent`](https://github.com/LockerDocx/firefox-ai-agent)** · Python · JavaScript · Firefox extension · MIT

A free, open-source AI agent that drives a real browser. You give it a goal in plain
language; it observes the page as a table of indexed elements, asks a model for one
operation and one target, and executes it. The model never writes selectors or code — only
the id of an element it was shown.

What makes it more than a wrapper around an API:

- **Measured, not guessed.** The executor prompt was cut from **21,233 to 10,111 characters
  (≈5,308 → ≈2,528 tokens, −52.4 %)** on a dense page, and it now stops growing with page
  size. `scripts/bench_prompt_size.py` reproduces the whole trade-off curve.
- **An honest changelog.** The v0.13.0 release shipped a one-line quoting bug that made
  **every** click, fill and select fail with a JavaScript `SyntaxError` — and 585 unit tests
  did not catch it, because the suite replaced the CDP layer and the broken half of
  `browser.py` is the half the suite never touched. That is now covered end to end.
- **Credentials are handled, not invented.** Password fields were excluded from the action
  space entirely, which made every login impossible. The field is now reachable, its contents
  are masked in the action, the page key and the guard, and if the goal does not supply a
  credential the run stops and says so instead of guessing one.
- **A verdict that cannot flatter itself.** `scripts/live_battery.py` decides success from
  the final URL rather than from the agent announcing `DONE`, treats a missing credential as
  working code rather than a failed login, and reports `NO EVALUABLE` instead of a percentage
  that cannot be compared with the target.

**819 tests**, ruff clean, all JavaScript parses, green under UTF-8 and under a legacy code
page. Shipped through a release pipeline that builds the wheel, the `.xpi` and the source
archive, with every change in `CHANGELOG.md` stating what was measured and what was not.

### Selected work

| Project | What it is | Stack |
|---|---|---|
| [`Quatre40optics`](https://github.com/LockerDocx/Quatre40optics) | Client website for an optician in Cardedeu, rebuilt from a Hostinger Website Builder site into a real codebase and moved to Vercel at zero cost. Includes the DNS migration runbook. | Next.js 14, React 18, TypeScript, Tailwind |
| [`Arnamar.sl`](https://github.com/LockerDocx/Arnamar.sl) | Client AI platform: describe a renovation in natural language and get an edited render back, plus vision-based surface estimation from a photo of the actual work. | React, TypeScript, Express, Gemini (vision + image) |
| [`arduino-iot-monitor`](https://github.com/LockerDocx/arduino-iot-monitor) | Final project for my systems and networks cycle: an Arduino UNO + DHT11 sensor streaming live temperature and humidity to a dashboard. | Arduino, Next.js, Firebase, Vercel |
| [`mondo_computer`](https://github.com/LockerDocx/mondo_computer) | Client website for an Italian computer retailer, where I did my Erasmus+ placement. SEO metadata, testimonials, FAQ, contact. | Next.js, TypeScript |
| [`Webprodev`](https://github.com/LockerDocx/Webprodev) | The site of my own studio: services, portfolio, pricing, plus client and admin dashboards and an AI chat widget. | React, TypeScript, Firebase |

### Background

**IT Support technician — Châteauform, Campus Belloch** · Feb 2025 – Apr 2026 · 365 h
Day-to-day IT for the companies on the campus: user onboarding and offboarding, Active
Directory and Microsoft Exchange for accounts, mailboxes, permissions and shares, hardware
setup and small upgrades, and GLPI for asset inventory. Working with real users is what
taught me that a technically correct answer is not always a useful one.

**Hardware technician — Mondo Computer, Forlì, Italy** · Jun 2026 · ~150 h · Erasmus+
Diagnosing and refurbishing old laptops component by component — screens, RAM, disks,
keyboards, touchpads, motherboards — then rebuilding working machines from the parts that
survived. A month in another country, another way of working.

**Founder and developer — WebProDev** · Jun 2023 – present
Everything from the first conversation with a client to design, development, deployment and
maintenance. I also handle the client side directly: understanding the idea and turning it
into something that actually works.

**Education**

- **ASIX, Cybersecurity profile** — Institut Tecnològic de Barcelona · from Sept 2026
  Systems and network administration, virtualisation, network services, security
  fundamentals, on both Windows and Linux.
- **Sistemes Microinformàtics i Xarxes** — Escola Ginebró · 2024 – 2026 · grade 8.80
  Hardware, operating systems and networks from the ground up, and the Arduino IoT project
  above as the final piece.
- **Cisco Networking Academy — Introduction to Cybersecurity** · Nov 2025
  6 hours and 7 labs: network vulnerabilities, threat detection, data protection, and the
  practices that actually protect systems and organisations.
- **Cisco Networking Essentials** · 2026

**Languages** — Catalan and Spanish, native.

---

<h2 id="español" align="center">Español</h2>

Empiezo aprendiendo desmontando. Arranqué con el hardware —desmontando ordenadores,
montando equipos, entendiendo qué había detrás de cada máquina— y fui entrando en redes,
administración de sistemas y soporte IT en un entorno profesional real. En paralelo empecé
a construir mis propios proyectos, que es lo que es **[WebProDev](https://github.com/LockerDocx/Webprodev)**:
mi espacio para desarrollo web, software a medida e integración de IA.

Ahora mismo estudio **primero de ASIX con perfil de Ciberseguridad en el ITB**, mientras
sigo llevando los proyectos. Busco oportunidades en administración de sistemas, soporte
informático, desarrollo web o de software e integración de IA: en Barcelona, en remoto, o
donde haga falta. Estoy abierto a otros países y a trabajar en inglés.

### Destacado — AI Agent for Firefox

**[`firefox-ai-agent`](https://github.com/LockerDocx/firefox-ai-agent)** · Python · JavaScript · Extensión de Firefox · MIT

Un agente de IA libre y de código abierto que conduce un navegador de verdad. Le das un
objetivo en lenguaje natural; observa la página como una tabla de elementos indexados, pide
al modelo una operación y un objetivo, y la ejecuta. El modelo nunca escribe selectores ni
código: solo el id de un elemento que se le ha mostrado.

Lo que lo distingue de una simple capa sobre una API:

- **Medido, no estimado.** El prompt del ejecutor bajó de **21.233 a 10.111 caracteres
  (≈5.308 → ≈2.528 tokens, −52,4 %)** en una página densa, y ya no crece con el tamaño de la
  página. `scripts/bench_prompt_size.py` reproduce toda la curva de compromiso.
- **Un changelog honesto.** La v0.13.0 se publicó con un fallo de comillas en una línea que
  hacía que **todos** los clics, rellenos y selecciones fallaran con un `SyntaxError` de
  JavaScript, y 585 pruebas no lo detectaron: la suite sustituye la capa CDP, y la mitad
  rota de `browser.py` es justamente la que la suite no tocaba. Ahora está cubierto de punta
  a punta.
- **Las credenciales se cuidan, no se inventan.** Los campos de contraseña estaban excluidos
  del espacio de acciones, lo que hacía imposible cualquier login. Ahora el campo es
  alcanzable, su contenido se enmascara en la acción, en la clave de página y en la guardia,
  y si el objetivo no aporta la credencial la ejecución para y lo dice, en vez de adivinarla.
- **Un veredicto que no puede favorecerse.** `scripts/live_battery.py` decide el éxito por la
  URL final y no porque el agente diga `DONE`, trata la falta de credencial como el
  comportamiento correcto y no como un login fallido, y dice `NO EVALUABLE` en vez de imprimir
  un porcentaje que no se puede comparar con el objetivo.

**819 pruebas**, ruff limpio, todo el JavaScript compila, verde en UTF-8 y también bajo una
página de códigos heredada. Publicado con un pipeline que genera la wheel, el `.xpi` y el
código fuente, y con cada cambio en `CHANGELOG.md` indicando qué está medido y qué no.

### Otros proyectos

| Proyecto | Qué es | Stack |
|---|---|---|
| [`Quatre40optics`](https://github.com/LockerDocx/Quatre40optics) | Web de cliente para una óptica de Cardedeu, reconstruida desde un sitio de Hostinger Website Builder a un código real y movida a Vercel sin coste. Incluye el manual de migración de DNS. | Next.js 14, React 18, TypeScript, Tailwind |
| [`Arnamar.sl`](https://github.com/LockerDocx/Arnamar.sl) | Plataforma de IA para un cliente: describes una reforma en lenguaje natural y recibes el render editado, además de estimación de superficies por visión a partir de una foto de la obra. | React, TypeScript, Express, Gemini (visión + imagen) |
| [`arduino-iot-monitor`](https://github.com/LockerDocx/arduino-iot-monitor) | Proyecto final de mi ciclo de sistemas y redes: un Arduino UNO con sensor DHT11 enviando temperatura y humedad en vivo a un panel. | Arduino, Next.js, Firebase, Vercel |
| [`mondo_computer`](https://github.com/LockerDocx/mondo_computer) | Web de cliente para una tienda de informática italiana, donde hice las prácticas Erasmus+. SEO, testimonios, FAQ y contacto. | Next.js, TypeScript |
| [`Webprodev`](https://github.com/LockerDocx/Webprodev) | La web de mi propio estudio: servicios, portfolio, precios, panel de cliente y de administración, y un widget de chat con IA. | React, TypeScript, Firebase |

### Trayectoria

**Técnico de soporte informático — Châteauform, Campus Belloch** · Feb 2025 – Abr 2026 · 365 h
Soporte diario para las empresas del campus: alta y baja de usuarios, Active Directory y
Microsoft Exchange para cuentas, buzones, permisos y recursos compartidos, preparación de
equipos y pequeñas ampliaciones de hardware, y GLPI para el inventario. Trabajar con
usuarios reales es lo que me enseñó que una respuesta técnicamente correcta no siempre es
una respuesta útil.

**Técnico de hardware — Mondo Computer, Forlì, Italia** · Jun 2026 · ~150 h · Erasmus+
Diagnóstico y reacondicionamiento de portátiles antiguos pieza a pieza —pantallas, RAM,
discos, teclados, touchpads, placas— y reconstrucción de equipos funcionales con lo que
sobrevive. Un mes en otro país y otra forma de trabajar.

**Fundador y desarrollador — WebProDev** · Jun 2023 – actualidad
Todo el proceso, desde la primera conversación con el cliente hasta el diseño, el
desarrollo, el despliegue y el mantenimiento. También hablo directamente con los clientes:
entender la idea y convertirla en algo que funcione de verdad.

**Formación**

- **ASIX, perfil de Ciberseguridad** — Institut Tecnològic de Barcelona · desde sept. 2026
  Administración de sistemas y redes, virtualización, servicios de red y fundamentos de
  ciberseguridad, en Windows y en Linux.
- **Sistemes Microinformàtics i Xarxes** — Escola Ginebró · 2024 – 2026 · nota 8.80
  Hardware, sistemas y redes desde abajo, con el proyecto de IoT con Arduino como pieza
  final.
- **Cisco Networking Academy — Introducción a la Ciberseguridad** · Nov 2025
  6 horas y 7 prácticas: vulnerabilidades de red, detección de amenazas, protección de datos
  y las prácticas que de verdad protegen sistemas y organizaciones.
- **Cisco Networking Essentials** · 2026

**Idiomas** — Catalán y español, nativos.

---

<p align="center">
  <a href="https://www.linkedin.com/in/gerard-morales/"><strong>Conectado en LinkedIn</strong></a>
  &nbsp;·&nbsp;
  <span>Disponible para oportunidades en sistemas, soporte, desarrollo e IA</span>
</p>
