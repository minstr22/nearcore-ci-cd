pipeline {
    agent any
    stages {
        stage('build') {
            steps {
           sh '''
                betatag=$(curl --silent "https://api.github.com/repos/nearprotocol/nearcore/releases" | grep -Po '"tag_name": "${fs}K.*?(?=")' | grep beta | head -1)
                echo $betatag
            '''
            }
             
            }
        }
    }
def fs = '/'


