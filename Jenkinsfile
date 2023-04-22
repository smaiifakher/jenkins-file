pipeline {
    agent any
    environment {
        KUBECONFIG = credentials('my-kubeconfig')
        DOCKER_REGISTRY = 'docker.io'
        DOCKER_IMAGES = [
            'smaii/pickbazar-laravel:latest',
            'smaii/pickbazar-admin:latest',
            'smaii/pickbazar-shop:latest',
            'mysql:8.0',
            'redis:alpine',
            'mailhog/mailhog:latest'
        ]
        K8S_NAMESPACE = 'my-cluster'
        MANIFESTS_PATH = 'kube'
    }
    stages {
        stage('Pull images from Docker Hub') {
            steps {
                 sh 'make --version'
            }
        }
        stage('Update the Kubernetes manifests') {
            steps {
                 sh 'make --version'
            }
        }
        stage('Apply the Kubernetes manifests') {
            steps {
                 sh 'make --version'
            }
        }
    }
}
