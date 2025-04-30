## In this project we create our podes using yml file called nginx-pod.yaml
Task 1

Create a pod using the imperative command and use nginx as the image
Task2

Create the YAML from the nginx pod created in task 1
Update the pod name in the YAML
Use that YAML to create a new pod with the name nginx-new.
Task3

Apply the below YAML and fix the errors, including all the commands that you run during the troubleshooting and the error message
apiVersion: v1
kind: Pod
metadata:
  labels:
    app: test
  name: redis
spec:
  containers:
  - image: rediss
    name: redis
    
