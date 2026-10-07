# Developer Master Brief (dev-brief.md)
**Documento Maestro de Contenido, SEO Local y Conversión**  
**Proyecto:** M&E Estética y Salud  
**Agencia:** WAFLERS  
**Rol Activo:** Lead Copywriter & Local SEO Strategist  
**Versión:** 1.0.0 (Aprobado para Ensamble Frontend)  
**Fecha:** 2026-10-07  
**Tono de Voz Rector:** *Estética del Alma* — Empático, cercano, sereno, clínicamente riguroso y 100% libre de Spanglish o clichés comerciales agresivos.  
**Canal Oficial de Conversión:** WhatsApp Business (`+54 9 261 681-7621`)  
**Ubicación Estratégica:** Av. San Martín 5355, Chacras de Coria, Luján de Cuyo, Mendoza  

---

## 1. Directrices de Copywriting y Pilares de Conversión

### 1.1 Tono "Estética del Alma"
El lenguaje combina la calidez y serenidad de un espacio holístico con la precisión técnica de un consultorio especializado.
* **Cero Spanglish:** Prohibido utilizar anglicismos vacíos como *"glow-up"*, *"anti-aging routine"*, *"beauty tips"* o *"skincare hacks"*. Se emplea terminología profesional y transparente: *"cuidado dermocosmético integral"*, *"renovación celular"*, *"firmeza y elasticidad cutánea"*, *"descarga neuromuscular"*.
* **Autoridad sin Distancia:** Se proyectan los 20 años de experiencia continua de su fundadora con humildad técnica y calidez de trato personal.

### 1.2 Neutralización Activa de la Barrera de Género (Enfoque 100% Unisex)
Históricamente, los centros estéticos han proyectado una comunicación exclusivamente femenina que genera rechazo e incomodidad en hombres.
* **Mandato de Redacción:** En la landing page se deja explícito que el consultorio atiende tanto a hombres como a mujeres sin distinción.
* La comunicación normaliza el cuidado de la piel, la depilación corporal/facial y el alivio de contracturas para cualquier persona que valore su salud y bienestar personal.

### 1.3 SEO Local Integrado Orgánicamente
Las palabras clave de intención transaccional en Mendoza (`depilacion definitiva chacras de coria`, `estetica chacras de coria`, `tratamientos faciales lujan de cuyo`, `masajes descontracturantes chacras de coria`) se tejen en los encabezados `h1`, `h2` y párrafos sin forzar la lectura ni caer en *keyword stuffing*.

---

## 2. Inyección de Metadata, Open Graph y Schema JSON-LD (`<head>`)

El Programador debe inyectar este bloque directamente en el `<head>` del archivo raíz (`index.html`):

```html
<!-- Meta Tags Primarios -->
<title>M&E Estética y Salud | Consultorio Privado en Chacras de Coria</title>
<meta name="title" content="M&E Estética y Salud | Consultorio Privado en Chacras de Coria" />
<meta name="description" content="Consultorio exclusivo de estética y bienestar en Chacras de Coria, Mendoza. Depilación definitiva Láser Titanium con equipo propio, tratamientos faciales y corporales, y masajes. Atención personalizada unisex." />
<meta name="robots" content="index, follow" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta name="theme-color" content="#FAF8F5" />
<link rel="canonical" href="https://mye-estetica.com.ar/" />

<!-- Open Graph / Previsualización en WhatsApp e Instagram -->
<meta property="og:type" content="website" />
<meta property="og:url" content="https://mye-estetica.com.ar/" />
<meta property="og:title" content="M&E Estética y Salud | Chacras de Coria, Mendoza" />
<meta property="og:description" content="Estética del alma, rigor técnico y privacidad total. Depilación Láser Titanium, tratamientos faciales Laca, remodelación corporal y masajes en Chacras de Coria. Turnos exclusivos unisex." />
<meta property="og:image" content="https://mye-estetica.com.ar/assets/brand/og-image.jpg" />
<meta property="og:locale" content="es_AR" />
<meta property="og:site_name" content="M&E Estética y Salud" />

<!-- Schema Markup LocalBusiness (JSON-LD) -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HealthAndBeautyBusiness",
  "@id": "https://mye-estetica.com.ar/#business",
  "name": "M&E Estética y Salud",
  "image": "https://mye-estetica.com.ar/assets/brand/logo.svg",
  "description": "Consultorio privado de estética integral, aparatología avanzada y bienestar holístico en Chacras de Coria, Mendoza. Atendido exclusivamente por su fundadora con 20 años de trayectoria.",
  "url": "https://mye-estetica.com.ar",
  "telephone": "+5492616817621",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Av. San Martín 5355",
    "addressLocality": "Chacras de Coria",
    "addressRegion": "Mendoza",
    "postalCode": "5505",
    "addressCountry": "AR"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": -32.9981,
    "longitude": -68.8789
  },
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"],
      "opens": "09:00",
      "closes": "20:00"
    }
  ],
  "priceRange": "$$",
  "sameAs": [
    "https://www.instagram.com/mye_esteticasalud"
  ]
}
</script>
```

