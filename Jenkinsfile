  env.DOCKERHUB_USERNAME = 'ajaykm'
  def containeridt
  node("docker-test") {
    checkout scm

    stage("Unit Test") {
      sh "docker container run --rm -i -v /home/jenkins_data/jenkins/workspace/dockercoreapp:/app -w /app microsoft/dotnet dotnet restore"
    }
