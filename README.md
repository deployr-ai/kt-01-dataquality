# Repositorio del DKT 01: Data Quality con PyDeequ y Great Expectations

## Para correr PyDeequ:

Crear un ambiente de python. Por ejemplo:
```
python3.10 -m venv kt-env
```

Activar el ambiente, instalar las librerías necesarias
```python
source kt-env/bin/activate
ipython kernel install --user --name=kt-env
pip install pandas==1.5
pip install sagemaker-pyspark
pip install pydeequ
```
Luego, estamos listos para correr la notebook `demo_pydeequ.ipynb`
## Para correr Great Expectations:
Activar el ambiente, instalar las librerías necesarias
```python
source kt-env/bin/activate
pip install great_expectations
pip install great_expectations_experimental
```
En la ventana de comandos, ir ingresando los siguientes comandos, y ejecutar por completo las jupyter notebooks que se abren automáticamente.
```bash
great_expectations init
great_expectations datasource new
great_expectations suite new
great_expectations suite edit <suite_name>
great_expectations checkpoint new <checkpoint_name>
```
