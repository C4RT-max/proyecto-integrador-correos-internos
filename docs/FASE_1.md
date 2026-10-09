# Fase 1: contexto, planificación y organización

**Equipo:** Jose Martin Fuel, Kevin Almache y Felipe Montenegro.  
**Fecha de preparación:** 9 de octubre de 2026.  
**Duración académica de esta fase:** semanas 1 y 2.  
**Estado:** borrador preparado con asistencia de IA; requiere revisión del equipo. La elección de correos internos fue confirmada por el usuario.

## 1. Base del proyecto

Según los apartados 1 a 5 de la consigna, una empresa de soluciones tecnológicas abrió una segunda sede. El proyecto completo debe integrar comunicación entre sedes, servicios institucionales, autenticación, protección de información, evaluación cuantitativa e impacto social y organizacional.

Participan Programación Orientada a Objetos, Tecnologías de Comunicación en Red, Fundamentos de Seguridad, Probabilidad y Estadística, y Tecnología y Sociedad. La duración total es de 16 semanas; las primeras dos corresponden a esta fase.

La plataforma prevista debe combinar cliente-servidor en Go, autenticación FastAPI y una red con OpenWrt, VLAN, VLSM a partir de 10.10.0.0/16, OSPF y los demás servicios exigidos. Esta es la base obligatoria de la consigna: aquí no se decide direccionamiento, topología propia, modelo de datos ni implementación.

## 2. Problema y necesidad organizacional

La apertura de una segunda sede exige que los colaboradores puedan intercambiar mensajes institucionales entre ubicaciones, identificarse como usuarios autorizados y consultar la comunicación que les corresponde. La organización necesita que la aplicación y la infraestructura operen de manera integrada y que su desempeño pueda evaluarse con evidencia.

El problema que atenderemos es la necesidad de un medio interno de comunicación entre colaboradores de ambas sedes, con acceso autenticado y operaciones de mensajería acotadas.

**Distinción entre evidencia y propuesta:** la existencia de dos sedes y la necesidad de integración provienen del caso académico. El PDF no identifica una empresa real, cantidad de trabajadores, canales actuales, incidentes ni pérdidas. No afirmamos haber realizado entrevistas ni medido esas situaciones. La aplicación de correos internos es la solución seleccionada para este escenario.

## 3. Selección justificada

**Sistema elegido: gestión de correos internos.**

Permitirá intercambiar mensajes entre usuarios registrados, consultar bandeja de entrada y enviados, leer y eliminar mensajes. Esas operaciones proceden del alcance mínimo recomendado en la consigna. No requiere integración con SMTP externo.

| Alternativa admitida | Relación con la necesidad | Consideración para elegir |
| --- | --- | --- |
| Correos internos | Comunicación institucional entre colaboradores de ambas sedes | Permite mensajes asincrónicos y operaciones claras; opción seleccionada |
| Chat empresarial | Comunicación de texto entre usuarios autenticados | También encaja; demanda atención especial a sesiones y dinámica de conversación |
| Gestión de imágenes | Intercambio y organización de material visual | Requeriría justificar una necesidad específica de imágenes no descrita en el caso |
| Gestión de videos | Intercambio controlado de archivos audiovisuales | Requeriría justificar esa necesidad y atender almacenamiento y transferencia |

Esta comparación es una valoración del equipo propuesta para revisión, no un estudio de campo.

Correos internos permite demostrar posteriormente una petición desde una sede a un servidor en otra, proteger el acceso con autenticación y observar tiempos de respuesta o resultados de operaciones. Estas son posibilidades de medición; el instrumento, las variables, la muestra y los umbrales se definirán en fases posteriores.

## 4. Beneficio esperado y límites

Se espera facilitar la comunicación interna y ofrecer un entorno controlado para integrar software, red y seguridad. Estos beneficios todavía no están demostrados.

La solución académica se limita a dos sedes y a las operaciones mínimas de correos internos. No se ofrece correo público, integración con Gmail u Outlook, entrega SMTP externa, alta disponibilidad ni servicios en la nube. No se añade calendario, videollamada, archivos adjuntos ni búsqueda avanzada como compromisos iniciales.

En esta fase se entregan contexto y selección, actores y responsabilidades, contrato de comunicación, repositorio con README y licencia preliminar, tablero, declaración de integridad y preparación del video. No se desarrolla la fase 2: no se redacta una especificación detallada de requisitos, casos de uso, diseño VLSM, arquitectura propia ni código.

## 5. Actores y usuarios iniciales