---

## 3. Matriz de Enlaces de Conversión WhatsApp

Todos los llamados a la acción utilizan el número internacional `+5492616817621` con mensajes preformateados y codificados en URL (`encodeURIComponent`):

| Ubicación del CTA | Texto del Botón | Mensaje Predeterminado en WhatsApp | Enlace URL Codificado |
| :--- | :--- | :--- | :--- |
| **Header Navbar** | Agendar Turno | *Hola, quisiera consultar disponibilidad de turnos en el consultorio de Chacras de Coria.* | `https://wa.me/5492616817621?text=Hola%2C%20quisiera%20consultar%20disponibilidad%20de%20turnos%20en%20el%20consultorio%20de%20Chacras%20de%20Coria.` |
| **Hero Principal** | Agendar Valoración Inicial | *Hola, me gustaría agendar una valoración inicial y conocer qué tratamiento se adapta mejor a mis necesidades.* | `https://wa.me/5492616817621?text=Hola%2C%20me%20gustar%C3%ADa%20agendar%20una%20valoraci%C3%B3n%20inicial%20y%20conocer%20qu%C3%A9%20tratamiento%20se%20adapta%20mejor%20a%20mis%20necesidades.` |
| **Hero Offer (Láser)** | Consultar Turno de Láser Titanium | *Hola, me interesa realizarme depilación definitiva Láser Titanium. Quisiera consultar zonas, precios y disponibilidad de días.* | `https://wa.me/5492616817621?text=Hola%2C%20me%20interesa%20realizarme%20depilaci%C3%B3n%20definitiva%20L%C3%A1ser%20Titanium.%20Quisiera%20consultar%20zonas%2C%20precios%20y%20disponibilidad%20de%20d%C3%ADas.` |
| **Catálogo Facial** | Consultar Tratamientos Faciales | *Hola, quisiera asesoramiento sobre los tratamientos faciales y dermocosmética de Laboratorio Laca.* | `https://wa.me/5492616817621?text=Hola%2C%20quisiera%20asesoramiento%20sobre%20los%20tratamientos%20faciales%20y%20dermocosm%C3%A9tica%20de%20Laboratorio%20Laca.` |
| **Catálogo Corporal** | Consultar Tratamientos Corporales | *Hola, me comunico para consultar por sesiones de aparatología corporal (reductores, presoterapia y tonificación).* | `https://wa.me/5492616817621?text=Hola%2C%20me%20comunico%20para%20consultar%20por%20sesiones%20de%20aparatolog%C3%ADa%20corporal%20(reductores%2C%20presoterapia%20y%20tonificaci%C3%B3n).` |
| **Catálogo Bienestar** | Coordinar Sesión de Masajes | *Hola, quisiera reservar un turno para una sesión de masajes integrales / terapias de relajación.* | `https://wa.me/5492616817621?text=Hola%2C%20quisiera%20reservar%20un%20turno%20para%20una%20sesi%C3%B3n%20de%20masajes%20integrales%20%2F%20terapias%20de%20relajaci%C3%B3n.` |
| **Bloque Contacto** | Escribir por WhatsApp | *Hola, quisiera coordinar un turno en M&E Estética y Salud.* | `https://wa.me/5492616817621?text=Hola%2C%20quisiera%20coordinar%20un%20turno%20en%20M%26E%20Est%C3%A9tica%20y%20Salud.` |
| **FAB Flotante** | WhatsApp Directo | *Hola, me comunico desde la web de M&E Estética y Salud para consultar por turnos disponibles.* | `https://wa.me/5492616817621?text=Hola%2C%20me%20comunico%20desde%20la%20web%20de%20M%26E%20Est%C3%A9tica%20y%20Salud%20para%20consultar%20por%20turnos%20disponibles.` |

---

