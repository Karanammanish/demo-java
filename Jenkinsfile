pipeline{
  agent any
  tools{
    maven 'Maven3'
    jre 'Openjdk8'
  }
  stages{
    stage('BUILD'){
      steps{
        sh 'mvn package'
      }  
    }
  }
}
