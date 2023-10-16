# Universidad Nacional 
## Escuela de Informática 
### Sistemas Distribuidos.

#### Proyecto II - Frontend.

Estudiante: 
David Rojas Chavarría
Cédula
114310962
Profesor:
Armando Arce Orozco.

Ciclo II 2023

Repositorio \
	https://github.com/DavidRojasChavarriaUNA/Proyecto-II-Frontend-SistemasDistribuidos2023 \

Para ejecutar el proyecto deberá ejecutar los siguientes pasos:

1. Para ejecutar el proyecto deberá ingresar a la consola o terminal y ubicarse en la carpeta del frontend \
	ejemplo (en windows)\
		 'cd "C:\Users\drojas\Desktop\Licenciatura UNA\Ciclo II 2023\Sistemas Distribuidos\Sesión 10\Proyecto-II-SistemasDistribuidos2023\Frontend"'

2. instalar los paquetes de node.js en caso que no los haya instalado. \
	"npm install"
	
3. ingresar al archivo .env y dejar la variable de entorno con la url del server backend \
	Importante agregar a la url /.netlify/functions ya que esta es la posición de las FAAS \ 
	VITE_BASE_URL=UrlDelServidorDeNetlify/.netlify/functions \
	ejemplo \
	VITE_BASE_URL=https://proy-ii-faas-drch-sist-dist-una-2023.netlify.app/.netlify/functions \

4. para ejecutar el frontend en local, puede hacerlo mediante el comando
	"npm run dev" \
	una vez inicializado, el sitio se levanta en la url local "http://localhost:3000", en el puerto 3000 \

5. Publicar el frontend en Netlify, y configurar el paso 3 con la URL que va a utilizar con el frontend
   - Runtime: Not set
   - Base directory: Frontend
   - Package directory: Frontend/
   - Build command: npm run build
   - Publish directory: Frontend/dist
   - Functions directory: Frontend/
   - Deploy log visibility: Logs are public
   - Build status: Active

URL del Frontend \
	https://proy-ii-front-drch-sist-dist-una-2023.netlify.app/