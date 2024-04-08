# charts

# Crear hello
helm create hello

#validar el chart
helm lint 

# Revisar los yaml
helm install --dry-run debug .

# Instalar helm 
helm install hello .

# Revisar si se instalo 
helm  list   

## Crear el tgz 
 % helm package hello 
Successfully packaged chart and saved it to: /Users/giovannyorjuelamelo/Documents/Laboratorio/git/charts/hello-0.1.0.tgz

## Crear repo 
 % helm repo index .