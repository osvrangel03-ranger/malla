# Documento de Visión y Alcance

> Red social local, con identidad real y cronología sin algoritmo.
> Borrador de exploración — **Fase 0**. No describe código todavía: describe qué es, para quién, qué entra y qué no.

- **Autor:** Osvaldo
- **Ciudad de arranque:** Tampico, Tamaulipas, México
- **Estado:** Borrador para discusión
- **Última actualización:** 2026

---

## 1. La apuesta en una frase

Construir una red social **local, con identidad real y sin algoritmo**, donde la ciudad
es la unidad y la plataforma es una **herramienta para hacer cosas** (vender, conectar,
enterarte de tu entorno), no un escaparate para competir por atención.

## 2. El problema

Las redes sociales actuales dejaron de ser un medio de comunicación y se volvieron:

- **Un concurso de comparación**, no un lugar de encuentro.
- **Un sistema de discursos fabricados** donde no distingues opinión real de contenido
  automatizado o incentivado.
- **Un terreno de anonimato abusivo**: perfiles fantasma, estafas y granjas de contenido.
- **Un orden impuesto por el algoritmo**, que decide qué es relevante para ti sin saber
  quién eres ni dónde vives.
- **Un mercado poco confiable**: el marketplace local se llenó de perfiles falsos y
  publicaciones de estafa.

La consecuencia: entras a compararte, no a conectar. Y eso nos aleja del fin original de
una comunicación sin fronteras.

## 3. La tesis (qué nos hace distintos)

| Dimensión | Redes dominantes | Esta red |
|---|---|---|
| Orden del contenido | Algoritmo opaco | **Cronología** (lo nuevo primero) |
| Alcance | Global y difuso | **Ciudad** como unidad, con puentes explícitos a otras ciudades |
| Identidad | Anónima o difusa | **Identidad real** (teléfono + ciudad) |
| Modelo | Publicidad y atención | **Sin publicidad**; sostenida por la comunidad |
| Rol | Escaparate / entretenimiento | **Herramienta** para un fin |
| Código | Cerrado | **Abierto** (excepto secretos operativos, no el login) |

**La idea central:** las empresas solo nos venden lo que elegimos comprar. La diferencia
real no se logra prohibiendo el algoritmo, sino **ofreciendo algo mejor que el caos**.

## 4. Principios no negociables

1. **Ciudad primero.** El contenido local de tu ciudad es el corazón. Ver otras ciudades
   es posible y explícito, nunca accidental.
2. **Cronología, no algoritmo.** Nada está "por encima" de otra cosa por pago o engagement.
3. **Identidad real.** Tu perfil dice de qué ciudad eres. Sin fantasmas.
4. **Cero publicidad.** Ningún anuncio, ningún contenido patrocinado disfrazado.
5. **Publicaciones personales.** Hechas por personas, no granjas automatizadas.
6. **Es una herramienta.** Si no sirve para resolver algo concreto, no es prioridad.
7. **Código abierto.** La transparencia es parte del producto y de la confianza.

> Nota de realidad: "principio" no es "gratis". Ver sección 9 (Sostenibilidad).

## 5. Usuario objetivo y nicho de arranque

**No** arrancamos con "toda la ciudad". Arrancamos con **un nicho con alta necesidad de
contacto local**, y crecemos barrio por barrio / círculo por círculo.

Candidatos de nicho inicial (a elegir uno en Fase 0.5):

- **Comerciantes de un mercado o zona comercial** — máxima necesidad del marketplace.
- **Una preparatoria / universidad** — densidad alta, identities verificables, adopción rápida.
- **Un fraccionamiento / colonia** — el modelo Front Porch Forum (EE.UU.), probado durante 20 años.

Perfil de usuario:
- Vive en Tampico (o su zona metropolitana: Ciudad Madero, Altamira).
- Quiere comprar/vender local sin miedo a estafas.
- Quiere enterarse de lo que pasa cerca, no de lo que pasa en el mundo entero.
- Está cansado de la superficialidad y del juicio público.

