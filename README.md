# camilladsp-EQ-comp-GUI
camilladsp parametric EQ / compressor / gain GUI in real-time use in parallel with camillagui with no gliches

# CamillaDSP Pro Master Console 🎛️

Una interfaz gráfica de usuario (GUI) avanzada y profesional construida con Python y PySide6 para controlar de forma remota **CamillaDSP**. Esta aplicación está diseñada para ingenieros de audio, audiófilos y entusiastas que buscan un control visual, rápido y preciso sobre su enrutamiento de audio, ecualización paramétrica y control dinámico.

## 🚀 Fortalezas y Características Principales

* **Control en Tiempo Real:** Visualiza vúmetros (VU meters) con respuestas instantáneas y controla las ganancias de tu hardware sin microcortes de audio.
* **Ecualizador Gráfico Interactivo:** Un motor matemático exacto dibuja la curva real de los filtros Biquad. Puedes crear, mover y ajustar el factor Q de tus filtros simplemente usando el ratón.
* **Auto-Compresión Dinámica:** Incluye una función inteligente que "escucha" un canal durante 5 segundos, analiza su rango dinámico y calibra automáticamente los tiempos de Ataque y Liberación (Attack/Release) del compresor.
* **Persistencia Inteligente:** La aplicación recuerda la última IP y Puerto utilizados, acelerando el flujo de trabajo en cada sesión.
* **Bilingüe:** Soporte nativo para alternar la interfaz entre Inglés y Español con un solo clic.
* **Interfaz Profesional (Dark Mode):** Diseñada para largas sesiones de estudio, con un esquema de colores oscuros, barras de desplazamiento dinámicas y elementos auto-ajustables (Responsive).

## 📋 Requisitos Previos

Para ejecutar esta aplicación, necesitas tener instalado Python 3.8 o superior, además de las siguientes librerías:

```bash
pip install PySide6 camilladsp
