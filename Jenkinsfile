pipeline{
    agent any
    tools {
  maven 'M2_HOME'
}
        stages{
            stage("Git SCM"){
                steps {
                git 'https://github.com/henrykrop2022/myapp-ansible.git'
                }
            }
            stage('Maven Build'){
                steps{
                    sh 'mvn clean package'
                }
            }
        }
    }