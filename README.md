Spin up some ubuntu-based virtual machines either locally or in public cloud (AWS, Azure, GCP...)
- one of the instances is going to be controller (leader)
- at least one runner agent (follower node). Preferably two

Find ways to test (make it accessible via HTTP and SSH) what happens on your instances (e.g. surf through jenkins workspace or run the project)

### Tips
Feel free to connect to follower(s) via password-based SSH auth instead of key

To begin with build the project from [here](https://github.com/spring-projects/spring-petclinic) using:
- Freestyle job
- Pipeline ([declarative](https://github.com/4crt/learn-jenkins/blob/main/jenkins/pipeline.jenkins))
