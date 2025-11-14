pipeline {
    // "agent any" = utilise l'agent Jenkins par défaut (ton conteneur jenkins)
    agent any

    stages {
        stage('Build') {
            steps {
                // 1ère étape : une seule commande
                sh 'echo "Hello World"'

                // 2ème étape : plusieurs commandes dans un bloc multi-ligne
                sh '''
                    echo "Multiline shell steps works too"
                    echo "On est dans le conteneur Jenkins"
                    ls -lah
                '''
            }
        }
    }
}
