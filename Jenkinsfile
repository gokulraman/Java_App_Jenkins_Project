pipeline{ 
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
                }
            }
        stage("build"){
            steps {
                 echo "----------- build started ----------"
                sh 'mvn clean deploy -Dmaven.test.skip=true'
                 echo "----------- build complted ----------"
            }
        }
       

    }
} 
