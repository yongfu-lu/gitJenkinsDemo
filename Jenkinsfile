this.today = new Date()

pipeline{
    agent any
    stages {
        stage("run main python file"){
            steps{
                sh "echo this is \
                    for testing line continuation \
                    there are three lines ${today}"
            }
        }
    }
}
