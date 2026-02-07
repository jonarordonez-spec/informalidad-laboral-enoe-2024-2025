# Análisis de Informalidad Laboral Femenina  
## Replicación de Stata en Python (ENOE T3 2024 vs T3 2025)

**Autor:** Jonathan Ruiz Ordoñez  
**Licencia:** MIT (ver archivo LICENSE)

### Descripción

Este repositorio contiene la replicación en Python de un análisis econométrico sobre informalidad laboral femenina, utilizando datos de la Encuesta Nacional de Ocupación y Empleo (ENOE) del INEGI para el tercer trimestre de 2024 y 2025.  

El análisis original se realizó en Stata y se reproduce aquí mediante regresión logística con pesos de expansión y ajuste por clúster en unidades primarias de muestreo (UPM). Incluye pruebas de diagnóstico, odds ratios, robustez mediante bootstrap y comparación con random forest.  

Los resultados se enfocan en la relación entre rangos de ingreso mensual y probabilidad de informalidad, con visualización gráfica.

### Conferencia y Colaboración Académica

Este trabajo fue presentado en la conferencia  
**"Las sombras vigentes del género en la informalidad laboral"**  
Impartida el 22 de enero de 2026, organizada por el Instituto Politécnico Nacional a través de la Sección de Estudios de Posgrado e Investigación de la Unidad Profesional Interdisciplinaria de Ingeniería y Ciencias Sociales y Administrativas (UPIICSA), en el marco del Grupo de Investigación Ciencias, Liderazgo y Empoderamiento Femenino.

La invitación fue realizada por la **Dra. Claudia Alejandra Hernández Herrera**. La presentación fue un esfuerzo colaborativo con:

- Dra. Eva Aide Torres Ortega  
- Dra. Orieta Iveth Flores Ahumada  
- Dra. Cristina Cabrera Ramos  

Enlace al video de la conferencia:  
https://www.youtube.com/watch?v=6nfatpBG0D0&t=712s  
(Canal: Gender y mas)

### Metodología

El análisis sigue los siguientes pasos:

1. Carga y combinación de datos de ENOE T3 2024 y T3 2025.  
2. Filtrado de mujeres ocupadas de 15 años o más.  
3. Construcción de la variable de informalidad basada en reglas definidas.  
4. Creación de rangos de ingreso, excluyendo valores faltantes.  
5. Análisis exploratorio de datos (EDA) para verificar distribuciones y calidad.  
6. Estimación de modelo logístico con pesos de expansión y ajuste por clúster (UPM).  
7. Pruebas de diagnóstico: multicolinealidad (VIF) y heteroscedasticidad (Breusch-Pagan).  
8. Cálculo de odds ratios para interpretación de efectos.  
9. Evaluación de robustez mediante bootstrap (intervalos de confianza).  
10. Comparación con un modelo de random forest.  
11. Visualización de probabilidades marginales ajustadas, conclusiones y limitaciones.

### Estructura del Repositorio

- `analisis_informalidad.ipynb` → Notebook principal con código y resultados.  
- `probabilidades_ajustadas.xlsx` → Probabilidades marginales ajustadas.  
- `Grafica_Informalidad_Femenina_Final.png` → Gráfica de barras comparativa.  
- `requirements.txt` → Dependencias del proyecto.  
- `LICENSE` → Licencia MIT.  
- `README.md` → Este archivo.

### Instalación y Ejecución

1. Clonar el repositorio:  
   git clone https://github.com/tu-usuario/informalidad-laboral-enoe-2024-2025.git

2. Instalar dependencias:  
   pip install -r requirements.txt

3. Abrir el notebook:  
   jupyter notebook analisis_informalidad.ipynb

### Agradecimientos

Este análisis fue posible gracias a la colaboración académica y la oportunidad de presentación en la conferencia organizada por el Instituto Politécnico Nacional.  

Agradezco especialmente a:

- Dra. Claudia Alejandra Hernández Herrera por la invitación y coordinación.  
- Dra. Eva Aide Torres Ortega  
- Dra. Orieta Iveth Flores Ahumada  
- Dra. Cristina Cabrera Ramos  

por su apoyo, orientación y participación conjunta en el proyecto "Las sombras vigentes del género en la informalidad laboral" (22 de enero de 2026, UPIICSA-IPN).  

Su experiencia y visión enriquecieron significativamente este trabajo.

### Licencia y Protección

Copyright © 2026 Jonathan Ruiz Ordoñez. Todos los derechos reservados.

Este trabajo está protegido bajo la licencia MIT (ver archivo LICENSE).  

Condiciones principales:  
- Uso, modificación y distribución permitidos únicamente con atribución obligatoria al autor y enlace al repositorio original.  
- Cualquier reproducción debe incluir el enlace al video de la conferencia y citar a los colaboradores.  
- Prohibido el uso comercial sin permiso escrito del autor.

En caso de uso no autorizado, se procederá conforme a la ley (DMCA en GitHub o notificación directa).