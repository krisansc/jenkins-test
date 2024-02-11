pipeline {
   agent any
   stages {
      stage('clone repo') {
          steps {           
              git clone https://github.com/krisansc/jenkins-test.git
              echo "pulled the code"
          }
      }
   }
}
