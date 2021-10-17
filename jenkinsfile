pipeline {
    agent any

    stages {
        // node { }

        stage('Build') {
            
            steps {
                sh "echo hello"
            }

            steps {
                ansiblePlaybook(
                    playbook: 'echo.yml',
                    inventory: 'inventory.ini',
                    credentialsId: 'id_macos_rsa',
                    // extras: '-e parameter="some value"')
                )
            }
        }

    }
}
