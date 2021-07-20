pipeline {
  agent any
  tools {
	maven ‘Maven 3.6.3’
}

  stages{
      stage(“Build”){
          steps{
              echo 'step 1'
              sleep 3
          }
      }
      stage(“Test”){
          steps{
              echo 'step 2'
              sleep 9
          }
      }
      stage(“Package”){
          steps{
              echo 'step 3'
              sleep 5
          }
      }
  }

  post{
    always{
        echo 'This pipeline is completed..'
    }
  }
}
