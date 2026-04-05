# Manual de Usuario - CamillaDSP Pro Master Console

¡Bienvenido a CamillaDSP Pro Master Console! Esta aplicación está diseñada para ofrecerte un control visual y preciso sobre tu hardware de audio utilizando el motor de CamillaDSP.

A continuación, aprenderás cómo conectarte y utilizar todas las herramientas disponibles.

---

## 1. Inicio y Conexión

Al abrir la aplicación, verás la pantalla de inicio donde debes establecer la conexión con tu dispositivo.

1. **IP Servidor:** Ingresa la dirección IP de la máquina donde se está ejecutando CamillaDSP (por defecto `127.0.0.1` si es tu propia máquina).
2. **Puerto:** Ingresa el puerto configurado para la conexión WebSocket (por defecto `1234`).
3. Haz clic en **ESCANEAR HARDWARE**.
4. Si la conexión es exitosa, aparecerán los modos de trabajo:
   * **DEFAULT:** Edita los ecualizadores generales ya existentes.
   * **INPUT MODE:** Permite seleccionar pares de canales de entrada (estéreo) para ecualizar antes de la mezcla.
   * **OUTPUT MODE:** Permite seleccionar canales de salida individuales para ecualizar y comprimir.
5. Selecciona los canales deseados y haz clic en **INICIAR ESTUDIO**.

*(Nota: La aplicación recordará automáticamente la última IP y puerto que utilizaste con éxito para tu próxima sesión).*

---

## 2. Solapa: Vúmetros y Dinámica

En esta pestaña controlarás los niveles de volumen y la compresión de tus canales de audio en tiempo real.

### Vúmetros y Faders
* **Visualización:** Observa el nivel de audio (en dB) de tus entradas (izquierda) y salidas (derecha).
* **Mute (Silenciar):** Haz clic izquierdo sobre el nombre de un canal de salida para silenciarlo (el texto se pondrá rojo) o activarlo (verde).
* **Fader de Volumen:** Mantén presionado el clic izquierdo sobre la perilla azul y arrastra hacia arriba o abajo para ajustar la ganancia. El cambio se aplicará al soltar el clic.
* **Resetear Volumen:** Haz clic derecho en la zona del fader para volver a `0.0 dB` instantáneamente.
* **Invertir Fase (+/-):** Haz clic en este botón para invertir la polaridad del canal de salida en el mezclador.

### Compresor y Auto-Calibración
* **Crear Compresor:** Haz doble clic directamente sobre la barra de color de un vúmetro de salida. El lugar donde hagas clic establecerá el límite (Threshold) inicial.
* **Borrar Compresor:** Haz clic derecho sobre el vúmetro de salida que tenga un compresor activo.
* **Auto-Compresión:** En la tabla de la parte inferior, verás los compresores activos. Haz clic en el botón **AUTO**. La aplicación medirá el audio durante 5 segundos y ajustará matemáticamente los tiempos de Ataque (Attack) y Liberación (Release) ideales según la dinámica de tu música.
* **Edición Manual:** Puedes hacer doble clic en cualquier número de la tabla (Threshold, Ratio, Makeup, etc.) para escribir un valor exacto manualmente.

---

## 3. Solapa: Filtros y EQ

Aquí puedes esculpir el sonido utilizando una gráfica interactiva de alta precisión matemática.

### Controles del Gráfico (Ratón)
* **Añadir Filtro:** Haz doble clic en cualquier espacio negro vacío del gráfico para crear un nuevo punto de ecualización.
* **Mover / Ajustar:** Mantén presionado el clic izquierdo sobre un punto numerado y arrástralo. Moverlo a los lados cambia la Frecuencia (Hz) y moverlo arriba/abajo cambia la Ganancia (dB). Un cuadro flotante te mostrará los valores exactos y se acomodará automáticamente para no salirse de la pantalla.
* **Ajustar el Ancho (Factor Q):** Pon el cursor sobre un punto y gira la **Rueda del Ratón** hacia arriba o hacia abajo para hacer que el filtro sea más ancho o más agudo.
* **Borrar Filtro:** Haz clic derecho sobre el punto numerado que deseas eliminar.

### Tabla de Filtros
Justo debajo del gráfico, verás una tabla con todos tus filtros creados.
* Puedes cambiar el tipo de filtro usando el menú desplegable (Peaking, Highshelf, Lowpass, etc.).
* Puedes hacer doble clic en las celdas de Freq, Gain o Q para escribir los valores exactos mediante el teclado.
* Usa el botón **X** para eliminar un filtro.

---

## 4. Idioma y Ayuda
* **Botón EN / ES:** En la pantalla de inicio, haz clic aquí para alternar toda la interfaz entre Inglés y Español.
* **Ayuda:** Abre un resumen rápido de los controles del ratón.
