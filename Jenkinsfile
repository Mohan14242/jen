pipeline {
    agent { node { label 'mohan'}}

    stages{
        stage('unit testting '){
            steps{
                sh 'zip -r ./*'
            }
        }
        stage('intergration testing stage'){
            steps{
                echo "this is the interation between the all stages"
            }
        }
        stage('this is the best way to do the pipeline'){
            steps{
                echo "please enter the way you want"
            }
        }


    }
}