## 4. Contenido Textual Exacto Sección por Sección

### Sección 0: Header / Navbar Sticky (`#header`)
* **Nombre de Marca en Header:** `M&E Estética y Salud`
* **Sub-etiqueta Mobile / Desktop:** `Chacras de Coria`
* **Enlaces de Navegación por Anclas:**
  1. `Diferenciales` (`href="#diferenciales"`)
  2. `Láser Titanium` (`href="#laser"`)
  3. `Tratamientos` (`href="#tratamientos"`)
  4. `El Espacio` (`href="#consultorio"`)
  5. `Preguntas` (`href="#faq"`)
  6. `Ubicación` (`href="#contacto"`)
* **Botón de Acción Rápida (Navbar CTA):**
  * **Texto:** `Agendar Turno`
  * **Destino:** Enlace de WhatsApp directo.

---

### Sección 1: Hero Section (`#hero`)
* **Eyebrow / Badge Superior:**
  `CHACRAS DE CORIA · CONSULTORIO PRIVADO EXCLUSIVO`
* **Titular Principal (`<h1>`):**
  `Estética avanzada y bienestar integral en Chacras de Coria: el cuidado que tu cuerpo merece.`
* **Bajada Descriptiva:**
  `Un espacio íntimo donde la tecnología de vanguardia y la armonía personal se encuentran. Atendido exclusivamente por su fundadora con 20 años de experiencia, 100% con turno previo programado, sin esperas compartidas y con atención unisex personalizada.`
* **Botones de Conversión (CTAs):**
  * **CTA Primario:** `Agendar Valoración Inicial` (dispara enlace de WhatsApp preconfigurado).
  * **CTA Secundario:** `Explorar Tratamientos` (`href="#tratamientos"`).
* **Badges de Autoridad & Confianza (debajo del Hero):**
  * `✓ 20 años de trayectoria técnica y capacitación continua`
  * `✓ Atención personalizada 1 a 1 sin cruzarse con nadie`
  * `✓ Aparatología propia permanente en consultorio`
  * `✓ Protocolos y tratamientos 100% unisex`

---

### Sección 2: Pilares de Confianza y Diferenciales ("La Experiencia M&E") (`#diferenciales`)
* **Eyebrow de Sección:**
  `EL VALOR DE LO EXCLUSIVO`
* **Título de Sección (`<h2>`):**
  `Por qué elegir un consultorio privado frente a un centro masivo`
* **Bajada de Sección:**
  `Tu tiempo, tu intimidad y tu tranquilidad son la prioridad. Diseñamos un modelo de atención donde nunca sos un número más ni esperás en una sala concurrida.`
* **Grid de 4 Diferenciales:**
  * **Diferencial 1: Privacidad Absoluta y Puntualidad Real**
    * *Título:* `Atención Exclusiva 1 a 1`
    * *Texto:* `El consultorio se reserva para una sola persona a la vez. No compartís sala de espera con desconocidos ni sufrís demoras innecesarias. Ingresás a tu hora convenida en un clima de silencio y confort.`
  * **Diferencial 2: Equipamiento Propio Permanente**
    * *Título:* `Sin Depender de Alquileres de Máquinas`
    * *Texto:* `Nuestra aparatología —incluyendo el Láser Titanium y los sistemas de radiofrecuencia— reside de manera fija en el consultorio. Coordinamos tus sesiones cualquier día de la semana sin atarte a fechas itinerantes mensuales.`
  * **Diferencial 3: Trayectoria de 20 Años y Rigor Técnico**
    * *Título:* `Atendido por su Dueña Especializada`
    * *Texto:* `Dos décadas de experiencia en cosmetología, drenaje y aparatología aplicada. Cada sesión es evaluada y ejecutada por la misma profesional, garantizando un seguimiento riguroso y personalizado de tu evolución.`
  * **Diferencial 4: Aval Oficial de Laboratorio Laca**
    * *Título:* `Distribuidora Oficial de Cosmética de Punta`
    * *Texto:* `Utilizamos y representamos oficialmente cremas, principios activos y sueros de Laboratorio Laca. Pureza dérmica certificada para potenciar cada resultado clínico y continuar tu cuidado en casa.`

---

### Sección 3: Hero Offer — Depilación Definitiva Láser Titanium (`#laser`)
* **Badge Destacado:**
  `SERVICIO ESTRELLA · TECNOLOGÍA PROPIA`
