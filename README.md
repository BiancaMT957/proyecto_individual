# Proyecto 4: "Extractor de documentación de IaC y diagramador básico"
#### Alumna: Bianca Merchán Torres.
#### código: 20220425E
#### correo: bianca.merchan.t@uni.pe
#### Repositorio: https://github.com/Jharvichu/PC4_Grupo8_Proyecto10

### Rol: 

Contribuí al desarrollo de los módulos config_files, root_dir, service_dir y summary_creator. Además, implementé la función generate_diagram_dot() para generar automáticamente un archivo .dot y su correspondiente imagen .png, representando un grafo de dependencias. Finalmente, diseñé e integré un script unificado en Python (generate_docs.py) que combina funcionalidades de otros dos scripts, permitiendo extraer metadatos de módulos Terraform y generar documentación automática en formato Markdown.


### Herramientas necesarias:

```
# terraform
$ sudo apt update
$ sudo apt install terraform
# python +3.8 
$ sudo apt update
$ sudo apt install software-properties-common
$ sudo add-apt-repository ppa:deadsnakes/ppa
$ sudo apt update
$ sudo apt install python3.8 python3.8-venv python3.8-dev
# graphviz
$ sudo apt update
$ sudo apt install graphviz
```

### Instrucciones

Para crear entorno virtual y activarlo.
```
python3 -m venv .venv
```

```
 source venv/bin/activate
 ```


## Ejecución
```
##  Cómo clonar y ejecutar este proyecto

```bash
git clone https://github.com/BiancaMT957/proyecto_individual.git
cd mi_proyecto_individual

# Si hay scripts Python:
python3 -m venv .venv
source .venv/bin/activate

## Para el main.tf
Dentro de la raiz del proyecto
terraform init
terraform apply

# Para el diagram_generator.py
Dentro de scripts
cd scripts
python3 diagram_generator.py

# Ejemplo de ejecución de generate_docs
python3 generate_docs.py



> Los archivos markdown dentro de `docs/` son generados, por lo cual no tienen una autoría definida.
> Se incluyó el script completo diagram_generator.py para que pueda funcionar al ejecutar.
