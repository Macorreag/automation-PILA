# Automation-PILA

Almacenamiento de test automatizados generados con deferentes extensiones de Chrome y Firefox, especialmente Selenium IDE para automatizar tareas en la plataforma de [Aportes en Linea Colombia](https://www.aportesenlinea.com/)

## Documentación de test automatizados mediante Selenium

### Variables

Para facilitar el acceso a cada uno de los Scripts se usan variables que están incluidas dentro de los Scrits aquí se desglosa la función de cada una de ellas:

- Cedula : Numero de identificación de la persona
- mesIngreso
- diaIngreso
- tipoNovedad: Tipo de novedad para ingresar [INGRESO , RETIRO DE LA EMPRESA]

### Funciones Completas

Los test automatizados que ya se han probado y son capaces de responder en la plataforma se encuentran en la Suite llamada _Complete_.

- [x] Login
- [x] Crear Novedades [Ingreso y Retiro]
- [x] Access Unitary [Permite la creación de variables para la ejecución de los demas scripts]

### Funciones incompletas

Los test que aún se están probando estan en la carpeta principal y no están añadidos a ningunaSuite.

- [ ] Modificación de planillas
- [ ] Crear un usuario [ Se debe programar para que revise si el usuario existe o no ]

### Problemas

Se conoce por selenium IDE que [eventos de tipo `:hover` - _mouse over_ no funcionan](https://github.com/SeleniumHQ/selenium-ide/issues/362) correctamente. Por esta razon algunos de los scripts pueden no funcionar correctamente al ejecutar esta acción.Sin embargo gran cantidad de los test automatizados intentan acceder de otra manera para que no sea necesario desencadenar este evento.

### Test Automatizados con la [extensión Selenium IDE](https://www.selenium.dev/selenium-ide/) - Para probar los mismos se uso el extensión de Google Chrome.

**Pasos**

    1. Adicionar Novedad Retiro (Mes,Dia)
    2. Colocarlo como Independiente
    3. Generar las planillas para los meses completos
    4. Colocarlo como Independiente 30 dias.
    5. Generar las planillas para los meses incompletos que incluyen aportes ARL.
