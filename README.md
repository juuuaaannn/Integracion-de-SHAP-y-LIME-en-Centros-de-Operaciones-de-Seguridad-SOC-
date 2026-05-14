# Integración de SHAP y LIME para mejorar la eficiencia en la detección de amenazas en la gestión de alertas en Centro de Operaciones de Seguridad
**Autor:** Juan Carlos Matias Gonzales Avendaño  
**Curso:** Inteligencia Artificial II  
**Universidad:** Universidad Nacional de Ingeniería — Facultad de Ingeniería Eléctrica y Electrónica

---

## Descripción

Estudio experimental que integra SHAP y LIME sobre un clasificador XGBoost entrenado 
con logs reales de servidor y aplicación para detectar anomalías en un Centro de 
Operaciones de Seguridad (SOC),, reduciendo la fatiga por alertas del analista mediante explicaciones locales y globales. 
Se alcanzan Accuracy=98.07% y AUC-ROC=99.52% utilizando únicamente tres features estructurales extraídos de logs crudos.

---

## Dataset

Los datos utilizados son logs reales crudos disponibles en el servidor institucional:  
🔗 https://uni-logs.us-mia-1.linodeobjects.com/list.html

Archivos utilizados:
- `logserver.tar.gz` — Registros del sistema operativo/servidor
- `logsapp.tar.gz` — Registros de eventos de aplicación

Colocar ambos archivos en la misma carpeta que el notebook antes de ejecutar.

---

## Estructura del Repositorio

```
├── experimento_shap_lime_soc.ipynb   # Código fuente con resultados visuales
├── fuentes/                           # PDFs de las 10 referencias bibliográficas
└── README.md                          # Documentación del proyecto y link al dataset
```

---

## Instalación y Ejecución

```bash
pip install xgboost shap lime scikit-learn pandas numpy matplotlib seaborn
```

Luego abrir `experimento_shap_lime_soc.ipynb` en VS Code o Jupyter y ejecutar las celdas en orden.

---

## Resultados Principales

| Métrica | Valor |
|---|---|
| Accuracy | 98.07% |
| Precision | 90.34% |
| Recall | 97.20% |
| F1-Score | 93.64% |
| AUC-ROC | 99.52% |
