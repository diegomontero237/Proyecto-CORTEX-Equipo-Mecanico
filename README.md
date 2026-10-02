# Proyecto-CORTEX-Equipo-Mecanico
##1. Perfil del agente

<img width="1919" height="962" alt="Captura de pantalla 2026-08-14 114418" src="https://github.com/user-attachments/assets/8840208e-ef96-4afd-9048-2eea6dbc0850" />
##2. Mapa De Procesos
<img width="1697" height="250" alt="Captura de pantalla 2026-08-21 113829" src="https://github.com/user-attachments/assets/0a4ce3a3-36fc-41c3-8c14-8a156ebc156e" />
Percepción y Atención: El sistema es excelente procesando fotos de piezas rotas, códigos de error en escáneres y analizando audios de motores. Pierde 3 puntos porque carece de los sentidos físicos indispensables en un taller: no puede oler gasolina mal quemada ni palpar la holgura de un rodamiento. Su diagnóstico depende totalmente de qué tan buena sea la información visual o auditiva que capture el celular del usuario.

Procesamiento Lingüístico: Traduce descripciones ambiguas o coloquiales (ej. "la moto se jalonea" o "suena como una matraca") a términos técnicos precisos al instante. Pierde 1 punto simplemente porque podría requerir entrenamiento adicional para comprender la jerga de taller o regionalismos muy específicos de ciertas zonas.

Aprendizaje y Memoria: La retención de datos es el punto más fuerte de una IA. Puede consultar manuales de despiece, diagramas eléctricos y torques de apriete de múltiples marcas simultáneamente, sin olvidar ni confundir una sola métrica. Supera ampliamente cualquier capacidad de memoria humana.

Pensamiento y Razonamiento: Ejecuta árboles de diagnóstico y lógica deductiva sin cometer errores por sesgos o fatiga. Se le restan 3 puntos porque carece de razonamiento espacial físico y de la "malicia" de un mecánico veterano; si la motocicleta tiene alteraciones no oficiales (cables mal empatados o adaptaciones caseras), el sistema lógico choca con la realidad

Motivación, Cognición y Emoción: Soy un programa informático; no poseo emociones genuinas ni motivación intrínseca. Proporciono respuestas pacientes y educadas, pero esa empatía es puramente simulada para mejorar el servicio al cliente. Un puntaje bajo aquí es honesto y realista: asegura que el desarrollo de tu producto se enfoque en la eficiencia técnica, sin intentar fingir que el asistente "sufre" junto al usuario por la avería.

##. Semana 4 (. Inventario de Inputs)
<img width="1911" height="978" alt="Captura de pantalla 2026-08-28 115830" src="https://github.com/user-attachments/assets/790ac15d-3c55-4edd-967b-5e09ffcc6dd3" />
##. Semana 5 (El Flujo de Procesamiento)
<img width="1200" height="682" alt="image" src="https://github.com/user-attachments/assets/a89aeb05-6b94-4ffd-a45e-efbbcae72a8f" />

## 2.Arquitectura de atencion con las reglas logicas definidas
RUIDO En la arquitectura de nuestro Gatekeeper, el ruido se refiere a las entradas de datos basura, ambigüedades, desvíos conversacionales e información irrelevante que los usuarios ingresan y que el sistema debe ignorar o limpiar antes del diagnóstico para evitar confusiones.

REGLAS DE ATENCION:Para definir las reglas de atencion,el sistema debe primero limpiar de la entrada del usuario todo el ruido conversacional, las historias de relleno y los datos vagos para extraer exclusivamente la información técnica relevante,despues debe exigir de forma obligatoria los datos clave de la máquina (marca, modelo, cilindrada y alimentación), antes de emitir cualquier concepto, activar un protocolo de emergencia que ordene la detención inmediata ante fallas críticas de frenos o fugas de combustible,prohibir guías sobre modificaciones peligrosas o ilegales, nunca dar informacion que haga probable un fallo mayor y termine en accidente o mas fallos para la moto

## 3. Arquitectura de Memoria (SEMANA ·7)
# Arquitectura de Memoria a Largo Plazo (LTM) - Asistente Mecánico de Motos

| Tipo de Memoria | Categoría de Datos | Descripción | Ejemplo de Entrada / Referencia |
| :--- | :--- | :--- | :--- |
| **Semántica (LTM)** | Manuales, Libros y Fuentes Bibliográficas | Repositorio de manuales de taller oficiales (OEM), guías de diagnóstico de marcas y literatura técnica de referencia como el Manual Arias-Paz de Motocicletas. | `"¿En qué parte del manual de taller oficial de la Yamaha FZ indica cómo cambiar el aceite?"` |
| **Semántica (LTM)** | Especificaciones Técnicas y Catálogos | Base de datos con medidas estándar, tolerancias de fábrica, pares de apriete (torques), calibración de bujías y viscosidades de aceites. | `"¿Qué tipo de aceite usa la moto y cada cuánto se cambia según las especificaciones?"` |
| **Semántica (LTM)** | Leyes Físicas, Fórmulas y Modelos Matemáticos | Fórmulas básicas de ingeniería, termodinámica, relación de compresión y electricidad aplicadas al diagnóstico de fallas mecánicas. | `"¿Cómo se calcula el torque para apretar la culata o la llanta correctamente?"` |
| **Episódica (LTM)** | Perfil del Vehículo y Estado Actual | Datos específicos de la motocicleta del usuario guardados en la app, como el modelo exacto, año y kilometraje actual. | `"Mi moto es una Yamaha FZ 150, modelo 2023, y tiene 15,000 kilómetros recorridos"` |
| **Episódica (LTM)** | Historial de Mantenimientos y Síntomática | Registro cronológico de lo que el usuario le conversó al bot en sesiones pasadas sobre fallas previas o repuestos cambiados. | `"Ayer te conté que la moto botaba humo blanco al encender en frío y revisamos los sellos"` |
