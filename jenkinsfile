pipeline {

agent any

tools {
maven 'Maven'
}

stages {

stage('Clone Code') {
steps {
git 'https://github.com/Gurraiah123/jenkins-demo.git'
}
}

stage('Build') {
steps {
sh 'mvn clean package'
}
}

stage('Test') {
steps {
sh 'echo Running tests...'
}
}

stage('Deploy') {
steps {
sh 'cp target/*.war /opt/tomcat/webapps/'
}
}

}

}
