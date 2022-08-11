pipeline {
    tools {
      nodejs "v16.16.0"
    }
    agent none
    stages {
        stage('Pipeline') {
            parallel {
                stage('Main') {
                    agent any
                    steps {
                        sh "npm i"
//                         sh "npx nx workspace-lint"
//                         sh "npx nx affected --base=HEAD~1 --target=lint --parallel=3"
//                         sh "npx nx affected --base=HEAD~1 --target=test --parallel=3"
//                         sh "npx nx affected --base=HEAD~1 --target=build --parallel=3"
                    }
                }
            }
        }
    }
}
