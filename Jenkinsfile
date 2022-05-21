pipeline {
    agent any
    stages {
        stage('Setup parameters') {
            steps {
                script { 
                    properties([
                        parameters([
                            choice(
                                choices: ['ONE', 'TWO'], 
                                name: 'PARAMETER_01'
                            )            
                        ])
                    ])
                    if(choice.equals("aa")){
                        properties([
                            parameters([
                                choice(
                                    choices: ['N', 'W'], 
                                    name: 'PARAMETER_02'
                            )            
                        ])
                    ])
                    }
                    else{
                        properties([
                            parameters([
                                choice(
                                    choices: ['O', 'T'], 
                                    name: 'PARAMETER_03'
                            )            
                        ])
                    ])
                    }
                }
            }
        }
    }   
}
