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

## 3. Arquitectura de Memoria
# Arquitectura de Memoria a Largo Plazo (LTM) - Asistente Mecánico de Motos

Esta tabla define la estructura de almacenamiento y recuperación de conocimiento a largo plazo para el bot asistente de mecánica, dividida en Memoria Semántica (conocimiento universal, bibliográfico y técnico) y Memoria Episódica (historial de interacciones y perfil del vehículo).

| Tipo de Memoria | Categoría de Datos | Descripción | Ejemplo de Entrada / Referencia |
| :--- | :--- | :--- | :--- |
| **Semántica (LTM)** | Manuales, Libros y Fuentes Bibliográficas | Repositorio de manuales de taller oficiales (OEM), guías de diagnóstico de marcas (Yamaha, Honda, Suzuki, Bajaj) y literatura técnica de referencia (ej. Manual Arias-Paz de Motocicletas, bibliografía de ingeniería vehicular). | `"Fuente: Manual de Taller Oficial Yamaha FZ-16, Secc. 5-3: Diagnóstico del Sistema de Inyección y Códigos de Error ECU"` |
| **Semántica (LTM)** | Especificaciones Técnicas y Catálogos | Base de datos estructurada con tolerancias de fábrica, pares de apriete (torques), holguras de válvulas, tipos de bujías, viscosidades de aceites y capacidades volumétricas estándar por cilindrada. | `"Especificación: Tolerancia de desgaste de pastillas de freno: mín 1.5 mm; Torque de pernos de culata (Motor 150cc): 25 Nm"` |
| **Semántica (LTM)** | Leyes Físicas, Fórmulas y Modelos Matemáticos | Fórmulas de ingeniería aplicadas (dinámica de fluidos, termodinámica, cálculo multivariable, relación de compresión y leyes eléctricas) para la resolución de cálculos complejos de rendimiento mecánico. | `"Fórmula / Ley: Relación de Compresión CR = (Vd + Vc) / Vc; Ley de Ohm V = I * R para diagnóstico de caídas de voltaje en batería"` |
| **Episódica (LTM)** | Perfil del Vehículo y Estado Actual | Datos específicos de la motocicleta en atención: modelo exacto, año, kilometraje acumulado actual, modificaciones personalizadas y condiciones ambientales de operación habitual. | `"Registro Vehículo: ID_Usu_042, Moto: Yamaha FZ 150 (2023), Kilometraje: 15,200 km, Modificación: Tubo de escape deportivo libre"` |
| **Episódica (LTM)** | Historial de Mantenimientos y Síntomática | Registro cronológico de las sesiones pasadas del usuario con el bot: fallas reportadas previamente, diagnósticos entregados, refacciones cambiadas y fechas de intervención técnica. | `"Historial Sesión: Fecha: 2026-07-15. Síntoma previo: Humo blanco al encender en frío. Acción tomada: Verificación de sellos de válvula y cambio de aceite SAE 10W-40"` |
