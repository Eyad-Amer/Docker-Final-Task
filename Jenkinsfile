pipeline {

  agent any
  
  stages {
      stage('Git Clone') {
            steps {
                git url:"https://github.com/Eyad-Amer/Docker-Final-Task.git", branch:'main'
            }
        }
        
    stage('Build Docker') {
      steps {
        sh 'docker build -t bitcoin_price:$BUILD_NUMBER .'
      }
    }
     stage('Build Tag') {
        steps{
            sh 'docker tag bitcoin_price:$BUILD_NUMBER eyaddocker/bitcoin_price:$BUILD_NUMBER'
        }
         
     }

    stage('Push Docker') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'DokerHub', passwordVariable: 'pass', usernameVariable: 'username')]) {
                    // the code here can access $pass and $user
                    sh 'docker login -u ${username} -p ${pass}'
                    sh 'docker push eyaddocker/bitcoin_price:$BUILD_NUMBER'
                }
            }
        }
    }

    
}
