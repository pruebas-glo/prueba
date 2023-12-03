# Proyecto Hello World con Kubernetes, GitHub Actions y ArgoCD

.
├── .github
│   └── workflows
│       └── cd.yml
├── Docker
│   └── Dockerfile
│   └── index.html
├── Kubernetes
│   └── deployment.yaml
│   └── service.yaml
├── .gitignore
├── README.md

Este proyecto demuestra cómo desplegar una aplicación "Hello World" en un clúster de Minikube utilizando GitHub Actions para la implementación continua y ArgoCD para la entrega continua.

## Estructura del Proyecto

- `.github/workflows/deploy.yml`: Archivo de flujo de trabajo de GitHub Actions.
- `hello-world-deployment.yaml`: Archivo de manifiesto de Kubernetes para el despliegue inicial.
- `argo-cd-app.yaml`: Archivo de configuración de ArgoCD.
- `Dockerfile`: Archivo Dockerfile para construir la imagen del contenedor.
- `README.md`: Este archivo.

## Instrucciones de Uso

1. Instala Minikube siguiendo las instrucciones en [Minikube](https://minikube.sigs.k8s.io/docs/start/).
2. Inicia el clúster Minikube: `minikube start`.
3. Aplica el despliegue inicial: `kubectl apply -f hello-world-deployment.yaml`.
4. Crea una imagen Docker y súbelo a tu repositorio de Docker Hub.
5. Configura los secretos de Docker en la configuración de tu repositorio en GitHub.
6. El flujo de trabajo de GitHub Actions se activará automáticamente en cada push a la rama principal.

¡Disfruta del desafío y buena suerte!