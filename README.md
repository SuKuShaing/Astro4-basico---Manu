# Proyecto de Manu para aprender Astro

Siguiendo el tutorial de Manu Martin
https://youtu.be/FafJOvhnGos?si=wSb3sChrIdgiHlWM




## EPERM: operation not permitted, rmdir
Con esto se solucionan el error
```
$ npm run build

> generador-de-sitios-estaticos---fazt@0.0.1 build
> astro build
EPERM: operation not permitted, rmdir 'D:\Progra\Youtube\Astro\Generador de sitios estaticos - Fazt\node_modules\.vite\deps'
  Stack trace:

```

ejecutando los pasos de aquí, se soluciona (ojo comandos para consola windows, no funcionana en bash porque emula comandos linux)

👇️ clean npm cache
npm cache clean --force

👇️ (Windows) delete node_modules and package-lock.json
rd /s /q "node_modules"
del package-lock.json
del -f yarn.lock

👇️ update your npm version
npm install -g npm@latest --force

👇️ clean npm cache
npm cache clean --force

👇️ install packages
npm install