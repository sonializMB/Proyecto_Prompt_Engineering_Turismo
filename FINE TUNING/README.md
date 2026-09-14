# Fine Tuning de Mistral-7B para Reglamento de Becas UAT

Entrenamiento de un modelo de lenguaje (Mistral-7B) para responder 
preguntas sobre el Reglamento de Becas de la UAT.

## Diagrama

![Proceso](images/diagram.png)

## Uso

1. Abrir `Maestria-FT-Mistral-Presentacion.ipynb` en Colab
2. Configurar `HF_TOKEN` en Secrets
3. Ejecutar todas las celdas

## Tecnologías

- Mistral-7B (4-bit)
- LoRA (r=16)
- Unsloth + Transformers
- Google Colab

## Resultados

| # | Pregunta | ANTES | DESPUÉS |
|---|----------|-------|---------|
| 1 | ¿Qué tipos de becas se consideran en el reglamento? | Respuestas genéricas sobre tipos de becas | "Becas de posgrado, especialidad, maestría y doctorado" |
| 2 | ¿Quién firma el convenio de beca? | "La institución que otorga la beca..." | "El becario y la Universidad" |
| 3 | ¿El Comité de Becas solo otorga o también regula? | "Puede tener dos funciones..." | "No solo otorga, también regula" |
| 4 | ¿Las becas en el extranjero aplican a...? | "Pueden aplicar a estudiantes o profesores..." | "Aplican a profesores y estudiantes" |
| 5 | ¿Quién brinda asesoría para solicitudes? | "Los organismos que otorgan la beca..." | "La Dirección de Servicios Escolares" |
| 6 | ¿Qué debe exponer el profesor por escrito? | "Tema del día, contenido, actividades..." | "Los resultados de la evaluación de calidad" |
| 7 | ¿Hijos de profesores pueden acceder a becas? | "Depende de las políticas de cada país..." | "Sí, pueden acceder" |
| 8 | ¿El becario puede solicitar entrevista? | "Sí, por cualquier motivo..." | "No, solo para cambiar de carrera" |
| 9 | ¿Cada cuánto se comprueba aprobación? | "Depende de la institución..." | "Cada periodo escolar" |
| 10 | ¿Cancelación automática o caso por caso? | "No se aplica automáticamente..." | "Se evalúa caso por caso" |

## Autor

Ricardo De Jesus Bernal Montalvo
