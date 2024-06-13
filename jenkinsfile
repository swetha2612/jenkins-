pipeline {
    agent any
    stages {
        stage('List and Count Files') {
            steps {
                sh 'ls -la'
                sh 'ls | wc -l'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Print Current User') {
            steps {
                sh 'whoami'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Create and Navigate Directory') {
            steps {
                sh 'mkdir myfolder'
                sh 'cd myfolder'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Create and Write to File') {
            steps {
                sh 'echo "Hello, Jenkins!" > mytextfile.txt'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Append to File') {
            steps {
                sh 'echo "Appending more content." >> mytextfile.txt'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Display File Content') {
            steps {
                sh 'cat mytextfile.txt'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Find and Replace') {
            steps {
                sh 'sed -i "s/Jenkins/CI-CD/g" mytextfile.txt'
                sh 'cat mytextfile.txt'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Compress and Archive Files') {
            steps {
                sh 'tar -czvf archive.tar.gz myfolder'
                sleep(5) // 5 seconds delay
            }
        }
        stage('Remove Directory') {
            steps {
                sh 'rm -rf myfolder'
                sleep(5) // 5 seconds delay
            }
        }
    }
}
