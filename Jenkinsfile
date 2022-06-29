pipeline{
        agent any
        stages{
            stage('Make Directory'){
                steps{
                    sh "mkdir ~/jenkins-tutorial-test"
                }
            }
            stage('Make Files'){
                steps{
                    sh "touch ~/jenkins-tutorial-test/file1 ~/jenkins-tutorial-test/file2"
                }
            }
            stage{'Build'} {
                steps {
                    sudo apt update
                }
            } 
            stage{'Test'} {
                steps {
                    mkdir example
                }
            }
            stage{`Deploy'} {
                steps {
                    cd example
                    pwd
                }
            }
        }
}
