node {
    stage('Clone') {
        checkout scm  
    }
    stage('Build image') {
        app = docker.build("test/nginx")
    }
    stage('Run image') {
        docker.image('test/nginx').withRun('-p 80:80') { c ->
        sh 'docker ps'
        sh 'curl localhost'
    }
    }
}

