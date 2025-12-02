package edu.iti;
def build(imageName, imageTag){
    sh "docker build -t ${imageName}:${imageTag} ."

}
def login(userName, password){
    sh "docker login -u ${username} -p ${password}"
}
def push(userName, password){
    sh "docker push ${username}:${password}"
}
