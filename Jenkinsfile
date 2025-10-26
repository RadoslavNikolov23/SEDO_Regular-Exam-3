pipeline {
    agent any

        stages {
            stage("Build the .Net Application") {
                steps {
                    bat 'dotnet build'
                }
            }
            stage("Run Unit and Integration Test") {
                steps {
                    bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}