## 6. Alcance por fases

### 6.1 Qué NO entra en el MVP (y por qué)

Estas son las trampas que pueden hundir el arranque. Se posponen, no se descartan:

- **Mesh por Bluetooth** — gran I+D, experiencia pobre, batería, iOS no permite BLE en
  segundo plano. Es feature de nicho futuro, no base del producto.
- **Historias / carruseles destacados** — valor estético alto, valor funcional bajo.
  Pueden esperar; compiten por tu tiempo contra lo que sí resuelve.
- **Grupos y páginas** — se construyen sobre una comunidad que primero tiene que existir.
- **Mensajería "que reemplace a WhatsApp"** — no se compite de frente contra efectos de
  red globales. Se compite por *utilidad local*.
- **Federación multi-ciudad completa** — decisión arquitectónica abierta (ver sección 8),
  pero su implementación no es MVP.

### 6.2 MVP (Fase 1) — el objetivo más pequeño que demuestra la tesis

| Módulo | Qué incluye | Criterio de "listo" |
|---|---|---|
| Registro e identidad | Alta con teléfono (SMS) + ciudad; sin INE | Un usuario real nuevo puede entrar en < 2 min |
| Perfil | Nombre, foto, ciudad, bio corta | El perfil muestra claramente de qué ciudad es |
| Publicaciones | Texto con **límite de caracteres** + 1–N fotos | Publicar una foto con texto funciona y se ve bien |
| Feed local | Cronológico, solo mi ciudad; filtro a otras | Veo lo de mi ciudad, sin algoritmo |
| Interacción | Reacciones y comentarios | Comentar una publicación |
| Reportes y moderación | Botón de reporte + panel admin básico | Puedo ocultar/expulsar contenido y cuentas abusivas |
| Marketplace v1 | Publicar artículo con foto + contacto; sin pagos en línea | Un comerciante publica y alguien le escribe |
| Aviso de privacidad | Texto legal claro y aceptable | Cumple mínimos de la LFPDPPP (ver sección 7) |

**Explícitamente fuera del MVP:** mesh BT, historias, grupos/páginas, mensajería
avanzada, verificación de identidad legal, pagos.

### 6.3 Fase 2 — profundizar el marketplace y la vida local

- Mensajería 1:1 dentro de la app.
- Marketplace con reputación, historial y verificación manual del vendedor
  ("programa de afiliados" gratuito: foto y publicaciones coinciden).
- Historias y carruseles en el perfil.
- Páginas y grupos locales.
- Notificaciones y búsqueda.

### 6.4 Fase 3 — ambición

- Mensajería experimental por Bluetooth / mesh (con expectativas realistas).
- Apps nativas (iOS/Android) más allá de la PWA.
- Federación / múltiples ciudades como nodos independientes.
- Verificación avanzada para comerciantes de alto volumen.

## 7. Restricciones legales y de privacidad (México)

Esto **no es asesoría legal formal**, pero define el marco que el producto debe respetar:

- **LFPDPPP** (Ley Federal de Protección de Datos Personales en Posesión de los
  Particulares) y sus reformas de 2025: la plataforma es **responsable** de los datos que
  recolecta. Requiere **aviso de privacidad**, derechos **ARCO** y medidas de seguridad.
- **Geolocalización = dato personal.** Regla de diseño: **guardar la ciudad, no las
  coordenadas exactas.** Nada de lat/long persistente.
- **Identidad:** verificar por **teléfono + ciudad**, no por documentos oficiales. Pedir
  INE/selfies te convierte en custodio de datos sensibles y multiplica tu riesgo y tu costo.
- **Menores:** la ley protege especialmente los datos de menores; hay que definir edad
  mínima y tratamiento.
- **Responsabilidad por contenido de usuarios:** se necesitan **Términos de Uso**,
  mecanismo de reporte y política de moderación.
- **Open source:** reduce riesgo pero no lo elimina; el responsable del tratamiento sigue
  siendo quien opera el servicio.

