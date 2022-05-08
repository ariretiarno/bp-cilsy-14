helm  upgrade jenkins jenkins/jenkins -n jenkins -f jenkins-values.yaml --install      ──(Sun,May08)─┘
Release "jenkins" does not exist. Installing it now.
NAME: jenkins
LAST DEPLOYED: Sun May  8 14:44:02 2022
NAMESPACE: jenkins
STATUS: deployed
REVISION: 1
NOTES:
1. Get your 'admin' user password by running:
  kubectl exec --namespace jenkins -it svc/jenkins -c jenkins -- /bin/cat /run/secrets/chart-admin-password && echo

2. Visit http://jenkins.kube.retiarno.my.id

3. Login with the password from step 1 and the username: admin
4. Configure security realm and authorization strategy
5. Use Jenkins Configuration as Code by specifying configScripts in your values.yaml file, see documentation: http://jenkins.kube.retiarno.my.id/configuration-as-code and examples: https://github.com/jenkinsci/configuration-as-code-plugin/tree/master/demos

For more information on running Jenkins on Kubernetes, visit:
https://cloud.google.com/solutions/jenkins-on-container-engine

For more information about Jenkins Configuration as Code, visit:
https://jenkins.io/projects/jcasc/


NOTE: Consider using a custom image with pre-installed plugins