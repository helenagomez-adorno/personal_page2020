## Guia para modificar Pagina Personal como colaborador en Github

1- Instalar git y configurar con tu usuario de github 

2- Instalar Hugo 

3- Clonar el repositorio desarrollo y producción.

git clone https://github.com/helenagomez-adorno/personal_page2020.git 

git clone https://github.com/helenagomez-adorno/helenagomez-adorno.github.io.git 


4- Ir a la carpeta de desarrollo

cd personal_page2020/

git submodule add -f -b master https://github.com/helenagomez-adorno/helenagomez-adorno.github.io.git public

5-Agregar contenido

...Hacer algun cambio


6-Para ver los cambios en el servidor local

Construir el sitio con el comando: hugo

Levantar el servidor hugo: hugo server

Ir al navegador: localhost:1313


7-Deployment

hugo

cd public

git add .

git commit -m "Build website"

git push

cd ..
