# charts

 https://poswark.github.io/charts/

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

## add repo helm 
 % helm repo add poswark  https://poswark.github.io/charts/
"poswark" has been added to your repositories

##  buscar repo
% helm search repo hello
NAME            CHART VERSION   APP VERSION     DESCRIPTION                
poswark/hello   0.1.0           1.16.0          A Helm chart for Kubernetes

## Funciona 
 helm install --dry-run hello poswark/hello

 