# 🎓 Sistema Difuso para Evaluación de Prioridad de Beca

> **Curso:** Sistemas Inteligentes | **Unidad:** Tercera Unidad  
> **Institución:** Universidad César Vallejo

---

## 📌 1. Descripción del Proyecto
Implementación de un sistema de apoyo para priorizar solicitudes de beca basado en **lógica difusa**. El sistema permite evaluar estudiantes considerando múltiples variables académicas y socioeconómicas, superando las limitaciones de los sistemas de decisión rígidos.

### 🛠 Herramientas Utilizadas
*   **Lenguaje:** Python
*   **Entorno:** Jupyter Notebook
*   **Librerías:** NumPy, Matplotlib, Scikit-Fuzzy, Pandas

---

## ✅ 2. Checklist de Entregables
- [x] Notebook ejecutado (`sistema_difuso_beca.ipynb`)
- [x] Definición de universos de discurso y conjuntos difusos
- [x] Gráficos de funciones de pertenencia
- [x] Sistema de 10+ reglas de inferencia
- [x] Resultados defuzzificados (5+ estudiantes)
- [x] Comparación contra regla rígida
- [x] Desarrollo del reto MIT (`situacion_economica`)
- [x] Respuestas a preguntas de análisis
- [x] Conclusión final

---

## 🧠 3. Preguntas de Análisis

**1. ¿Qué diferencia existe entre lógica clásica y lógica difusa?**  
La lógica clásica solo admite 0 o 1 (binaria), mientras que la difusa admite grados de pertenencia continuos, permitiendo representar conceptos imprecisos como "asistencia media" de forma realista.

**2. ¿Qué es un grado de pertenencia?**  
Es un valor entre 0 y 1 que indica la medida en que un dato pertenece a un conjunto difuso.

**3. ¿Por qué un estudiante puede pertenecer parcialmente a dos conjuntos al mismo tiempo?**  
Por el solapamiento de las funciones de pertenencia (trapezoidales/triangulares), lo cual modela transiciones graduales en lugar de límites abruptos.

**4. ¿Qué representa la fuzzificación?**  
Es el proceso de convertir un valor numérico "nítido" en sus grados de pertenencia a conjuntos difusos.

**5. ¿Qué representa la defuzzificación?**  
Es el proceso inverso: obtener un valor numérico concreto a partir de la inferencia difusa (usando habitualmente el método del centroide).

**6. ¿Qué regla difusa considera más importante en este laboratorio?**  
La regla `promedio alto & asistencia alta → prioridad alta`, por ser el criterio académico fundamental.

**7. ¿Qué diferencia encontró entre la lógica difusa y la regla rígida?**  
La lógica difusa suaviza los resultados, evitando la exclusión injusta de estudiantes que están cerca del umbral (ej. 15.9 vs 16).

**8. ¿Qué riesgos tendría usar este sistema para asignar becas reales?**  
Sesgos en el diseño de reglas, falta de transparencia/explicabilidad y el riesgo de omitir variables sociales críticas si no se supervisa humanamente.

**9. ¿Qué variables adicionales agregaría para mejorar el sistema?**  
Situación económica familiar, número de dependientes, costos de traslado y participación en voluntariado.

**10. ¿En qué otros contextos se podría aplicar un sistema difuso?**  
Evaluación de riesgo crediticio, diagnóstico médico, control industrial y sistemas de recomendación.

---

## 🚀 4. Reto MIT: Inclusión de Situación Económica

**Pregunta central: ¿El sistema se volvió más justo al considerar la situación económica?**

*   **Técnicamente:** El sistema es más sensible al contexto; permite que estudiantes con méritos similares pero distintas necesidades económicas obtengan prioridades diferenciadas.
*   **Éticamente:** El sistema es más equitativo al reconocer brechas socioeconómicas. Sin embargo, no garantiza justicia absoluta sin auditoría de los datos fuente, ponderación adecuada y supervisión humana para casos excepcionales.

---

## 💡 5. Conclusión Final
El sistema desarrollado demuestra que la lógica difusa permite una evaluación flexible y humana de los estudiantes. Al integrar la `situacion_economica`, el modelo evoluciona hacia una mayor equidad, evitando sesgos de exclusión propios de los sistemas rígidos. No obstante, su efectividad depende de la calidad de los datos y de la transparencia del comité al definir las reglas. Este sistema debe funcionar siempre como **soporte a la decisión humana**, nunca como un sustituto automático.