* **Título de Sección (`<h2>`):**
  `Depilación definitiva Láser Titanium en Chacras de Coria: sesiones rápidas, indoloras y para todo el año`
* **Bajada de Sección:**
  `Olvidate de las fechas restrictivas y del dolor innecesario. Incorporamos la tecnología más eficiente del mercado en nuestro propio gabinete para ofrecerte una experiencia cómoda, segura y con resultados visibles desde las primeras sesiones.`
* **Ficha de Beneficios Clave:**
  * **Cabezal con Enfriamiento Continuo:** `Sistema de frío por contacto que minimiza la sensación térmica en la piel, permitiendo un tratamiento sumamente confortable e indoloro.`
  * **Disponibilidad Total por Equipo Propio:** `Al no depender de alquileres de aparatología, reservás tu sesión de lunes a sábado según tu conveniencia horaria, asegurando la continuidad del ciclo biológico del vello.`
  * **Protocolo 100% Unisex:** `Atención natural y profesional para hombres y mujeres. Tratamiento integral en zonas faciales, corporales completas, espalda, pecho, barba o piernas, adaptando la potencia a cada tipo de folículo.`
  * **Apto para Todos los Fototipos de Piel:** `Tecnología trío que actúa eficazmente en pieles claras y bronceadas, permitiendo sostener el tratamiento de manera segura durante las cuatro estaciones.`
* **Microcopy de Confianza Preventiva:**
  `Te brindamos una pauta clara de cuidados previos y posteriores a la exposición solar para cuidar la salud de tu piel y evitar cualquier tipo de mancha o irritación.`
* **Llamado a la Acción Específico:**
  * **Texto del Botón:** `Consultar Turno de Láser Titanium`
  * **Micro-texto al pie:** `Reserva directa por WhatsApp · Asesoramiento personalizado de zonas y frecuencia.`

---

### Sección 4: Catálogo de Tratamientos Integrales (`#tratamientos`)
* **Eyebrow de Sección:**
  `CUIDADO INTEGRAL DE CABEZA A PIES`
* **Título de Sección (`<h2>`):**
  `Tratamientos faciales, corporales y bienestar: ciencia dérmica y relajación holística`
* **Bajada de Sección:**
  `Cada cuerpo y cada rostro tienen necesidades singulares. Combinamos aparatología de precisión con maniobras manuales y activos biológicos de primer nivel para restaurar la frescura, tonificar y disolver el estrés diario.`

#### Sub-bloque 4.1: Estética Facial & Dermocosmética
* **Título del Bloque:** `Cuidado Facial & Renovación Cutánea`
* **Descripción General:** `Protocolos diseñados para desintoxicar los poros, estimular la síntesis natural de colágeno y devolver luminosidad al rostro.`
* **Tratamientos Incluidos:**
  1. **Limpieza Profunda & Peeling Cosmetológico:** Higiene celular exhaustiva, exfoliación controlada y extracción delicada para eliminar impurezas, equilibrar el sebo y afinar los poros.
  2. **Radiofrecuencia Facial & Espátula Ultrasónica:** Onda térmica que tensa la piel, atenúa líneas de expresión y redefine el óvalo facial, complementada con vibración ultrasónica profunda.
  3. **Línea Dermocosmética Anti-Age Laboratorio Laca:** Nutrición intensiva con activos concentrados (ácido hialurónico, antioxidantes y péptidos tensores) avalados por formulación de laboratorio.
* **Microcopy Unisex:** `Tratamientos adaptados para todo tipo de piel, ideales para descongestionar el rostro tras semanas de trabajo o exposición ambiental.`
* **Botón de Consulta:** `Consultar Tratamientos Faciales`

#### Sub-bloque 4.2: Estética Corporal & Aparatología Avanzada
* **Título del Bloque:** `Remodelación Corporal, Reducción & Firmeza`
* **Descripción General:** `Soluciones no invasivas orientadas a movilizar adiposidad localizada, reducir celulitis y devolver firmeza al tejido muscular y dérmico.`
* **Tratamientos Incluidos:**
  1. **Ultracavitación & Radiofrecuencia Corporal:** Ultrasonido focalizado que disuelve depósitos grasos resistentes, combinado con estimulación térmica que combate la flacidez y alisa la textura cutánea.
  2. **Presoterapia Secuencial de Botas y Abdomen:** Masaje neumático continuo que activa la circulación de retorno, descongestiona piernas cansadas y optimiza el drenaje linfático integral.
  3. **Electroestimulación Muscular (Ondas Rusas / Cuadradas):** Tonificación de grupos musculares profundos para reafirmar glúteos, abdomen o piernas y definir el contorno corporal.
