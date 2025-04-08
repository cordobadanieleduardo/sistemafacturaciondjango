mkdir sistemafacdjango
>cd sistemafacdjango
git clone https://github.com/debsconsultores/sis_cmp_fac_py_dj_2.2-.git sistema
cd sistema
git log
py -m venv ..\venv
..\venv\Scripts\activate

pip freeze
py -m pip install --upgrade pip

Django==5.2


pip install Django psycopg[binary] Pillow reportlab django-userforeignkey djangorestframework
pip install dj-database-url gunicorn PyPDF2 pylint xhtml2pdf python-decouple whitenoise
pip install mysqlclient

pip freeze








code .








10. Migrar
python manage.py migrate

11. Crear Super Usuario
python manage.py createsuperuser --username test --email test@mail.com

12. Levantar Servidor
py manage.py runserver 0.0.0.0:8000











Manejo de paquetes con PIP

package-name = Nombre del Paquete a Instalar

Instalar 

pip install package-name

Instalar una versión específica del paquete

pip install package-name==1.0.0

Buscar en PyPI por una paquete en particular :

pip search "query"

Para ver detalles de un paquete instalado:

pip show package-name

Listado de paquetes instalados:

pip list

pip freeze

Listar todos los paquetes desactualizados:

pip list --outdated

Actualizar un paquete desactualizado:

pip install package-name --upgrade

Tenga en cuenta que algunas versiones antiguas de paquetes son removidas automáticamente por PIP cuando se actualizan a una versión nueva del paquete

Para reinstalar completamente el paquete:

pip install package-name --upgrade --force-reinstall

Para deshacerse completamente de un paquete:

pip uninstall package-name