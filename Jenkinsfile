pipeline{
  node any
  tools{
    maven 'Maven3'
    jdk 'Openjdk8'
  }
  stages{
    stage('BUILD'){
      steps{
        sh 'mvn install'
      }  
      post{
        success{
          echo 'Now Archiving it...'
          archiveArtifact artifact: **/target/*.war
        }
      }
    }
  }
}
