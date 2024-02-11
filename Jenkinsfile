pipeline {
   agent any
   stages {
      stage('clone repo') {
          steps {           
              checkout changelog: false, scm: scmGit(branches: [[name: '*/main']], extensions: [lfs()], userRemoteConfigs: [[url: 'https://github.com/krisansc/jenkins-test.git']])
              echo "pulled the code"
              sh "ls -a"
              sh "pwd"
              sh "cat Jenkinsfile"
          }
      }
   }
}
