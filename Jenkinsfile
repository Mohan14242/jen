pipeline {
    agent { node { label 'mohan'}}

    stages{
        stage('unit testting '){
            steps{
                sh 'zip -r mohan.zip ./* --exclude=.git --exclude=.js'
            }
        }
        stage('intergration testing stage'){
            steps{
                nexusArtifactUploader{
                    nexusVersion: 'nexus3',
                    protocol: 'http',
                    nexusUrl: '34.229.189.0:8081/repository/catalogue/',
                    groupId: 'com.mohan',
                    version: '402.1.0',
                    repository:'catalogue',
                    credentialsId: 'nexus-auth',
                    Artifacts: [
                        [ArtifactId:'catalogue',
                        classifier: '',
                        file:'mohan.zip',
                        type:'zip']
                    ]
                }
            }
        }
        stage('this is the best way to do the pipeline'){
            steps{
                echo "please enter the way you want"
            }
        }
        stage('this is the chiru'){
            steps{
                echo 'this is the mohan'
            }
        }


    }
}


Your admin user password is located in
/home/nexus/sonatype-work/nexus3/admin.password