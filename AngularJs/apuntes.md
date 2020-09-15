
# CORS EN ANGULAR TOKEN JWT SPRING CONTROLLER
# En la raiz del proyecto crear un archivo "proxy.conf.json" y agregar lo siguiente
{
  "/tmpproveedores/*": {
    "tarjet": "http://localhost:9000",
    "secure": false,
    "loglevel": "debug"
  }
}
# agregar en el package.json
"start": "ng serve --proxy-config proxy.conf.json",
# quitar url tarjet dato de los services -> opcional
