# Putting it into Practice

Using what you have learnt, host the following microservices deployed behind a load balancer.

The microservices are for a smart home-management system. You can send requests to turn lights on/off, requests for changing the temperature of the heating, and even check the status of these in a centralised service.

Create yourself a brand new git repository to store your Terraform code, and write the code to:

- Create a VPC for your new application services
- Create any required security groups
- Create EC2 instances running different applications (For now just keep it to one EC2 instance per application to save on costs)
- Create different target groups for the different services
- Add an [AWS load balancer that uses path-based routing](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html) to route to different target groups

Each of the various applications can be found on the links below:

- https://github.com/northcoders/ce-smart-home-heating
- https://github.com/northcoders/ce-smart-home-lights
- https://github.com/northcoders/ce-smart-home-status
