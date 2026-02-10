Confidence and Risk Index (CRI)
Whitepaper técnico preliminar

Versión 0.1 — Enero 2026
Resumen ejecutivo

El Confidence and Risk Index (CRI) es un indicador cuantitativo diseñado para evaluar simultáneamente dos dimensiones fundamentales del comportamiento de un activo financiero:

    Confidence: estabilidad, direccionalidad y coherencia del movimiento reciente.

    Risk: variabilidad, aceleración y sensibilidad a cambios bruscos.

El CRI combina estas dimensiones en un índice sintético, normalizado y reproducible, construido para ser transparente, auditable y adecuado para validación académica.
1. Introducción

Los indicadores tradicionales de riesgo suelen centrarse en una única dimensión: volatilidad, drawdown, VaR o medidas de dispersión. Sin embargo, los mercados financieros presentan dinámicas donde la confianza (persistencia direccional) y el riesgo (variabilidad) interactúan de forma no lineal.

El CRI nace con tres objetivos:

    Unificar ambas dimensiones en una métrica interpretable.

    Mantener trazabilidad completa del proceso de cálculo.

    Permitir comparaciones entre activos y horizontes temporales.

2. Fundamentos conceptuales
2.1. Dimensión de Confidence

Evalúa la coherencia del movimiento reciente del activo. Se basa en:

    Momentum: dirección media del cambio.

    Tendencia: pendiente estimada mediante regresión lineal móvil.

    Persistencia: estabilidad relativa de la dirección.

La hipótesis subyacente:
Un activo con movimiento direccional claro y estable presenta mayor “confianza”.
2.2. Dimensión de Risk

Evalúa la sensibilidad del activo a cambios bruscos. Se basa en:

    Volatilidad: dispersión de los retornos.

    Aceleración: variación de la pendiente.

    Inestabilidad local: ruido relativo.

3. Metodología del CRI

El CRI se construye en tres etapas.

3.1. Cálculo de métricas base
Retornos simples
```
r_t = (P_t - P_{t-1}) / P_{t-1}
```
Volatilidad móvil
```
σ_t = sqrt( (1/n) * Σ (r_{t-i} - r̄)^2 )
```
Momentum
```
M_t = P_t - P_{t-n}
```
Tendencia (regresión lineal móvil)
```
P_t = α + βt + ε_t
```
3.2. Normalización
```
X_norm = (X_t - min(X)) / (max(X) - min(X))

```
3.3. Combinación sintética
```
CRI_t = w_c * C_t + w_r * (1 - R_t)

```
donde:

    C_t = dimensión de Confidence

    R_t = dimensión de Risk

    w_c, w_r = pesos (por defecto 0.5 / 0.5)

4. Interpretación del CRI

    CRI cercano a 1 → movimiento estable, direccional y con bajo riesgo.

    CRI cercano a 0 → movimiento errático, volátil o sin dirección.

    CRI intermedio → situaciones mixtas.

5. CRI Universe: extensión multiactivo

Permite:

    Comparativas entre activos

    Rankings dinámicos

    Mapas de riesgo-confianza

    Series temporales paralelas

6. Propiedades del indicador

    Transparencia: componentes explícitos y auditables.

    Reproducibilidad: cálculo determinista.

    Robustez: métricas complementarias.

    Interpretabilidad: descomposición clara.

7. Limitaciones

    No es un modelo predictivo.

    La normalización depende del rango histórico.

    Cambios estructurales pueden requerir recalibración.

    No sustituye análisis fundamental.

8. Futuras extensiones

    Métricas auxiliares (entropía, skewness, volatilidad fractal).

    Validación estadística formal.

    Integración con datasets alternativos.

    Versión CRI‑X multihorizonte.

    Paper académico completo.

9. Conclusión

El CRI ofrece una aproximación equilibrada y transparente para evaluar simultáneamente la confianza y el riesgo en series financieras. Su diseño modular y auditable lo hace adecuado para investigación académica y análisis cuantitativo profesional.

Este whitepaper preliminar establece los fundamentos metodológicos que guiarán su evolución futura.












