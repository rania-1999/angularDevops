pipeline {

    agent any

   tools {nodejs '17.3.1'
}

    stages {
         stage ('Checkout GIT'){
                steps {
                    echo 'pulling... ';
                        git branch :'rania',
                        url : 'https://github.com/rania-1999/angular.git';
                }
            }

      stage('Install') {
      steps { sh 'npm install' }
    }
 stage('Test') {
      steps {
         sh 'npm test'
      }
    }    
   stage ('build')
         {
           steps{
                sh ' npm run ng '  }
     }
    }
}