**Acción de Fase 0.5:** consultar a un abogado local antes de recolectar cualquier dato
de ubicación o identidad a escala.

## 8. Decisiones abiertas (a resolver en Fase 0)

1. **¿Un servidor central o nodos federados por ciudad?**
   - Central: más control y simplicidad; tu costo escala con los usuarios.
   - Federado (tipo ActivityPub): encaja con los valores, reparte costos y cold-start,
     pero es más complejo.
   - *Recomendación inicial:* diseñar el modelo de datos compatible con federación futura,
     pero lanzar centralizado para aprender rápido.
2. **¿Cómo se sostiene sin publicidad?**
   - Donaciones, cooperativa de usuarios, patrocinio de negocios locales sin ads invasivos.
   - *Debe decidirse ANTES de diseñar almacenamiento de fotos/video*, porque define límites.
3. **¿Nombre y branding?** Pendiente. La identidad debe comunicar "local, real, útil".
4. **¿Qué tan libre es el registro entre ciudades?** ¿Cuarentena de contenido foráneo?
5. **¿Qué pasa con el contenido dañino pero legal?** Política de moderación explícita.

## 9. Sostenibilidad: los costos reales

El código abierto y "sin monetización" **no** significa "sin costos".

| Costo | Realidad |
|---|---|
| Almacenamiento y ancho de banda | **El enemigo principal.** Fotos y sobre todo **video** escalan rápido. |
| Hosting básico | ~$0–50 USD/mes en un MVP pequeño; sube con usuarios. |
| Moderación | **Trabajo humano.** Es el gasto oculto de toda red social. |
| Tu tiempo | Proyecto "en serio": **1 a 3 años**, no semanas. |
| Distribución | Trabajo de campo (no de código): conseguir los primeros 100 usuarios. |

## 10. Riesgos y mitigación

| Riesgo | Mitigación |
|---|---|
| **Se muere vacía** (efecto de red) | Sembrar un nicho, no la ciudad entera. Crecer círculo por círculo. |
| **Bomba legal por datos** | Teléfono + ciudad, no documentos; ciudad en vez de coordenadas; asesoría legal. |
| **Estafas en el marketplace** | Reputación comunitaria + verificación manual a escala pequeña. |
| **Toxicidad y moderación** | Política clara + identidad real (reduce anonimato abusivo) + panel admin. |
| **Costo de almacenamiento** | Comprimir imágenes, límites de video, plan de sostenibilidad desde el día uno. |
| **Riesgo de que "no enganche"** | Es un riesgo real y aceptable: la promesa es utilidad, no dopamina. Medir utilidad, no tiempo en pantalla. |
| **Reinventar lo que ya existe** | Estudiar Front Porch Forum, Nextdoor, Mastodon/Lemmy, Briar/Bridgefy/Meshtastic. |

## 11. Métricas de éxito (de utilidad, no de vanidad)

- **Transacciones locales cerradas** en el marketplace.
- **Personas que vuelven** por una razón concreta (vender, enterarse, conectar).
- **Reportes resueltos** / tiempo de respuesta de moderación.
- **Retención por barrio o nicho**, no promedio global.
- **Cero** anuncios y **cero** contenido patrocinado, siempre. (Métrica de integridad.)

## 12. Preguntas abiertas para la siguiente sesión

1. ¿Cuál de los tres nichos de arranque eliges (mercado, universidad, colonia)?
2. ¿Central o federado? (decisión que condiciona todo lo técnico)
3. ¿Cómo se financia el mes 1? (donaciones / cooperativa / patrocinio)
4. ¿Nombre provisional y esencia del branding?
5. ¿Qué es lo mínimo que haría que un tampiqueño la use **mañana**?

---

### Próximo paso sugerido

Elegir el **nicho de arranque** y una **decisión de sostenibilidad**.
Con eso, el documento pasa de "visión" a "plan de MVP concreto" y ya se puede hablar de
arquitectura técnica.
