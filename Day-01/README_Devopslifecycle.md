# DevOps Lifecycle - Application Focused
We are going to take a look at the high-level view of the application from start to finish and then back around again like a constant loop.

## Development
Let's take a brand new example of an Application, to start with we have nothing created, maybe as a developer, you have to discuss with your client or end user the requirements and come up with some sort of plan or requirements for your Application. We then need to create from the requirements our brand new application.

In regards to tooling at this stage, there is no real requirement here other than choosing your IDE and the programming language you wish to use to write your application.

As a DevOps engineer, remember you are probably not the one creating this plan or coding the application for the end user, this will be a skilled developer.

But it also would not hurt for you to be able to read some of the code so that you can make the best infrastructure decisions moving forward for your application.

We previously mentioned that this application can be written in any language. Importantly this should be maintained using a version control system, this is something we will cover also in detail later on and in particular, we will dive into Git.

It is also likely that it will not be one developer working on this project although this could be the case even so best practices would require a code repository to store and collaborate on the code, this could be private or public and could be hosted or privately deployed generally speaking you would hear the likes of GitHub or GitLab being used as a code repository. Again we will cover these as part of our section on Git later on.

## Testing
At this stage, we have our requirements and we have our application being developed. But we need to make sure we are testing our code in all the different environments that we have available to us or specifically maybe to the programming language chosen.

This phase enables QA to test for bugs, more frequently we see containers being used for simulating the test environment which overall can improve on cost overheads of physical or cloud infrastructure.

This phase is also likely going to be automated as part of the next area which is Continuous Integration.

The ability to automate this testing vs 10s,100s or even 1000s of QA engineers having to do this manually speaks for itself, these engineers can focus on something else within the stack to ensure you are moving faster and developing more functionality vs testing bugs and software which tends to be the hold up on most traditional software releases that use a waterfall methodology.

## Integration
Quite importantly Integration is at the middle of the DevOps lifecycle. It is the practice in which developers require to commit changes to the source code more frequently. This could be on a daily or weekly basis.

With every commit, your application can go through the automated testing phases and this allows for early detection of issues or bugs before the next phase.

## Deployment
Ok so we have our application built and tested against the requirements of our end user and we now need to go ahead and deploy this application into production for our end users to consume.

This is the stage where the code is deployed to the production servers, now this is where things get extremely interesting and it is where the rest of our 86 days dives deeper into these areas. Because different applications require different possibly hardware or configurations. This is where Application Configuration Management and Infrastructure as Code could play a key part in your DevOps lifecycle. It might be that your application is Containerised but also available to run on a virtual machine. This then also leads us onto platforms like Kubernetes which would be orchestrating those containers and making sure you have the desired state available to your end users.

## Monitoring
Things are moving fast here and we have our Application that we are continuously updating with new features and functionality and we have our testing making sure no gremlins are being found. We have the application running in our environment that can be continually keeping the required configuration and performance.

But now we need to be sure that our end users are getting the experience they require. Here we need to make sure that our Application Performance is continuously being monitored, this phase is going to allow your developers to make better decisions about enhancements to the application in future releases to better serve the end users.

This section is also where we are going to capture that feedback wheel about the features that have been implemented and how the end users would like to make these better for them.

**Reliability** is a key factor here as well, at the end of the day we want our Application to be available all the time it is required. This then leads to other observability, security and data management areas that should be continuously monitored and feedback can always be used to better enhance, update and release the application continuously.

You can find more about this in [Continuous Cycle of Devops](./README_DetailedCycle.md)

