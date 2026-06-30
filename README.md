# Juan Enrique Rivera

<!-- Opcional: reemplaza la URL por una foto/hero tuya (sube la imagen al repo o usa un link) -->
<!--
<p align="center">
  <img src="URL_DE_TU_FOTO" width="600" />
</p>
-->

<p align="center"><i>
Estudié para construir edificios y terminé construyendo software.<br/>
Me gusta agarrar un problema feo —del campo, de la salud, del mercado— y bajarlo<br/>
a un sistema que funcione solo, 24/7, sin que nadie lo esté mirando.<br/>
Del sensor en terreno al dashboard. Del dato crudo a la decisión.<br/>
Casi nada de lo que hay acá es una demo: está corriendo ahora mismo<br/>
en algún Mac, un VPS o un mini-PC en una bodega.
</i></p>

---

## Ahora

**Construyendo** sistemas que operan solos: trading (**momoneitor**, **HERMES**), un huerto vertical entero (**Carmelo**) y pipelines de datos públicos (**Mercado-Pharma-Stack**).

**A fondo con Claude Code y arquitectura de agentes** — documenté y dejé impecables +25 repos con esto, varios usan agentes y MCP en producción.

**Constructor Civil UC** que pasó de la obra a la ingeniería de proyectos TI y de ahí al software. Mezclo mundo físico (ESP32, PCBs, riego, clima) con backend, datos e IA.

**Disponible para** consultoría y proyectos — automatización, agentes de IA, IoT/agro y data. Escríbeme por acá o por [LinkedIn](https://www.linkedin.com/in/).

---

## Proyectos

> 🔒 = privado (va la descripción, no el código). El resto son públicos y clickeables.

### 📈 Trading y mercados de predicción

**momoneitor** 🔒 — Tablero de trading en mi Mac, 24/7. Vigila SOXL, aplica compras escalonadas con filtro de régimen y me avisa por Telegram cuándo comprar; yo aprieto el gatillo. `FastAPI · Postgres · Docker · Claude`

**HERMES** 🔒 — Fondo de trading automático para Polymarket: varios bots en paralelo, cada uno con coordinador y watchdog, con frenos abajo del todo (DRY_RUN, circuit breakers, topes). `Python · FastAPI · Redis`

**atlas-vega-polymarket** 🔒 — Flota de ~40 bots, uno por estrategia (copy trade, arbitrajes, weather, snipers, market making), con un core común de riesgo. Los orquesta launchd. `Python · launchd · Postgres`

**Tau** 🔒 — Agente de IA 24/7 sobre OpenClaw + core multi-agente (Orchestrator → Director → Quant → Risk → Execution) operando Manifold y Polymarket. `Python · multi-agente`

### 🌱 AgroTech — huerto vertical (AgroUrbana)

**[QiU](https://github.com/jnrivra/QiU)** ⭐ — PCB open-source basada en ESP32 para automatizar hidroponía: 7 relés, 6 bombas dosificadoras, sensado de pH/EC/clima/peso. ~80 USD, diseñada en EasyEDA. `ESP32 · Hardware`

**[IvY_agents](https://github.com/jnrivra/IvY_agents)** — Suite de inteligencia para huerto vertical: un sistema de diseño de 14 agentes de IA más dashboards en React/TS para VPD, temperatura, humedad y CO₂. `TypeScript · React · IA`

**Carmelo** 🔒 — El cerebro de clima de 4 salas: cada una corre su algoritmo cada 2-3 min sobre Node-RED + Home Assistant; la data va a InfluxDB/DuckDB para cruzar clima con rendimiento. Expone herramientas a Claude vía MCP. `Node-RED · HA · Python · InfluxDB`

**unify-guardian** 🔒 — Monitoreo y seguridad 24/7 de la red UniFi en Docker: Prometheus + Grafana + Loki más un exportador propio que detecta intrusos, fallas de cámaras y ARP spoofing. `Docker · Prometheus · Python`

**interfazFertiriego** 🔒 — Riego automático: pantalla Nextion → ESP32-S3 → válvulas vía MCP23017 sobre ESPHome/HA. 6 islas + bomba, una sola válvula abierta a la vez. `ESPHome · ESP32 · Nextion`

*Y la familia de análisis de cultivo (privados):* **vpdAnalisis**, **dataRabbit**, **RabbitData**, **Analisis-Cultivo**, **HomeAssistant-AUditor** — apps web/Streamlit para seguir VPD, comparar semanas y revisar el histórico de sensores. · También público: **[EZO_PRS](https://github.com/jnrivra/EZO_PRS)** (componente ESPHome) y **[Eagle-Libraries](https://github.com/jnrivra/Eagle-Libraries)**.

### 💊 Datos de salud pública

**Mercado-Pharma-Stack** · **MP-Scrapper** 🔒 — Tomo el dato público de cuánto gasta el Estado chileno en medicamentos (Mercado Público, Cenabast), lo dejo limpio en una base de datos y encima un dashboard con asistente de IA. `Python · Next.js · Supabase`

### 🏥 Salud y hardware médico

**[proyecto-suena](https://github.com/jnrivra/proyecto-suena)** — Firmware ESP32 (UC CHRISTUS) para nodos que miden ruido, luz y temperatura del ambiente de descanso de pacientes hospitalizados; publica por MQTT. `C++ · ESP32 · MQTT`

**[uvcCalculator](https://github.com/jnrivra/uvcCalculator)** — Simulador 3D de dosis UV-C para desinfectar aire en ductos HVAC: mapa de dosis y optimización de tubos germicidas. `React · Three.js`

**clinica-kr** 🔒 — Todo para abrir una clínica de medicina estética en Valdivia: marca, web (Odoo + Cloudflare), marketing (Meta Ads + n8n + WhatsApp), equipos y legal. `Odoo · n8n · Python`

### 🤖 IA, contenido y civic tech

**[conecta_catemu](https://github.com/jnrivra/conecta_catemu)** — Participación ciudadana municipal por WhatsApp con IA: reportes y encuestas vía bot, categorización con Claude en n8n y dashboard en tiempo real. (Hackathon 2025) `Express · SQLite · Claude · n8n`

**[creador_rol](https://github.com/jnrivra/creador_rol)** — Compañero web de RPG de mesa para niños (4-8 años): doble pantalla, audio procedural y arte generado con IA. Cero dependencias. `Vanilla JS`

**mawida-broll-tools** 🔒 — Genera prompts de B-roll con IA para nichos regulados: parte el guion en escenas y traduce los términos sensibles a lenguaje visual neutro al exportar. `Node · Express · Claude API`

**Triangulatron** 🔒 — App local para el Comité de Prevención de la Tortura: toma el material de las visitas, extrae hallazgos, los cruza entre fuentes y arma un borrador de informe. `Python · Flask · Claude Code`

### 🧰 Utilidades

**[fintual_devops_interview](https://github.com/jnrivra/fintual_devops_interview)** — Prototipo Django + Postgres vuelto servicio operable: N+1 resuelto (96s → 54ms), full-text search, observabilidad (Prometheus), Docker/K8s/Helm. `Django · Postgres · K8s`

**[etiquetatron](https://github.com/jnrivra/etiquetatron)** — App de escritorio que extrae etiquetas de envío desde PDFs y las guarda como imágenes a 300 DPI listas para imprimir. `Python`

---

<sub>La mayoría de mis repos son privados — escríbeme si quieres ver alguno por dentro.</sub>
