# Análisis de Modelos VAR y SVAR con Python: El Caso Peruano (2004-2025)

Este repositorio contiene la implementación técnica y el análisis econométrico desarrollado por **DataPolis** para estudiar la dinámica conjunta de variables macroeconómicas clave. 

## 📊 Descripción del Proyecto
El objetivo es capturar la interacción entre las expectativas de los agentes, la política monetaria y la actividad real sin imponer restricciones estructurales fuertes inicialmente.

### Variables Analizadas:
* **expec**: Expectativas económicas (Variable líder)[cite: 142, 1532].
* **tasa**: Tasa de interés nominal (Instrumento de política monetaria)[cite: 150, 153].
* **gpbi**: Crecimiento del Producto Bruto Interno[cite: 157, 158].
* **gipx**: Crecimiento de la inversión privada[cite: 166, 167].

## 🛠️ Metodología Aplicada
1. **Análisis de Series de Tiempo**: Pruebas de estacionariedad (ADF, KPSS) y test de Zivot-Andrews para quiebres estructurales[cite: 54, 71, 407].
2. **Cointegración**: Test de Johansen para determinar relaciones de largo plazo[cite: 618].
3. **Estimación**: Modelo VAR(2) en niveles, seleccionado mediante el criterio de información bayesiano (BIC)[cite: 509, 722].
4. **Identificación Estructural (SVAR)**: Uso de la descomposición de Cholesky para analizar el impacto de shocks estructurales[cite: 1138, 1222].

## 📈 Conclusiones Clave
* **Expectativas**: Actúan como una variable líder que anticipa movimientos en la actividad económica[cite: 1509, 1532].
* **Política Monetaria**: Muestra una alta persistencia y afecta significativamente a la inversión privada[cite: 1533].
* **Estabilidad**: El sistema es dinámicamente estable, con todas sus raíces dentro del círculo unitario[cite: 967].

## 💻 Requisitos
Para replicar este análisis, se requieren las siguientes librerías de Python:
- `pandas`
- `numpy`
- `statsmodels`
- `matplotlib`
- `seaborn`

---
**DataPolis** | Centro de Análisis Económico y de Políticas Públicas (Perú, 2026)