* **Microcopy:** `Sesiones progresivas con aparatología en regla y supervisión personalizada.`
* **Botón de Consulta:** `Consultar Tratamientos Corporales`

#### Sub-bloque 4.3: Terapias de Bienestar y Descarga Holística
* **Título del Bloque:** `Masajes Terapéuticos & Equilibrio del Alma`
* **Descripción General:** `El momento para desconectar de la rutina en un espacio de absoluto silencio, aromaterapia suave y manos experimentadas.`
* **Tratamientos Incluidos:**
  1. **Masajes Descontracturantes & Sedativos:** Alivio focalizado de tensiones en espalda, cuello, trapecios y cintura, devolviendo elasticidad a la fibra muscular y serenidad al sistema nervioso.
  2. **Masajes Relajantes & Reflexología Podal:** Maniobras fluidas combinadas con estimulación en puntos reflejos de los pies para armonizar órganos internos y aliviar la fatiga física.
  3. **Sesiones de Reiki Energético:** Terapia holística para desbloquear centros energéticos, calmar la sobrecarga mental y restaurar la vitalidad interna.
* **Microcopy Unisex:** `Espacio ideal para deportistas, profesionales con sobrecarga postural y cualquier persona que busque descanso genuino.`
* **Botón de Consulta:** `Coordinar Sesión de Masajes`

---

### Sección 5: El Consultorio (Atmósfera y Equipamiento) (`#consultorio`)
* **Eyebrow de Sección:**
  `UN REFUGIO EN CHACRAS DE CORIA`
* **Título de Sección (`<h2>`):**
  `La armonía de un espacio pensado exclusivamente para tu descanso`
* **Bajada de Sección:**
  `Nuestro consultorio privado sobre Av. San Martín te recibe con camilla confortable, fundas impolutas, luz natural serena y rigurosos protocolos de asepsia. Un entorno tranquilo y silencioso donde el cuidado personal es una pausa sagrada en tu día.`
* **Puntos Fuertes del Espacio:**
  * **Higiene y Desinfección Clínica:** Esterilización rigurosa de aparatología e instrumental antes de cada paciente.
  * **Cabina Individual a Puertas Cerradas:** Tu turno es tu espacio propio; jamás habrá interrupciones externas ni tránsito de terceros.
  * **Equipamiento Instalado en Sala:** Gabinete equipado con torre de insumos, lupa de trabajo y aparatología propia lista para operar.
* **Slot Reservado para Casos Reales (Placeholder Text):**
  * *Texto:* `Seguimiento de Resultados: Evaluamos el progreso sesión a sesión con fotografías de control privado para que compruebes la evolución de tu piel y contorno corporal.`

---

### Sección 6: Preguntas Frecuentes (FAQ Interactivo) (`#faq`)
* **Eyebrow de Sección:**
  `TRANSPARENCIA Y CONFIANZA`
* **Título de Sección (`<h2>`):**
  `Preguntas frecuentes sobre turnos, tratamientos y protocolos`
* **Bajada de Sección:**
  `Despejamos tus principales dudas antes de tu primera visita para que reserves tu turno con total tranquilidad.`

#### Acordeón de 5 Preguntas y Respuestas Exactas:

1. **¿Los tratamientos son tanto para hombres como para mujeres?**
   * *Respuesta:* `Sí, absolutamente. En M&E Estética y Salud todos nuestros tratamientos son 100% unisex. Atendemos a hombres y mujeres sin ningún tipo de distinción: desde depilación definitiva de espalda, barba o piernas, hasta limpiezas faciales profundas y masajes descontracturantes. El cuidado del cuerpo, la piel y el bienestar es un derecho y una necesidad de todos.`

2. **¿El tratamiento de depilación con Láser Titanium genera dolor o quemaduras?**
   * *Respuesta:* `No. La tecnología Láser Titanium cuenta con un cabezal refrigerado de enfriamiento continuo por contacto, lo que neutraliza la sensación de calor y convierte la sesión en un procedimiento sumamente confortable e indoloro. Además, adaptamos la intensidad y los parámetros a tu sensibilidad dérmica para que disfrutes de una experiencia segura y sin molestias.`

