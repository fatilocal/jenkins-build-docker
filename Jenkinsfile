node {
    stage('Clone') {
        git 'https://github.com/fatilocal/jenkins-helloworld-1.git'
    }
    stage('Build') {
        sh '''
       javac Main.java
       '''
    }
    stage('Run') {
        sh '''
        java Main
        '''
    }
}

