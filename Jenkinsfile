pipeline {
agent any
stages {
stage ('Compile Stage') {
steps {
withMaven(maven : 'Maven 3.8') {
bat'mvn clean compile'
}
}
}
stage ('Testing Stage') {
steps {
withMaven(maven : 'Maven 3.8') {
bat'mvn test'
}
}
}
stage ('Install Stage') {
steps {
withMaven(maven : 'Maven 3.8') {
bat'mvn install'
}
}
}
}
}
