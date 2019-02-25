---
layout: article
language: 'es-es'
version: '4.0'
category: 'installation'
---
# Instalación

* * *

## Windows

To use Phalcon on Windows, you will need to install the phalcon.dll. We have compiled several DLLs depending on the target platform. Los archivos dll pueden encontrarse en nuestra página de [descarga](https://phalconphp.com/en/download/windows).

Identify your PHP installation as well as architecture. If you download the wrong DLL, Phalcon will not work. `phpinfo()` contains this information. In the example below, we will need the NTS version of the DLL:

![phpinfo](/assets/images/content/phpinfo-api.png)

The available DLLs are:

| Arquitectura | Version | Tipo                  |
|:------------:|:-------:| --------------------- |
|     x64      |   7.x   | Thread safe           |
|     x64      |   7.x   | Non Thread safe (NTS) |
|     x86      |   7.x   | Thread safe           |
|     x86      |   7.x   | Non Thread safe (NTS) |

Editar el archivo php.ini y luego añadir al final:

```ini
extension=php_phalcon.dll
```

Reiniciar tu navegador web.