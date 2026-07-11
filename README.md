# 🎓 Laboratorio: Sistema Difuso para Evaluación de Prioridad de Beca

> **Curso:** Sistemas Inteligentes | **Unidad:** Tercera Unidad  
> **Institución:** Universidad César Vallejo

---

## 📌 1. Descripción del Proyecto
Implementación de un sistema de apoyo para priorizar solicitudes de beca basado en **lógica difusa**. El sistema procesa variables de desempeño académico y participación para generar una recomendación objetiva de prioridad.

### 🛠 Herramientas Utilizadas
*   **Lenguaje:** Python
*   **Entorno:** Jupyter Notebook
*   **Librerías:** NumPy, Matplotlib, Scikit-Fuzzy, Pandas

---

## ✅ 2. Checklist de Entregables
- [x] Notebook ejecutado (`sistema_difuso_beca.ipynb`)
- [x] Análisis del reto MIT (inclusión de `situacion_economica`)
- [x] Comparación técnica vs. Regla Rígida
- [x] Respuestas a preguntas de análisis
- [x] Conclusión final

---

## 🧠 3. Preguntas de Análisis

**1. ¿Qué diferencia existe entre lógica clásica y lógica difusa?**  
La lógica clásica es binaria (0 o 1), mientras que la difusa admite grados intermedios de verdad, permitiendo modelar la imprecisión del lenguaje humano.

**2. ¿Qué es un grado de pertenencia?**  
Es el valor (entre 0 y 1) que cuantifica cuánto pertenece un elemento a un conjunto difuso.

**3. ¿Por qué un estudiante puede pertenecer parcialmente a dos conjuntos al mismo tiempo?**  
Debido al solapamiento de las funciones de pertenencia (trapezoidales/triangulares), lo cual modela transiciones graduales en lugar de límites abruptos.

**4. ¿Qué representa la fuzzificación?**  
La conversión de valores numéricos ("nítidos") a grados de pertenencia en conjuntos difusos.

**5. ¿Qué representa la defuzzificación?**  
El proceso de obtener un valor numérico final a partir de la salida difusa (generalmente usando el método del centroide).

**6. ¿Qué regla difusa considera más importante en este laboratorio?**  
*Promedio alto & asistencia alta → prioridad alta*, por ser los indicadores de mayor peso académico.

**7. ¿Qué diferencia encontró entre la lógica difusa y la regla rígida?**  
La lógica difusa suaviza los resultados, evitando exclusiones injustas cerca de los límites que sí ocurren con las reglas rígidas.

**8. ¿Qué riesgos tendría usar este sistema para asignar becas reales?**  
Sesgos en el diseño de las funciones de pertenencia y falta de explicabilidad si no se auditan las reglas.

**9. ¿Qué variables adicionales agregaría para mejorar el sistema?**  
Situación socioeconómica, distancia de residencia y participación en voluntariado.

**10. ¿En qué otros contextos se podría aplicar un sistema difuso?**  
Diagnóstico médico, control industrial y sistemas de recomendación.

---

## 🚀 4. Reto MIT: Inclusión de Situación Económica

**Pregunta central: ¿El sistema se volvió más justo al considerar la situación económica?**

*   **Técnicamente:** El sistema se volvió más **sensible al contexto**, permitiendo que el mérito académico sea ponderado junto con la necesidad real.
*   **Éticamente:** Mejora la equidad, pero requiere auditoría constante para asegurar que los datos económicos sean veraces y no introduzcan nuevos sesgos.

---

## 💡 5. Conclusión Final
El sistema desarrollado demuestra que la lógica difusa ofrece un modelo más humano y flexible para la toma de decisiones. Al integrar la variable de situación económica, pasamos de una evaluación puramente académica a una **evaluación equitativa**. El sistema debe permanecer como una herramienta de soporte a la decisión humana, garantizando siempre la transparencia en sus reglas.

---
*Repositorio creado como producto final del laboratorio de Sistemas Inteligentes.*