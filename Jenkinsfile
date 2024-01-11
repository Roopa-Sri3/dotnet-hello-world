pipeline{
  agent any
    stages{
   stage("Build"){
    steps{
       script{
        sh """
        dotnet restore
        """
      }
    
  }
  }
    stage("run"){
      steps{
      
        script{
          sh 'dotnet run --project hello-world-api'
        }
        
      }
    }
  }
}
    
