# R-Citigroup-Volatility-Arch-Garch

## Descripción

Análisis de la volatilidad en los rendimientos de las acciones de Citigroup (C) utilizando modelos ARCH y GARCH. El estudio modela la varianza condicional de los rendimientos y pronostica la volatilidad futura, considerando eventos clave como la crisis financiera de 2008 y la separación de Banamex.

## Objetivos

- Detectar efectos ARCH en los rendimientos de Citigroup
- Modelar la volatilidad mediante ARCH(1) y GARCH(1,1)
- Pronosticar la volatilidad condicional a futuro
- Analizar el impacto de eventos financieros en la varianza

## Datos

- Ticker: C (Citigroup)
- Fuente: Yahoo Finance via `quantmod`
- Periodo: Enero 2000 - Abril 2025
- Frecuencia: Mensual
- Variable: Rendimientos del precio de cierre
- Eventos clave: Crisis 2008, COVID-19, Separación Banamex

## Metodología

### Análisis Exploratorio
- Pruebas de estacionariedad (ADF)
- Análisis de autocorrelación (ACF)
- Distribución de rendimientos

### Detección ARCH
- Prueba LM de efectos ARCH
- Significancia estadística de heterocedasticidad

### Modelado Volatilidad
- **ARCH(1)**: Modelo básico de heterocedasticidad
- **GARCH(1,1)**: Modelo generalizado con persistencia
- Validación de residuos y supuestos

### Pronósticos
- Pronóstico de volatilidad condicional
- Intervalos de confianza
- Análisis de persistencia

## Resultados

- Rendimientos estacionarios (p-value = 0.01)
- Media constante pero varianza cambiante
- Alta volatilidad durante crisis 2008-2009
- Pronóstico estable de volatilidad futura

## Autor

- José Luis Corona López

## Referencias

- Banamex. Separación Banamex-Citi. https://www.banamex.com/separacion-banamex-citi.html
- La Política Online. (2024, 18 de marzo). Ante la incertidumbre del mercado, Citi ahora aplaza la salida a bolsa de Banamex hasta 2026. https://www.lapoliticaonline.com/mexico/economia-mx/ante-la-incertidumbre-del-mercado-citi-ahora-aplaza-la-salida-a-bolsa-de-banamex-hasta-2026/
- Sorkin, A. R. (2010). The role of Citigroup in the 2008 financial crisis: An analysis of systemic risk. Journal of Financial Crises, 2(1), 35-50. Yale University. https://elischolar.library.yale.edu/cgi/viewcontent.cgi?article=1592&context=journal-of-financial-crises#:~:text=During%20the%20first%20three%20weeks,would%20constitute%20a%20systemic%20risk.
