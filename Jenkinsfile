properties([parameters([[$class: 'WHideParameterDefinition', defaultValue: 'yoyo', name: 'hidden_var']])]) 
  pipeline {
        agent any

stages{
        stage("make param global") {
             steps {
                 script{
               tmp_param =  "Hello"
               env.custom_var = tmp_param
                 }
              }
        }
        stage("test if param was saved") {
            steps {
              echo"About to check result"
              echo "${env.custom_var}"
            }
        }
    }
  }
