# Documento de contexto y selección del sistema

**Equipo:** Jose Martin Fuel, Kevin Almache y Felipe Montenegro.  
**Fecha de preparación:** 9 de octubre de 2026.  
**Duración académica de esta fase:** semanas 1 y 2.  
**Acuerdos:** los tres integrantes confirmamos la elección de correos internos y la organización del trabajo.

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

Esta comparación justifica la selección del equipo a partir del caso académico.

Correos internos permite demostrar posteriormente una petición desde una sede a un servidor en otra, proteger el acceso con autenticación y observar tiempos de respuesta o resultados de operaciones. Estas son posibilidades de medición; el instrumento, las variables, la muestra y los umbrales se definirán en fases posteriores.

## 4. Beneficio esperado y límites

Se espera facilitar la comunicación interna y ofrecer un entorno controlado para integrar software, red y seguridad. Estos beneficios todavía no están demostrados.

La solución académica se limita a dos sedes y a las operaciones mínimas de correos internos. No se ofrece correo público, integración con Gmail u Outlook, entrega SMTP externa, alta disponibilidad ni servicios en la nube. No se añade calendario, videollamada, archivos adjuntos ni búsqueda avanzada como compromisos iniciales.

Los entregables de esta fase son el documento de contexto y selección, la matriz de actores y responsabilidades, el contrato de comunicación, el repositorio con README y licencia preliminar y el video de presentación. Cada documento se presenta por separado. La declaración de integridad complementa la entrega. No se desarrolla la fase 2: no se redacta una especificación detallada de requisitos, casos de uso, diseño VLSM, arquitectura propia ni código.

## Documentos relacionados

La identificación inicial de usuarios y la distribución del equipo se presentan en la [matriz de actores, roles y responsabilidades](MATRIZ_ACTORES_ROLES.md). Los acuerdos de trabajo están en el [contrato de comunicación](CONTRATO_COMUNICACION.md).

## Fuente

“PROYECTO INTEGRADOR – TERCER NIVEL”, apartados 1 a 5, páginas 3 a 5, y apartado 6, fase 1, página 6.
