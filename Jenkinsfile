pipeline 
{
    
  agent any

  stages {
             

    stage("build"){
	when {
		tag "2.0"
             }
        steps{
            echo "building the application"
            }
        } 
		
	stage("test"){
        steps{
             echo "testing the application"
            }
        } 
		
	stage("deploy"){
        steps{
            echo "deploying the application"
            }
        } 
		
	stage("deploy for FIX branch"){
	    when {
		   branch "FIX-*"
		}
        steps{
            echo "deploying this step only when branch is FIX-*"
            }
        } 
		
	stage("deploy for DEA branch"){
		when {
		   branch "DEA-*"
		}
        steps{
            echo "deploying the step only when branch is DEA-*"
            }
        } 
   
    
  }
}