pipeline {
  agent any
  stages {
    stage('Saluta il mondo') {
      steps {
        echo 'Hello, world!'
      }
    }

    stage('Saluta l\'utente') {
      steps {
        library 'sayHello'
      }
    }

    stage('Manda e-mail') {
      steps {
        emailext(subject: 'Stai attento!', body: 'Sei sicuro di star facendo un buon lavoro?', attachLog: true, from: 'markobau.mlp@outlook.it', to: 'marcoleonardo.porro@gmail.com')
      }
    }

  }
}