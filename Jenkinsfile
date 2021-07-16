pipeline {

agent {
    node {
      label 'master'
    }
  }
  
      tools {

        maven 'maven-3.8.1'
    }
    
    stages {
        
     stage('Tool version Check') {
            steps {
                echo "Hello, Maven"
                sh "mvn --version" 
            }
        }
        
   

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
            
        }
        
        stage('Stage 2') {
            steps {
                echo 'Stage2 Hello world!'  
                echo  'Stage2 $date'
               
            }
            
        }
        
        
        stage('Stage 3') {
            steps {
                echo 'Welcome to Stage3 '  
                echo  'Stage3 '
            }
            
        }           
    }

}
