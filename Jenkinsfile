pipeline {				
    agent any				
    stages {
        stage ("Checkout"){
            steps{
                git 'https://github.com/MoneyTiger/random-python-repo.git'
            }
        }
        stage ("Create File") {		
            steps {
                build 'NameTextFile'	
            }
        }
        stage ("Read File") {
            steps{
                build 'readNameFile'
            }
        }
        stage ("Show Disk Space") {
            steps{
                build 'freeDiskSpaceWindows'
            }
        }    
        stage ("Move File") {
            steps{
                build 'moveNameFile'
            }
        }
        stage ("Build"){
            steps{
                bat 'python anotherFile.py'
            }
        }
    }
}
