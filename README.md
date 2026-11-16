[README.md](https://github.com/user-attachments/files/34943333/README.md)
# Simulador SCADA & PLC Industrial: Línea de Envasado y Control de Calidad
**Proyecto Demo B2B para Demostración a Socios e Inversionistas**

Este proyecto es un **Gemelo Digital y Simulador de PLC** en tiempo real para un proceso industrial repetitivo de alto valor: **Línea Automatizada de Envasado, Dosificado, Tapado y Rechazo Neumático por Visión Artificial**.

---

## 🚀 Cómo Enviar y Mostrar la Prueba a tus Socios

Tienes **4 formatos listos** para que tus partners puedan ingresar y probar el simulador de inmediato:

### Opción 1: Archivo Autónomo (Standalone) - La más rápida
- El archivo `index.html` es **100% autónomo** y no requiere instalar Node.js, Python ni servidores.
- **Cómo enviarlo**:
  1. Envía el archivo `index.html` directamente por WhatsApp, Telegram, Slack o correo electrónico.
  2. Tus socios solo deben hacer **doble clic** sobre el archivo y se abrirá al instante en cualquier navegador (Google Chrome, Microsoft Edge, Safari o Firefox).
  3. Funciona en Windows, Mac, Linux, tablets y teléfonos móviles con pantalla táctil.

### Opción 2: Enlace Web Gratuito en la Nube (URL con 1 Clic)
Si prefieres enviarles un link (ejemplo: `https://mi-empresa-plc.vercel.app`):
- **Vercel o Netlify**: Arrastra la carpeta `plc-industrial-simulator` a [vercel.com](https://vercel.com) o [netlify.com/drop](https://app.netlify.com/drop). En 10 segundos te generará un enlace público HTTPS seguro.
- **GitHub Pages**: Sube el archivo a un repositorio de GitHub y activa GitHub Pages en *Settings > Pages*.

### Opción 3: Servidor Local para Presentación en Vivo
Si vas a presentar la demo en una reunión por Google Meet, Zoom o Teams:
1. Abre una terminal en esta carpeta y corre:
   ```powershell
   python -m http.server 8080
   ```
2. Abre `http://localhost:8080` en tu navegador y comparte pantalla.

### Opción 4: Exportación a Software Industrial Real
Si tus socios son ingenieros de automatización o directores de planta:
- La arquitectura I/O y la lógica de peldaños Ladder implementada corresponde estrictamente al estándar **IEC 61131-3**.
- Es 100% trasladable a **Siemens TIA Portal (S7-1200 / S7-1500)**, **Rockwell Studio 5000 (Allen-Bradley)** o **CODESYS v3.5**.

---

## 🎯 Qué Pueden Probar tus Socios en el Simulador

1. **Dashboard SCADA & Métricas OEE**:
   - Conteo de unidades totales, unidades conformes y tasa de rechazo en tiempo real.
   - Velocidad de producción dinámica en PPM (botellas por minuto).
2. **Inyector de Fallas en Vivo**:
   - Botón `Inyectar Botella con Nivel Bajo`: La estación de visión artificial detecta la falta de volumen y activa el pistón de descarte `%Q0.5`.
   - Botón `Inyectar Botella Sin Tapa`: El PLC detecta la ausencia de tapa y expulsa la unidad defectuosa.
3. **Variador de Frecuencia (VFD)**:
   - Slider para cambiar la velocidad de la cinta de 20 Hz a 80 Hz y ver el impacto en la cadencia de producción.
4. **Monitor Ladder en Tiempo Real**:
   - Visualización de la corriente lógica energizando contactos `%I`, marcas `%M`, temporizadores `TON` y bobinas `%Q`.
5. **Exportación de Datos para ERP / MES**:
   - Botón para descargar un archivo `.csv` con la telemetría del turno de producción.
