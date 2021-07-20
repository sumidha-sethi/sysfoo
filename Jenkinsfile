pipeline {
  agent any
  tools {
	maven ‘Maven 3.6.3’
}

  stages{
      stage(“Build”){
          steps{
              echo 'step 1'
              sh 'mvn compile'
          }
      }
      stage(“Test”){
          steps{
              echo 'step 2'
              sh 'mvn clean test'
          }
      }
      stage(“Package”){
          steps{
              echo 'step 3'
              sh 'mvn package -DskipTests '
          }
      }
  }

  post{
    always{
        echo 'This pipeline is completed..'
    }
  }
}
