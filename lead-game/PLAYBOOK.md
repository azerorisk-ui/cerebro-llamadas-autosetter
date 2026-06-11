# 🎮 DM RUSH · Playbook del lead magnet jugable

> El juego no es el producto. El juego es el **carrusel de 2026**: un formato
> que nadie usa todavía en el mercado info hispano y que convierte un CTA
> pasivo ("comenta SISTEMA") en una experiencia que la gente comparte sola.

---

## 1. El posicionamiento (la decisión clave)

Hay dos formas de jugar esta carta, y la respuesta correcta es **las dos, en orden**:

### Jugada A — El juego como demostración (semana 1)
Lanzas **DM RUSH** a tu propia audiencia. El jugador ES el setter de su
bandeja de Instagram durante 60 segundos. Leads calientes, curiosos y
vendehumos entran cada vez más rápido. Es imposible ganar al final del día.

**Eso es el pitch de Autosetter sin pitchear**: el jugador *siente* en 60
segundos el problema que tú resuelves. La pantalla final le dice cuánto
dinero "dejó morir" y su eficiencia de setter → CTA directo.

### Jugada B — El sistema como lead magnet (semanas 2-4)
Tu historial (Carruseles con Claude, Historias con Claude, Horse Magnet)
tiene un patrón: **no vendes el activo, vendes la máquina de hacer activos**.
Aquí igual: el recurso que entregas no es "un juego", es
**"Juegos con Claude" — el sistema para que cualquier creador genere su
propio mini-juego lead magnet personalizado a su nicho y su CTA en 1 hora**.

Por eso `index.html` tiene TODO lo personalizable en un objeto `CONFIG`
arriba del archivo: mensajes, precios, nicho, textos, CTA, share. Cambias
el CONFIG → tienes el juego de un coach fitness, de un growth partner, de
quien sea. Esa es la prueba de que el "engine personalizable" que intuías
es real y barato.

---

## 2. Por qué un juego convierte mejor que un PDF

| Mecánica | Qué hace por ti |
|---|---|
| **Inversión** | Quien juega 60s está más comprometido que quien descarga un PDF que no abre. Effort = ownership. |
| **Cualificación** | La pantalla de resultados es un diagnóstico disfrazado: "dejaste morir 2.400€" segmenta solo. |
| **Share loop** | El score es presumible/comentable → screenshots en historias → tráfico nuevo sin ads. |
| **Demo del dolor** | El jugador vive el problema (bandeja inbound desbordada) en vez de leerlo. Es una VSL interactiva. |
| **Novedad** | Nadie en info hispano lo está haciendo. El "cómo lo hizo" genera tanta conversación como el juego. |

---

## 3. El funnel completo

```
Reel/Carrusel: "Convertí mi bandeja de DMs en un videojuego"
        ↓ comenta "GAME"
ManyChat → link al juego (60-90 seg, móvil)
        ↓ pantalla de resultados (score + diagnóstico)
        ├─ CTA primario: "Quiero mi bandeja en automático" → Autosetter
        ├─ CTA recurso: "Quiero crear MI juego" → email/keyword → sistema Juegos con Claude
        └─ Share: texto pre-escrito con su score → historias → loop
```

**Métricas para validar (en este orden):**
1. % de clic desde el DM al juego (¿el hook funciona?)
2. % de partidas completadas (¿el juego engancha? objetivo: >70%)
3. % de clic en CTA tras jugar (¿la pantalla final vende? objetivo: >15%)
4. Shares orgánicos (¿hay loop viral?)

Si 2 y 3 funcionan con tu audiencia, el sistema es vendible al mercado.

---

## 4. Cuánto se tarda (tu pregunta)

- **Un juego como el del post de Twitter** (mundo abierto, crafting, tiles):
  semanas. No es el formato correcto para un lead magnet — nadie juega 20
  minutos desde una historia.
- **Un juego como DM RUSH** (60-90s, una mecánica, móvil, score final):
  **este prototipo se hizo en una sesión con Claude**. Pulirlo con sonido,
  captura de email y analytics: 1-2 días. Ese dato ES parte del pitch del
  recurso.

Regla del formato: *snackable* — una mecánica, menos de 90 segundos,
vertical, score compartible, CTA en la pantalla de resultados.

---

## 5. Plan de ejecución

**Semana 1 — Validar con tu audiencia**
- [ ] Ajustar `CONFIG` (URL real del CTA, precios, copys)
- [ ] Subir a Cloudflare Pages (mismo stack que autosetter-lab)
- [ ] Conectar keyword de ManyChat → link
- [ ] Lanzar con contenido "convertí mi bandeja en un videojuego" + behind the scenes
- [ ] Medir las 4 métricas de arriba

**Semana 2-3 — Empaquetar el sistema (si valida)**
- [ ] Documentar el proceso: prompt maestro + plantilla CONFIG + guía de deploy
- [ ] "Juegos con Claude" como recurso entregable (mismo formato que tus drops anteriores)
- [ ] Caso de estudio con tus propios números como prueba

**Semana 4 — Escalar**
- [ ] 2-3 variantes de mecánica para otros nichos (quiz-runner, tycoon de MRR, simulador de lanzamiento)
- [ ] Versión white-label para growth partners (ellos lo despliegan para sus clientes)

---

## 6. Cómo probar el prototipo ya

```bash
# abrir lead-game/index.html en el navegador, o servirlo:
cd lead-game && python3 -m http.server 8080
# → http://localhost:8080 (mejor desde el móvil)
```

Todo lo editable está en el objeto `CONFIG` al inicio del `<script>` de
`index.html`: duración, economía, mensajes por nicho, rangos y CTA.
