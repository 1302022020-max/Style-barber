# Corte Ideal

App web (PWA) para barbería: se sube la foto del cliente, se detecta la forma del rostro
con MediaPipe (en el navegador, la foto no sale del celular) y se recomiendan cortes
según rostro, tipo de cabello y forma de cabeza.

## Subir a GitHub
```
git init
git add .
git commit -m "Corte Ideal"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/corte-ideal.git
git push -u origin main
```

## Desplegar en Render
1. New > Web Service > conecta el repositorio.
2. Runtime: Python 3
3. Build Command: `pip install -r requirements.txt`
4. Start Command: `gunicorn app:app`
5. Abre la URL (https) en el celular > menú del navegador > "Agregar a pantalla de inicio".

## Ajustar recomendaciones
Los cortes están en el objeto `CORTES` dentro de `static/index.html`.
Edítalos con los nombres y criterios de tu barbería.
