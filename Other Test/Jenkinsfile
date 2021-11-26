pipeline{
    agent any

    stages{
        
        stage('Test'){

            steps{
                 bat 'echo This is for post'
            }
        }
    }

    post{

        always{
            bat 'echo I will always execute'
        }
        success{
            bat 'echo I will only execute when job is success '
        }
        failure{
            bat 'echo I will only execute when the job is failed'
        }
        unstable{
            bat 'echo I will only execute when the job is unstable'
        }
    }
}
