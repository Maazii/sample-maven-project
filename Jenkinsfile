pipeline
{
  agent any

  stages
  {
    stage("Initialize Git")
    {
      git init
    }
    stage("Maven Install")
    {
      steps
      {
        withMaven(maven: "maven3")
        {
          sh "mvn clean install"
        }
      }
    }
  }
}
