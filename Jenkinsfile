pipeline {
    agent any

        stages {
            stage("Build the .Net Application") {
                when {
                    branch 'main'
                }
                steps {
                    bat 'dotnet build'
                }
            }
            stage("Run Unit and Integration Test") {
                when {
                    branch 'main'
                }
                steps {
                    bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
