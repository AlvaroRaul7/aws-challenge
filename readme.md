## Requerimientos para el desafío

- Git (https://git-scm.com/downloads)
- Instalar AWS-CLI https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html
- Zip 
- Visual Studio Code (Opcional)

Claves de acceso para configurar AWS CLI


```
ID de clave de acceso
AKIASFSTGGZK37LGLRRP

Clave de acceso secreta
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

Region
us-east-1
```



 
### Probar el challenge de forma local (Opcional)
- [ ] Instalar Poetry
  https://python-poetry.org/docs/basic-usage/
  - [ ] Instalar dependencias con `poetry install`
  - [ ] Activar el entorno virtual con `poetry shell`
  - [ ] Correr el proyecto con `poetry run python amazon_rekognition.py`


### Desafío

- Editar el archivo `amazon_rekognition.py` con la url de la imagen que se encuentra en la variable `test_challenge_url`
- Subir el modulo  `amazon_rekognition.py` a AWS Lambda con el nombre `aws-<nombre>-<apellido>`
  * El handler para la función Lambda es `amazon_rekognition.lambda_handler`
  * El rol para crear la función Lambda es `arn:aws:iam::149424584277:role/AwsEcuadorSupport`
  * El runtime de la funcion Lambda es `Python 3.8`

- Invocar a la funcion Lambda desde la terminal de comandos 
- Imprimir el response en la terminal de comandos

Se deberia esperar el siguiente response segun la imagen:

```

{"statusCode": 200, "headers": {"Content-Type": "application/json"}, "body": "{\"Number of labels found\": 15, \"Labels for the image \": [\"Outer Space\", \"Astronomy\", \"Person\", \"Baby\", \"Wheel\", \"Machine\", \"Bicycle\", \"Vehicle\", \"Transportation\", \"Planet\", \"Head\", \"Globe\", \"Outdoors\", \"Night\", \"Nature\"]}"}

```

### Referencias

- https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html
- https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-awscli.html
  
  



 
  
