pipeline {
  agent any
  stages {
    stage('Saluta il mondo') {
      parallel {
        stage('Saluta il mondo') {
          steps {
            echo 'Hello, world!'
          }
        }

        stage('Manda e-mail') {
          steps {
            mail(subject: 'Stai attento!', body: 'Sei sicuro di star facendo un buon lavoro?', from: 'marco.leonardo.porro@accenture.com', to: 'markobau.mlp@outlook.it')
          }
        }

      }
    }

    stage('Saluta l\'utente') {
      steps {
        library 'sayHello'
      }
    }

  }
}