| Actor | Relación con la propuesta | Necesidad o interés inicial |
| --- | --- | --- |
| Colaboradores de sede A | Usuarios de correos internos | Enviar y consultar mensajes autorizados |
| Colaboradores de sede B | Usuarios de correos internos | Comunicarse con la otra sede y consultar sus mensajes |
| Administración de TI | Actor técnico del escenario | Mantener servicios y accesos según responsabilidades que se definan después |
| Dirección de la empresa | Parte interesada | Coordinar ambas sedes y disponer de una solución viable |
| Equipo de tres estudiantes | Responsable del proyecto académico | Planificar, documentar y demostrar contribuciones |
| Docentes de las cinco asignaturas | Evaluadores y orientadores | Comprobar integración y cumplimiento de la consigna |

La administración de TI es un actor organizacional propuesto; no implica diseñar un rol de aplicación ni otorgarle acceso al contenido privado de los mensajes.

## 6. Matriz de roles y responsabilidades

Distribución propuesta, pendiente de ratificación. Responsable significa coordinar y consolidar; revisor significa comprobar y aportar. La carga técnica de fases futuras podrá ajustarse.

| Trabajo de fase 1 | Responsable | Revisor | Evidencia esperada |
| --- | --- | --- | --- |
| Contexto y necesidad organizacional | Jose Martin Fuel | Kevin Almache | Documento revisado y aporte identificable |
| Selección justificada del sistema | Jose Martin Fuel | Felipe Montenegro | Justificación acordada |
| Actores y distribución del equipo | Kevin Almache | Jose Martin Fuel | Matriz validada por los tres |
| Repositorio, README y tablero | Kevin Almache | Felipe Montenegro | URL accesible y seguimiento actualizado |
| Contrato de comunicación | Felipe Montenegro | Jose Martin Fuel | Acuerdo ratificado |
| Licencia, integridad y declaración de IA | Felipe Montenegro | Kevin Almache | LICENSE y declaración revisados |
| Guion y edición del video | Felipe Montenegro | Kevin Almache | Video claro con intervención de los tres |
| Exposición del problema y selección | Jose Martin Fuel | Los otros dos | Primer segmento del video |
| Exposición de organización y repositorio | Kevin Almache | Los otros dos | Segundo segmento del video |
| Exposición de ética, licencia y cierre | Felipe Montenegro | Los otros dos | Tercer segmento del video |
| Revisión y entrega de fase 1 | Los tres | Revisión cruzada | Checklist y entrega final |

Como referencia de coordinación del proyecto completo, Jose acompañará software; Kevin, infraestructura; Felipe, seguridad. El trabajo cuantitativo será compartido: Kevin apoyará las mediciones técnicas, Jose su relación con la aplicación y Felipe su documentación e interpretación. Tecnología y Sociedad será coordinada por Felipe con revisión de los tres. Estas responsabilidades no autorizan ejecutar las siguientes fases.

## 7. Plan de dos semanas

No se asignan fechas de calendario porque no se proporcionó el inicio oficial. D1 a D14 son días relativos de las semanas 1 y 2.

| Periodo | Actividad | Responsable | Resultado |
| --- | --- | --- | --- |
| Semana 1, D1–D2 | Leer la base y acordar contexto y aplicación | Jose + equipo | Contexto y selección revisados |
| Semana 1, D3 | Validar actores y responsabilidades | Kevin + equipo | Matriz ratificada |
| Semana 1, D4 | Acordar comunicación e integridad | Felipe + equipo | Contrato y declaración |
| Semana 1, D5–D7 | Crear repositorio, publicar README/licencia y organizar tablero | Kevin, con revisión de Felipe | Repositorio y seguimiento accesibles |
| Semana 2, D8–D10 | Revisar documentos y preparar presentación | Los tres | Guion y documentos coherentes |
| Semana 2, D11–D12 | Grabar y editar video breve | Los tres; edición Felipe | Video con participación equilibrada |
| Semana 2, D13 | Revisar enlaces, licencia, autoría y alcance | Los tres | Checklist sin omisiones |
| Semana 2, D14 | Entregar únicamente fase 1 | Los tres | Archivos y enlaces verificados |

## 8. Riesgos de organización y acciones

| Riesgo inicial | Acción de fase 1 | Responsable |
| --- | --- | --- |
| Dificultad para usar GitHub | Crear un repositorio común y practicar aportes pequeños con cuentas propias | Kevin |
| Reparto desigual del trabajo | Una tarea responsable y revisión cruzada; registrar aportes reales | Los tres |
| Avanzar a fases no solicitadas | Revisar el alcance antes de abrir nuevas tareas | Jose |
| Confundir borradores con resultados | Etiquetar propuestas y pendientes; no inventar pruebas ni entrevistas | Felipe |
| Retraso en el video | Ensayar D10 y reservar D11–D12 para grabación | Los tres |

## 9. Fuente y alcance de la lectura

Fuente: “PROYECTO INTEGRADOR – TERCER NIVEL”, apartados 1–5, páginas 3–5; apartado 6, fase 1, página 6. La figura de arquitectura de página 4 es referencia institucional, no diseño producido por el equipo. La consigna exige video breve, pero no fija duración: tres minutos es nuestra propuesta.
