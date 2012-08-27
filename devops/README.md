# curious-learners

## DevOps track

This track teaches how to reduce your team's pain and your customer's
unhappiness caused by the risks and costs of manual application operation
and deployment processes.

The objective is to give you hands-on experience with reliable automation
tools in real-world scenarios.

### Suggested topics:

### 1.   Cloud basics with *Amazon EC2*

To have an easy and safe practise environment, we'll start by learning how
to get instant virtual machines out of the Amazon EC2 service.

We'll be using several virtual machines to simulate a realistic client
infrastructure. 

### 2.   Automating system configuration with *Puppet*

Which packages should be installed on a server, what services should be running,
which configuration files should be customized, cron jobs running, user accounts
and SSH keys set up - all this is usually partially described in MS Word format
deployment documentation. 

Changes to configuration need to be both formally and informally communicated
to operations staff, checked, and possibly requested again.

We'll learn how to formally describe system configurations and admin processes
with the Puppet specification language, and put those configurations into action.

### 3. Continous integration and binary artifact management with *Git*, *Jenkins CI* and *Sonatype Nexus*

We'll set up a Continuous Integration tool, configure automatic builds for our
example Java web application Git repository, and set up automatic binary build
(Maven) artefact deploys into Sonatype Nexus.

We'll configure Nexus to serve our JARs and WARs to both our developers, and
to our application deployment infrastructure.

### 4. Lab #1: Set up 10 AWS EC2 micro instances, Puppet conf, add *Java* web apps

Now that we have our example Java application being automatically built 
by Jenkins and deployed to Nexus, we'll boot up some virtual machines 
from Amazon EC2, set up a Java application server cluster with Puppet, 
and set up our Puppet configuration to automatically deploy the desired 
version of the web application to the desired application servers.

### 5. Managing database schema changes with *Liquibase* and *MCollective*

Beyond code changes, we developers sometimes want to modify the application's
database schema. We'll learn how to use Liquibase to keep track of those changes,
audit them, and reliably deploy them to a production application server cluster
with Puppet and MCollective.

### 6. OS, JVM and application monitoring with *RHQ* and *logstash*

Visibility into server and application status means being able to react to
problems before they become catastrophes. We'll use Red Hat RHQ to set up
monitoring on hardware, disk space, operating system, and JVM level, as
well as some application alerts.

While log files are traditionally monitored by tailing them through SSH,
and setting up keyword alerts in server monitoring systems, going through
history, searching for potentially problematic situations, and applying
special analysis on things like stack traces is awkward at best without
tools like logstash.

### 7. Managing your dev environment with *Vagrant* and Puppet

We'll emulate the production environment on our own development machines
with Vagrant, and use Puppet to recreate our production environment locally.
