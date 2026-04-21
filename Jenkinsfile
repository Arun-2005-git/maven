pipeline {
agent any
tools {
maven 'Maven3'
jdk 'JDK17'
}
 stage('Checkout') {
            steps {
                git branch:'main',
                    url:'https://github.com/Arun-2005/mvn-project.git'
}
stage('Build') {
steps {
sh 'mvn clean compile'
}
}
stage('Test') {
steps {
sh 'mvn test'
}
}
stage('Package') {
steps {
sh 'mvn package'
}
}
}
}
