pipeline{
    agent any
    stages {
        stage("run main python file"){
            steps{
                sh('python3 main.py')
            }
        }

        stage("create aws cloudFormation stack"){
            steps{
                sh('aws cloudformation create-stack --stack-name exampleStack2 --template-body file://cfn.json --parameters ParameterKey=KeyExample,ParameterValue=KeyExample')
            }
        }
    }
}

aws cloudformation create-stack --stack-name exampleStack --template-body file://cfn.json --parameters ParameterKey=KeyExample,ParameterValue=KeyExample