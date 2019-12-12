pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('build') {
      steps {
        sh 'cp /root/.jenkins/workspace/Promo_master/target/SistPromo.war /opt/wildfly/standalone/deployments'
      }
    }

  }
}