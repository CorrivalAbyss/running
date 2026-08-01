# 🏃 RunnersLog - Calculadora de Ritmos para Running

Una app bonita y dinámica para calcular tus ritmos de series y llevar un seguimiento de tus entrenamientos.

## ✨ Características

✅ **Calculadora bidireccional de ritmos**
- Introduce un tiempo en una distancia y obtén el ritmo por km
- Introduce tu ritmo objetivo y obtén los tiempos para diferentes distancias (100m a 1000m)

✅ **Calendario de seguimiento**
- Apunta tus series con distancia, tiempo y ritmo
- Visualiza un calendario con tus entrenamientos marcados
- Ve el historial de tus últimas series

✅ **Seguridad local**
- Protegida con contraseña
- Todos tus datos se guardan localmente en tu iPhone (sin nube)

✅ **Tema profesional de running**
- Diseño moderno y fluido
- Interfaz optimizada para iPhone

---

## 📱 Cómo instalar en iPhone

### Opción 1: Instalar como App (Recomendado)

1. **Descarga todos los archivos:**
   - `running-app.html`
   - `manifest.json`
   - `sw.js`

2. **Sube los archivos a un servidor web** o usa un servicio como:
   - Vercel (gratuito)
   - Netlify (gratuito)
   - GitHub Pages

3. **En tu iPhone:**
   - Abre el navegador Safari
   - Ve a la URL de tu app
   - Toca el botón de compartir (↑)
   - Selecciona "Añadir a pantalla de inicio"
   - Elige un nombre (ej: "RunnersLog")
   - ¡Listo! Aparecerá como una app en tu pantalla de inicio

### Opción 2: Usar localmente (Sin servidor)

Si solo quieres usarla en tu computadora:
- Abre el archivo `running-app.html` en tu navegador
- Funciona completamente offline

---

## 🚀 Uso

### Primera vez
1. Crea una contraseña segura
2. ¡Entra a la app!

### Calculadora: Tiempo → Ritmo
1. Introduce la distancia (ej: 400 metros)
2. Introduce el tiempo (ej: 1:12)
3. Toca "Calcular ritmo"
4. Obtendrás tu ritmo en min/km

### Calculadora: Ritmo → Splits
1. Introduce tu ritmo objetivo (ej: 4:30 min/km)
2. Toca "Calcular splits"
3. Verás los tiempos para todas las distancias de 100m a 1000m

### Calendario de Series
1. Selecciona un día en el calendario
2. Introduce la distancia, tiempo y ritmo
3. Toca "Guardar"
4. El día se marca en verde
5. Puedes ver tus últimas series en el historial

---

## 💾 Datos locales

- Contraseña hasheada en localStorage
- Todos los entrenamientos guardados localmente
- No se sincroniza con la nube (privado en tu iPhone)
- Si limpias el caché del navegador, perderás los datos

---

## 🔒 Seguridad

- Tu contraseña solo se guarda localmente
- Los datos de entrenamientos se almacenan de forma segura en tu dispositivo
- No hay conexión a internet requerida después de la instalación inicial

---

## 📋 Formato de entrada

**Tiempo:** `minuto:segundo` (ej: 1:12, 4:45, 0:45)
**Ritmo:** `minuto:segundo` (ej: 4:30, 5:00, 3:45)
**Distancia:** números en metros (ej: 400, 1200, 5000)

---

## 🎯 Ejemplos

### Ejemplo 1: Calcula tu ritmo de una serie
- Hiciste 400 metros en 1:12
- Distancia: 400
- Tiempo: 1:12
- Resultado: 3:00 min/km

### Ejemplo 2: Planifica splits para una serie
- Quieres correr a 4:30 min/km
- Ritmo: 4:30
- Verás:
  - 100m → 0:27
  - 200m → 0:54
  - 400m → 1:48
  - 600m → 2:42
  - 800m → 3:36
  - 1000m → 4:30

---

## 📞 Troubleshooting

**"No se instala como app"**
- Asegúrate de que está en HTTPS (no HTTP)
- Usa Safari, no otros navegadores
- Intenta limpiar el caché

**"Se borra mi contraseña"**
- No limpies el caché/datos de Safari
- La contraseña se guarda en localStorage

**"No funciona offline"**
- La primera carga debe ser online para que se descargue el service worker
- Luego funcionará sin conexión

---

¡Disfruta calculando tus ritmos de entrenamiento! 🏃‍♂️🏃‍♀️
