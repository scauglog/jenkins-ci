node {
    stage('Build') {
        echo 'Building....'
        sh 'echo Hello world from develop'
        sh 'pwd > mon-fichier.txt'
        sh 'docker images'
        withCredentials([file(credentialsId: "secret-file", , variable: "MY_SECRET_PATH")]) {
            sh "cat $MY_SECRET_PATH"
        }
    }
}
