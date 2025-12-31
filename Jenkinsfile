@Library('jenkins-shared-library') _

def configMap = [
    project: "roboshop",
    component: "shipping"
]

// if branch is not equal to main, then run CI pipeline
if ( ! env.BRANCH_NAME.equalsIgnoreCase('main') ){
    javaEKSPipeline(configMap)
}
else {
    echo "Please proceed with PROD process"
}