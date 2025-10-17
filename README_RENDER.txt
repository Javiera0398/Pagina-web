
# Despliegue en Render

1. Subir este proyecto a un repositorio en GitHub:
   git init
   git add .
   git commit -m "Proyecto Salón de Belleza"
   git remote add origin https://github.com/usuario/repositorio.git
   git push -u origin main

2. Ir a https://render.com y crear un nuevo Web Service.

3. Configurar:
   - Build Command: pip install -r requirements.txt
   - Start Command: gunicorn app:app
   - Environment: Python 3.10

4. Añadir variables de entorno:
   - GMAIL_USER
   - GMAIL_PASSWORD
   - TWILIO_SID
   - TWILIO_TOKEN
   - TWILIO_WHATSAPP

5. Deploy y probar el endpoint /reservar
