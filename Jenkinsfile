pipeline {
   agent any
   stages {
      stage('clone repo') {
          steps {           
              checkout scmGit(branches: [[name: '*/main']], extensions: [[$class: 'WipeWorkspace'], lfs(), cloneOption(noTags: false, reference: '', shallow: false)], userRemoteConfigs: [[url: 'https://github.com/krisansc/jenkins-test.git']])
              echo "pulled the code"
              sh "ls -a"
              sh "pwd"
              sh "cat Jenkinsfile"
          }
      }
   }
}
