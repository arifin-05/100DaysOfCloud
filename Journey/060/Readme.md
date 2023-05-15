## Introduction


- Well Architected Framework (General Guiding Principles)
- AWS Cloud Best Practices – Design Principles


## Cloud Research


### #1. Well Architected Framework (General Guiding Principles)


- Stop guessing your capacity needs
- Test systems at production scale
- Automate to make architectural experimentation easier
- Allow for evolutionary architectures (design based on changing requirements)
- Drive architectures using data
- Improve through game days, simulate applications for flash sale days


### #2. AWS Cloud Best Practices – Design Principles


- Scalability: vertical & horizontal
- Disposable Resources: servers should be disposable & easily configured
- Automation: Serverless, Infrastructure as a Service, Auto Scaling
- Loose Coupling:
    - Monolith are applications that do more and more over time, become bigger
    - Break it down into smaller, loosely coupled components
    - A change or a failure in one component should not cascade to other components
- Services, not Servers:
    - Don’t use just EC2
    - Use managed services, databases, serverless, etc !
