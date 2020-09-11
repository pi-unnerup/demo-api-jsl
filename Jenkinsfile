jsl = library(
  identifier: 'jenkins-shared-library@docker-build',
  retriever: modernSCM(
    [
      $class: 'GitSCMSource',
      remote: 'https://github.com/controlplaneio/jenkins-shared-library.git'
    ]
  )
)

buildImage([jsl: jsl])
  .build(
    registry: 'controlplane',
    image_name: 'demo-api'
  )
  // .unitTest(
  //   command: 'My unit test command'
  // )
  // .deploy(
  //   command: 'My deploy command'
  // )
