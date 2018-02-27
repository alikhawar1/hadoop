pipeline {
   agent {
    dockerfile {
      additionalBuildArgs "--build-args ${start-build-env.sh}"
    }
  tools {
        maven 'maven 3.3.9' 
        jdk 'jdk 9.0.4' 
    }
   
   stages {
      stage('hadoop-build') {
        steps {
           sh './start-build-env.sh'    
        } 
      }
   }
}
