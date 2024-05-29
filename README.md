```python
# Thief Raccoon - Herramienta de Phishing de Inicio de Sesión

Thief Raccoon es una herramienta diseñada con fines educativos para demostrar cómo se pueden llevar a cabo ataques de phishing en varios sistemas operativos. Esta herramienta tiene como objetivo crear conciencia sobre las amenazas de ciberseguridad y ayudar a los usuarios a comprender la importancia de medidas de seguridad como la autenticación de dos factores (2FA) y la gestión de contraseñas.

<a href="https://ibb.co/L0Zn2XP"><img src="https://i.ibb.co/3TCBL9s/Captura-de-pantalla-2024-05-23-111620.png" alt="Captura-de-pantalla-2024-05-23-111620" border="0"></a>

## Características

- Simulación de phishing para Windows 10, Windows 11, Windows XP, Windows Server, Ubuntu, Ubuntu Server y macOS.
- Captura de credenciales de usuario para demostraciones educativas.
- Pantallas de inicio de sesión personalizables que imitan sistemas operativos reales.
- Modo de pantalla completa para mejorar la simulación de phishing.

## Instalación

### Requisitos previos

- Python 3.x
- pip (instalador de paquetes de Python)
- ngrok (para exponer el servidor local a internet)

### Descargar e Instalar

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/davenisc/thief_raccoon.git
   cd thief_raccoon

2. Instalar python venv
   
   ```bash
   apt install python3.11-venv

3. **Crear venv:**

   ```bash
   python -m venv raccoon_venv
   source raccoon_venv/bin/activate

4. **Instalar las bibliotecas requeridas:**
   
   ```bash
   pip install -r requirements.txt

**Uso**

1. **Ejecutar el script principal:**
   
   ```bash
   python app.py

2. **Seleccionar el sistema operativo para la simulación de phishing:**

   Después de ejecutar el script, se presentará un menú para seleccionar el sistema operativo. Ingresa el número correspondiente al SO que deseas simular.

3. **Acceder a la página de phishing:**

   Si estás en la misma red local (LAN), abre tu navegador web y navega a http://127.0.0.1:5000.
   
   Si deseas que la página de phishing sea accesible por internet, usa ngrok.

Usando ngrok

1. **Descargar e instalar ngrok**

Descarga ngrok desde ngrok.com y sigue las instrucciones de instalación para tu sistema operativo.

2. **Exponer tu servidor local a internet:**

3. **Obtener la URL pública:**

Después de ejecutar el comando anterior, ngrok te proporcionará una URL pública. Comparte esta URL con tus sujetos de prueba para acceder a la página de phishing por internet.

**Cómo instalar Ngrok en Linux?**

1. Instala ngrok via Apt con el siguiente comando:

   ```bash
   curl -s https://ngrok-agent.s3.amazonaws.com/ngrok.asc \
      | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null \
      && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" \
      | sudo tee /etc/apt/sources.list.d/ngrok.list \
      && sudo apt update \
      && sudo apt install ngrok

2. Ejecuta el siguiente comando para agregar tu authtoken al ngrok.yml predeterminado

   ```bash
      ngrok config add-authtoken xxxxxxxxx--your-token-xxxxxxxxxxxxxx

**Despliega tu aplicación en línea**

3. Pon tu aplicación en línea en un dominio efímero que redirija a tu servicio upstream. Por ejemplo, si está escuchando en el puerto http://localhost:8080, ejecuta:

      ```bash
      ngrok http http://localhost:5000

**Ejemplo**

1. **Ejecutar el script principal:**
   
   ```bash
   python app.py


2. **Seleccionar Windows 11 del menú:**

   ```bash
   Selecciona el sistema operativo para el phishing:
   1. Windows 10
   2. Windows 11
   3. Windows XP
   4. Windows Server
   5. Ubuntu
   6. Ubuntu Server
   7. macOS
   Ingresa el número de tu elección: 2

3. **Acceder a la página de phishing:**

Abre tu navegador y ve a http://127.0.0.1:5000 o a la URL pública de ngrok.

**Descargo de responsabilidad**

**Esta herramienta está destinada únicamente con fines educativos. El autor no se hace responsable de ningún mal uso de esta herramienta. Siempre obtén permiso explícito del propietario del sistema antes de realizar pruebas de phishing.**

**Licencia**

Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

**Capturas de Pantalla**

<a href="https://ibb.co/mcNh32n"><img src="https://i.ibb.co/S3fVzMk/Captura-de-pantalla-2024-05-23-111751.png" alt="Captura-de-pantalla-2024-05-23-111751" border="0"></a>

<a href="https://ibb.co/tcwRjPh"><img src="https://i.ibb.co/2P0JVY6/Captura-de-pantalla-2024-05-23-111817.png" alt="Captura-de-pantalla-2024-05-23-111817" border="0"></a>

<a href="https://ibb.co/KjYk72D"><img src="https://i.ibb.co/mCmwt90/Captura-de-pantalla-2024-05-23-111841.png" alt="Captura-de-pantalla-2024-05-23-111841" border="0"></a>

<a href="https://ibb.co/Wy9MBtt"><img src="https://i.ibb.co/yyTZgSS/Captura-de-pantalla-2024-05-23-111900.png" alt="Captura-de-pantalla-2024-05-23-111900" border="0"></a>

<a href="https://ibb.co/Qf7kKMJ"><img src="https://i.ibb.co/c1KwrQy/Captura-de-pantalla-2024-05-23-111937.png" alt="Captura-de-pantalla-2024-05-23-111937" border="0"></a>
