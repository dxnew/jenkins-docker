pipeline {
agent any
    tools {
        maven 'Maven-3.6.3'
        jdk 'JDK11'
    }
    node {
      env.JAVA_HOME = tool 'JDK11'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
