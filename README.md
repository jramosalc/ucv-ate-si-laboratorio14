Sistema Difuso para Evaluación de Prioridad de Beca
Descripción
Laboratorio del curso de Sistemas Inteligentes (Tercera Unidad). Implementación de un sistema de apoyo para priorizar solicitudes de beca basado en lógica difusa, considerando variables como promedio académico, asistencia, participación y situación económica.

Herramientas
Python

Jupyter Notebook

NumPy

Matplotlib

Scikit-Fuzzy

Entregables del Laboratorio
[x] Notebook ejecutado (sistema_difuso_beca.ipynb)

[x] Gráficos de conjuntos difusos

[x] Resultado defuzzificado

[x] Comparación contra regla rígida

[x] Desarrollo del reto MIT

[x] Respuestas a preguntas de análisis

[x] Conclusión final

20. Preguntas de análisis
1. ¿Qué diferencia existe entre lógica clásica y lógica difusa?
La lógica clásica (booleana) solo admite dos valores de verdad: verdadero (1) o falso (0); un elemento pertenece o no pertenece a un conjunto. La lógica difusa admite grados de pertenencia continuos entre 0 y 1, permitiendo representar conceptos imprecisos del lenguaje natural de forma más realista.

2. ¿Qué es un grado de pertenencia?
Es un valor numérico entre 0 y 1 que indica en qué medida un dato pertenece a un conjunto difuso determinado. Un grado de 0 significa que no pertenece en absoluto, 1 significa pertenencia total, y valores intermedios indican pertenencia parcial.

3. ¿Por qué un estudiante puede pertenecer parcialmente a dos conjuntos al mismo tiempo?
Porque las funciones de pertenencia se solapan en sus bordes. Por ejemplo, un promedio de 14 puede pertenecer simultáneamente al conjunto "bajo" y al conjunto "medio", reflejando que el límite entre categorías no es abrupto sino gradual.

4. ¿Qué representa la fuzzificación?
Es el proceso de convertir un dato numérico "nítido" (crisp) en sus grados de pertenencia a cada conjunto difuso definido para esa variable.

5. ¿Qué representa la defuzzificación?
Es el proceso de convertir el conjunto difuso resultante de la inferencia en un único valor numérico concreto (prioridad de beca). Se utiliza comúnmente el método del centroide.

6. ¿Qué regla difusa considera más importante en este laboratorio?
La regla: promedio alto & asistencia alta → prioridad alta, ya que combina los dos criterios académicos más objetivos y de mayor peso institucional.

7. ¿Qué diferencia encontró entre la lógica difusa y la regla rígida?
La regla rígida clasifica de forma binaria y es muy sensible a cambios cerca del umbral, pudiendo excluir a alguien por una centésima. El sistema difuso otorga una puntuación continua que refleja matices y evita saltos bruscos.

8. ¿Qué riesgos tendría usar este sistema para asignar becas reales?
El diseño de funciones de pertenencia puede incluir sesgos subjetivos, falta de transparencia ante apelaciones, exclusión de variables cualitativas importantes (contexto familiar) y el riesgo de tratar el resultado como una decisión automática definitiva sin supervisión humana.

9. ¿Qué variables adicionales agregaría para mejorar el sistema?
Situación económica familiar, número de dependientes, distancia al centro de estudios, participación en voluntariado y antecedentes de apoyos previos.

10. ¿En qué otros contextos se podría aplicar un sistema difuso?
Evaluación de riesgo crediticio, diagnóstico médico asistido, control de electrodomésticos inteligentes, sistemas de recomendación y control de tráfico.

21. Reto MIT: Inclusión de Situación Económica
Pregunta central: ¿El sistema se volvió más justo al considerar la situación económica?

Técnicamente, el sistema es ahora más sensible al contexto, permitiendo que estudiantes con méritos académicos similares pero distintas necesidades económicas reciban prioridades diferenciadas.

Éticamente, el sistema es más equitativo al reconocer que el mérito académico no ocurre en igualdad de condiciones. No obstante, la justicia final depende de:

La ponderación técnica otorgada a la variable económica frente al mérito.

La veracidad de los datos fuente.

La supervisión humana, siendo el sistema una herramienta de apoyo y no una decisión automática.

24. Conclusión final
El sistema difuso desarrollado permite priorizar becas con mayor flexibilidad que una regla rígida, evitando exclusiones arbitrarias cerca de los umbrales. La incorporación de la variable situacion_economica demostró que es posible elevar la equidad del sistema, reconociendo el contexto socioeconómico del estudiante. Sin embargo, el éxito del sistema depende críticamente del diseño de las reglas y la calidad de los datos, requiriendo siempre auditoría humana para evitar sesgos ocultos y garantizar una asignación justa.