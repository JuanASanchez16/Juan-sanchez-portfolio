# Chatbot SegurPlus v6.0

Chatbot experimental para una aseguradora ficticia, desarrollado como proyecto academico para explorar asistentes conversacionales con RAG, triaje de urgencias y comportamiento agentico.

El objetivo principal de esta version es que el bot no responda igual ante cualquier consulta: primero evalua la gravedad del problema, adapta el tono y la longitud de la respuesta, y decide si debe informar, tramitar una asistencia o recomendar contactar con emergencias.

## Funcionalidades principales

- Triaje previo antes de pedir la poliza.
- Deteccion de emergencias extremas como fuego, fuga de gas o heridos graves.
- Diferenciacion entre emergencia extrema y urgencia no vital.
- Deteccion de gravedad: baja, media, alta y critica.
- Respuestas mas breves y directas en situaciones graves.
- RAG sobre catalogo de coberturas de seguros de hogar y coche.
- Tools simuladas para acciones internas:
  - enviar tecnico de hogar,
  - enviar grua,
  - registrar incidencia,
  - derivar a agente humano.
- Analisis estructurado de la incidencia.
- Resumen final del parte al cerrar la conversacion con `exit`.
- Proteccion basica de datos personales mediante anonimizado de PII.

## Flujo del chatbot

1. El usuario inicia una consulta.
2. El bot realiza un triaje previo.
3. Si hay peligro extremo, recomienda llamar al 112 o bomberos y no pide poliza.
4. Si la urgencia no es vital, solicita ramo y numero de poliza.
5. El bot consulta la base de conocimiento RAG.
6. Clasifica la gravedad de la incidencia.
7. Decide una accion interna simulada.
8. Al cerrar con `exit`, genera un resumen final de la incidencia.

## Ejemplos de prueba

Emergencia extrema:

```text
Huele mucho a gas en la cocina
```

Respuesta esperada: el bot recomienda llamar al 112 o bomberos y no pide poliza.

Urgencia no vital:

```text
Tengo una tuberia rota y se esta inundando la cocina
```

Respuesta esperada: el bot solicita poliza y tramita asistencia de hogar.

Incidencia de coche:

```text
El coche no arranca y necesito una grua
```

Respuesta esperada: el bot activa una asistencia de grua.

Cierre de conversacion:

```text
exit
```

Respuesta esperada: el bot muestra el resumen final de la incidencia.

## Tecnologias utilizadas

- Python
- Jupyter Notebook
- LangChain
- Groq / Llama 3.3
- FAISS
- HuggingFace Embeddings
- Pydantic

## Nota

Este proyecto es experimental y academico. No esta conectado a sistemas reales de emergencias, polizas ni asistencia de una aseguradora. En una situacion real de peligro, se debe contactar directamente con los servicios de emergencia.
