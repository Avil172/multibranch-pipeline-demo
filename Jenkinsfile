pipeline {
    agent any
    stages {
        stage('Setup parameters') {
            steps {
                script { 
                    properties([
                        parameters([
                            choice(
                                choices: ['d1-2','s1-5','t1-3','n1-2','p1-3'], 
                                name: 'Select environment'
                            )                            
                        ])
                    ])
                }
            }
        }
    }   
}
