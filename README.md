# ⚡ Analizador de Consumo Eléctrico & Comparador PVPC

[![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-blue.svg)](LICENSE)
[![HTML5 / Vanilla JS](https://img.shields.io/badge/Tecnología-HTML5%20%7C%20TailwindCSS%20%7C%20Chart.js-38B2AC.svg)](https://tailwindcss.com/)
[![PVPC API](https://img.shields.io/badge/Datos-Red%20Eléctrica%20de%20España%20(REE)-E53E3E.svg)](https://www.ree.es/)
[![Datadis](https://img.shields.io/badge/Integración-Datadis.es-059669.svg)](https://datadis.es/)

Herramienta web integral y gratuita para analizar el consumo horario de tu punto de suministro eléctrico (CUPS), comparar tu coste real entre la tarifa regulada **PVPC (Red Eléctrica de España)** y **tarifas del mercado libre por tramos**, simular facturas completas con impuestos y optimizar la recarga de **Vehículos Eléctricos (VE)**.

---

## 🌟 Características Principales

### 1. 📥 Métodos de Importación Flexibles
* **Archivos CSV de Distribuidoras**: Compatible con las exportaciones de curvas horarias de i-DE (Iberdrola), E-Distribución (Endesa), UFD (Naturgy), E-Redes, etc.
* **Integración Directa con Datadis.es**: Descarga tus lecturas horarias oficiales, datos identificativos de contrato (CUPS) y picos de potencia máximos directamente desde la API oficial.
* **Exportación a CSV**: Permite convertir lecturas descargadas de la API a formato CSV estándar.

### 2. ⚖️ Comparativa Económica Integral
* **Descarga Automática de Precios PVPC**: Conexión directa con la API de REE para obtener el precio oficial hora a hora del periodo analizado.
* **Hasta 6 Perfiles de Tarifas Manuales**: Configuración personalizada de precios y horarios Punta, Llano y Valle, fines de semana y festivos nacionales.
* **Simulador Completo de Factura**: Incluye término de potencia (P1 y P2), margen de comercialización, bono social, alquiler de contador, impuesto eléctrico (IE) e IVA.
* **Simulador de Hábitos de Consumo**: Permite simular qué ocurriría con tu factura si desplazaras ciertos porcentajes de tu consumo entre P1, P2 y P3.

### 3. 🚗 Análisis y Detección de Vehículo Eléctrico
* **Detección Automática de Cargas**: Filtrado por umbral de potencia horaria deduciendo el consumo base de la vivienda.
* **Métricas de Eficiencia**: Estimación de kilómetros recorridos, coste por km (€/km) tanto en energía neta como en coste final con impuestos incluidos.

### 4. 📊 Gráficas e Inteligencia de Precios
* **Precios del Día en Tiempo Real**: Curva horaria diaria con señalización de mínimos, máximos y comparativa frente a tu tarifa contratada.
* **Calendario Térmico Diario**: Mapa de calor por colores según el coste medio diario con acceso al perfil horario de cada día.
* **Evolución Cronológica y por Días de la Semana**: Visualiza qué días de la semana concentran mayor consumo y gasto.
* **Histórico y Tendencia Anual PVPC**: Gráfica interactiva de los 12 meses del año con análisis de precios mínimos, máximos y medias mensuales.
* **Recomendaciones de Horarios Óptimos (IA)**: Detección automática de las franjas horarias más baratas y más caras diferenciadas entre días laborables y fines de semana.

### 5. 🔒 Privacidad y Portabilidad
* **100% en el Navegador (Client-Side)**: Tus credenciales, curvas horarias y datos personales se procesan en local y nunca se almacenan en servidores externos.
* **Copia de Seguridad (.json)**: Exporta e importa toda tu configuración, perfiles de tarifas y datos de consumo con un solo clic.

---

## 🚀 Puesta en Marcha

No requiere instalación, Node.js ni compilación.

1. Clona el repositorio o descarga el archivo:
   ```bash
   git clone https://github.com/tu-usuario/analizador-consumo-electrico.git