3. **¿Con qué frecuencia se coordinan las sesiones y qué disponibilidad de turnos tienen?**
   * *Respuesta:* `Una de nuestras mayores ventajas es que disponemos de aparatología propia en consultorio fijo, sin depender de máquinas alquiladas por fechas aisladas. Esto significa que podemos coordinar tus sesiones en el día y horario que mejor te convenga de lunes a sábado, respetando con exactitud los intervalos biológicos ideales para que cada tratamiento sea sumamente eficaz.`

4. **¿Qué precauciones debo tener con la exposición al sol durante el tratamiento?**
   * *Respuesta:* `La salud de tu piel es lo primero. En el caso de la depilación definitiva o de peelings cosmetológicos, te indicamos evitar la exposición solar directa 48 a 72 horas antes y después de cada sesión, además de mantener un uso constante de protector solar con factor adecuado. De esta manera prevenimos manchas dérmicas e irritaciones, asegurando que el tejido cicatrice y regenere de forma óptima.`

5. **¿Cómo se realiza la reserva de turnos y cuáles son los medios de pago disponibles?**
   * *Respuesta:* `Para garantizar que cada paciente cuente con el consultorio a su entera disposición y sin esperas, atendemos exclusivamente con turno previo acordado vía WhatsApp. Podés abonar mediante transferencia bancaria, billeteras virtuales (Mercado Pago) o efectivo al momento de tu sesión. Al confirmar tu horario, te brindamos la ubicación exacta y las indicaciones para tu llegada.`

---

### Sección 7: Ubicación y Contacto Directo (`#contacto`)
* **Eyebrow de Sección:**
  `COORDINÁ TU VISITA`
* **Título de Sección (`<h2>`):**
  `Te esperamos en el corazón de Chacras de Coria`
* **Bajada de Sección:**
  `Un consultorio de fácil acceso, estacionamiento cómodo en las inmediaciones y la calidez de una atención que prioriza tu tiempo.`
* **Ficha de Datos de Contacto:**
  * **Dirección:** `Av. San Martín 5355, Chacras de Coria, Luján de Cuyo, Mendoza`
  * **Modalidad de Atención:** `Exclusivamente con turno previo programado (sin sala de espera compartida).`
  * **Días y Horarios:** `Lunes a Sábados de 09:00 a 20:00 hs.`
  * **WhatsApp de Reservas:** `+54 9 261 681-7621`
  * **Instagram Oficial:** `@mye_esteticasalud`
* **Llamado a la Acción Principal:**
  * **Texto del Botón:** `Escribir por WhatsApp para Coordinar Turno`
  * **Microcopy:** `Respondemos a la brevedad para coordinar tu cita según tu disponibilidad horaria.`

---

### Sección 8: Footer Institucional (`#footer`)
* **Logo en Footer:** `M&E Estética y Salud`
* **Bajada Institucional:**
  `Consultorio privado de estética avanzada, dermocosmética y bienestar holístico en Chacras de Coria, Mendoza. 20 años dedicados al cuidado consciente y personalizado de tu cuerpo.`
* **Enlaces Rápidos de Navegación:**
  * `Diferenciales` (`#diferenciales`)
  * `Láser Titanium` (`#laser`)
  * `Tratamientos Faciales & Corporales` (`#tratamientos`)
  * `El Consultorio` (`#consultorio`)
  * `Preguntas Frecuentes` (`#faq`)
  * `Contacto` (`#contacto`)
* **Canales Digitales:**
  * `Instagram: @mye_esteticasalud`
  * `WhatsApp: +54 9 261 681-7621`
* **Aviso de Salud / Legal:**
  `Los tratamientos estéticos y cosmetológicos ofrecidos no reemplazan el diagnóstico ni el tratamiento médico dermatológico. Cada protocolo es evaluado de forma individual.`
* **Créditos y Derechos:**
  `© 2026 M&E Estética y Salud. Todos los derechos reservados. Desarrollado con excelencia por WAFLERS.`

---

### Componente Flotante: WhatsApp Floating Action Button (FAB)
* **Tooltip Flotante (Hover / Micro-interacción):**
  `¿Tenés dudas o querés agendar? Escribinos por WhatsApp.`
* **Texto Accesible (`aria-label`):**
  `Abrir conversación de WhatsApp con M&E Estética y Salud`
* **Enlace:** `https://wa.me/5492616817621?text=Hola%2C%20me%20comunico%20desde%20la%20web%20de%20M%26E%20Est%C3%A9tica%20y%20Salud%20para%20consultar%20por%20turnos%20disponibles.`
