# $ heroku create intro

_Code goes in, apps come out. I can explain that._

## Part 1: Philosophy
12Factor: http://12factor.net  
- Codebase/apps/deploys  
- Dependencies  
- Store config in the environment  
- Backing Services  
- Processes  
	
## Part 2: PaaS
### The wat

**What is PaaS:**  
"Platform as a service (PaaS) is a category of cloud computing services that 
provide a computing platform and a solution stack as a service [...] The consumer
 controls software deployment and configuration settings. The provider 
 provides the networks, servers, storage and other services."
- https://en.wikipedia.org/wiki/Platform\_as\_a\_service

SaaS is like GMail, Basecamp. IaaS is AWS, with EC2, Load Balancers, S3, etc. 
PaaS is a set of those solutions (IaaS) combined and packaged. 

- Heroku allows you to push your code, configure backing services, and dynamically
adjust the amount of resources your application can consume. 
- Spend time solving app problems, not infrastructure 
- _Tyler's full stack comment_

### Features 

**Check it:**

- Elasticity & scale: scale horizontally
- Intelligent routing: load balancing across a fleet of dynos
- Process management: acting a fool? we'll replace you
- Distribution and redundancy: hardware be damned – here one day, there the next
- Isolation: subvirtualized containers with benefits

### Terms:
- Git: version control 
- Slugs: compiled*, compressed and portable versions of the app
- Configuration and Config Vars: everything that is likely to vary between deploys
- Dynos: a unit of work, light weight, multipurpose container 
- Buildpacks: packaged scripts to compile the slug
- Processes: one or more stateless executions


## Part 3: Using
- rails new
- heroku create
- push code
- scale
- one-offs
- swap add-ons (Dev -> Basic)