# SIIAU API Client
## _Simple SDK for interacting with SIIAU web service_

> [!IMPORTANT]
> Este no es un proyecto de siiau-dev, sino que es un fork de [dev-cucei-itrans/siiau-api-client](https://github.com/dev-cucei-itrans/siiau-api-client) de lo que parece ser un proyecto relacionado con SIIAU 2 (aka Leo).
> Sólo hice este fork en caso que ellos decidan borrar o ocultar su repositorio.

### Documentación adicional
[Documentación](https://dev-cucei-itrans.gitbook.io/siiau-api-client)

### Instalación
````bash
composer require dev-cucei-itrans/siiau-api-client
````
### Configuración de credenciales
Para hacer uso del paquete se tendrán que configurar las debidas credenciales dentro del archivo .env
````env
SIIAU_WS_URL="https://example.siiau.com"
SIIAU_WS_EMAIL="your@email.com"
SIIAU_WS_PASSWORD="YourSecurePassword"
````

### Uso
````php
$alumno = siiau()->alumno()->encontrar(
    codigo: '1234567890'
);
````

### Cómo utilizar los DTO
El uso del helper retornará un DTO. Con esto podrá acceder a información específica de la respuesta de forma sencilla.
````php
echo($alumno->carrera->id);
````
Realizando esto, podría imprimir lo siguiente.
````bash
INNI
````

## Contribución

Cualquier sugerencia, problema o duda generar un nuevo issue si es que no existe uno que lo describa ya 🙂
