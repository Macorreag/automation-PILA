# Automation-PILA

Almacenamiento de test automatizados generados con deferentes extensiones de chrome especialmente Selenium IDE para automatizar tareas en la plataforma de [Aportes en Linea Colombia](https://www.aportesenlinea.com/)

## Documentación de test automatizados mediante Selenium

### Variables

Para facilitar el acceso a cada uno de los Scripts se usan variables que están incluidas dentro de los Scrits aquí se desglosa la función de cada una de ellas:

- Cedula : Numero de identificación de la persona
- mesIngreso
- diaIngreso
- tipoNovedad: Tipo de novedad para ingresar [INGRESO , RETIRO DE LA EMPRESA]

### Funciones Completas

Los test automatizados que ya se han probado y son capaces de responder en la plataforma se encuentran en la Suite llamada _Complete_.

[x] Login
[x] Crear Novedades [Ingreso y Retiro]
[x] Access Unitary [Permite la creación de variables para la ejecución de los demas scripts]

### Funciones incompletas

Los test que aún se están probando estan en la carpeta principal y no están añadidos a ningunaSuite.
[ ] Modificación de planillas
[ ] Crear un usuario [ Se debe programar para que revise si el usuario existe o no ]

### Test Automatizados con la [extensión Selenium IDE](https://www.selenium.dev/selenium-ide/) - Para probar los mismos se uso el extensión de Google Chrome.

**Pasos**

    1. Adicionar Novedad Retiro (Mes,Dia)
    2. Colocarlo como Independiente
    3. Generar las planillas para los meses completos
    4. Colocarlo como Independiente 30 dias.
    5. Generar las planillas para los meses incompletos que incluyen aportes ARL.
