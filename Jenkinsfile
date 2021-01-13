pipeline {
     agent any
         stages{
            stage('click credit_card') {
                    steps{
                              echo "credit card page opened!!";
                        }
         }

             stage('user name') {
                    steps{
                               echo "user name successfully entered!";
                         }
                 }

            stage('password') {
                    steps{
                                echo "password entered successfully!!";
                             /*sh exit ("1");*/
                        }
                }

                stage('Deploy')    {
                    steps{
                                 echo "pass!";
                        }
                }

        }
        post {
            always {
                      echo 'this will always run'
                }
                success {
                      echo 'this will run only if successful'
                }
                failure {
                      echo 'this will run only if failed'
                }
                unstable {
                     echo 'this will run only if the run was marked as unstable'
		}
		changed {
		       echo 'this will run only if the state of the pipeline has changed'
			   echo ' for example, if the pipeline was previously failing but is now successfully'
		}
	}
}	
