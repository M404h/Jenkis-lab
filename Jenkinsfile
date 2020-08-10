pipeline { 
    agent { docker { image 'bryandollery/terraform-packer-aws-alpine' } }
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('BuildStaging') { 
            steps { 
        
            }
        }
       
        stage('DeployStaging'){
            steps {
                echo 'deploying application on staging environment'
            }
        }
        stage('ValidateStageDeployment') {
            steps {
                echo 'validate deployment on staging'
            }
        }
    }
}
