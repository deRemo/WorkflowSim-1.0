## NOTE: WorkflowSim IS NO LONGER MAINTAINED.

---

Table of Contents
-----------------

1. Directory structure of the WorkflowSim Toolkit
2. Software requirements: Java version 1.6 or newer 
3. Installation and running the WorkflowSim Toolkit


1. Directory structure of the WorkflowSim Toolkit
----------------------------------------------

workflowsim/			-- top level WorkflowSim directory
	docs/			-- WorkflowSim API Documentation
	examples/		-- WorkflowSim examples
	lib/			-- WorkflowSim jar archives
	sources/		-- WorkflowSim source code


2. Software requirements: Java version 1.6 or newer
---------------------------------------------------

WorkflowSim has been tested and ran on Sun's Java version 1.8.0 or newer.
If you have non-Sun Java version, such as gcj or J++, they may not be compatible.
You can use Eclipse, NetBeans, or Ant to compile and run WorkflowSim

3. Installation and running the WorkflowSim Toolkit
### Welcome to WorkflowSim Pages.
WorkflowSim is a workflow simulator to support large-scale scheduling, clustering and provisioning studies. It is developed by Weiwei Chen, a Phd student from University of Southern California under the Apache License version 2.0. WorkflowSim is not yet fully completed and we welcome your contribution to this project. 

This page introduces the basic features of WorkflowSim and how to install and run it with Eclipse or NetBeans.

### 1. Use WorkflowSim with GitHub/Eclipse

( It is suggested to use WorkflowSim if you are going to contribute back to this project, otherwise it is not required. )


1.1 Register a GitHub account and fork your own branch

Go to the repository page (https://github.com/WorkflowSim/WorkflowSim-1.0) and click 'Fork' on the top-right corner next to 'Star'. Then you will have your own branch of WorkflowSim and you can maintain your codes under this branch and commit your changes to it. In this example, we use 'chenww05' as an example and you will see a new repo called chenww05/WorkflowSim-1.0. Go to your repo, and copy the path. In this case, it is "https://github.com/chenww05/WorkflowSim-1.0.git". 

1.2 Install EGit


Open your Eclipse, go to 'Help'->'Install New Software', in 'Work with', choose '--All Available Sites', make sure you have EGit listed, otherwise click the item and install it. 

1.3 Check out your source codes

First, create a new java project called 'WorkflowSim' (it doesn't have to be 'WorkflowSim'). Right click your project, choose 'Import'. Click 'Git'->'Projects from Git'. Set the URL to be "https://github.com/chenww05/WorkflowSim-1.0.git". And then you will see a branch called 'master', tick it and continue. And you don't need import projects again so just cancel. 

1.4 Import Source Files and Libraries

Right click the project again and choose 'Properties'. Go to 'Java Build Path'. Link two source directories (your_repo_root/examples, your_repo_root/sources)to the source folders. Add two external JARs (your_repo_root/lib/flanagan.jar and your_repo_root/lib/jdom-2.0.0.jar) to the Libraries.  

1.5 Run an Example

Run an example i.e., org.workflowsim.examples.WorkflowSimBasicExample1.java. Open WorkflowSimBasicExample1.java, replace the 

String daxPath = "/Users/chenweiwei/Work/WorkflowSim-1.0/config/dax/Montage_100.xml";

with your real physical file path. Right click on WorkflowSimBasicExample1.java and choose 'Run File'. You should be able to see some output:

98        SUCCESS        2            0            6.91        263.78            270.69            8
99        SUCCESS        2            0            0.83        270.69            271.52            9

### 2. Use WorkflowSim with GitHub/NetBeans

2.1 Register a GitHub account and fork your own branch

It is the same to 1.1.

2.2 Install Git

Go to 'Teams'->'Available Plugins'. Search for 'Git' and install it. 

2.3 Check out your source codes

First, create a new java project with Existing Sources called 'WorkflowSim' (it doesn't have to be 'WorkflowSim'). Right click this project and choose 'Set as Main Project' for convenience. 
Right click this project again and choose 'Versioning'->'Initialize Git Repository'. You don't need to change the root path, just click 'OK'. 

Right click the project and choose 'Git'->'Remote'->'Pull', set the 'Repository URL' to be 'https://github.com/chenww05/WorkflowSim-1.0.git' and the 'Remote name' to be 'master'. Click 'OK' and you will see a branch called 'master', tick it and continue. 

2.4 Import Source Files and Libraries

After a while the download is down, right click the project again and choose 'Project Properties'. Go to 'Sources', click 'Add Folder' and choose two folders (your_repo_root/examples and your_repo_root/sources). Go to 'Libraries', add all jars  (your_repo_root/lib/*.jar). 

2.5 Run an Example

The same to 1.5. 

### 3. Use WorkflowSim with Eclipse but without GitHub
( If you don't want to contribute back to WorkflowSim with your codes, you can use WorkflowSim without GitHub. )

3.1 Download Source Files. 

Skip 1.1 and 1.2. Different to 1.3, we download source files directly from https://github.com/WorkflowSim/WorkflowSim-1.0/archive/master.zip and unzip it to your_repo_root. 

3.2 Switch to 1.4 and continue with the rest steps (1.5). 

### 4. Use WorkflowSim with NetBeans but without GitHub

4.1 Download Source Files

The same to 3.1. 

4.2 Switch to 2.4 and continue with the rest steps (2.5).

### Authors and Contributors
This page is written by Weiwei Chen @chenww05. For details or bug reports, please contact the author. 

### Support or Contact
Please send an email to support@workflowsim.org. We appreciate your contribution to this project and please go to github to submit your bug report.  
Many of the questions may have been answered in our wiki pages: https://github.com/WorkflowSim/WorkflowSim-1.0/wiki/_pages
### Mailing Lists

WorkflowSim Announce
Message about new release or updates
workflowsim-announce@googlegroups.com

WorkflowSim Users
Messages about WorkflowSim related questions/reports
workflowsim-user@googlegroups.com

WorkflowSim Developers
Messages about WorkflowSim development
workflowsim-dev@googlegroups.com

---

---

# CloudSim: A Framework For Modeling And Simulation Of Cloud Computing Infrastructures And Services #

Cloud computing is the leading approach for delivering reliable, secure, fault-tolerant, sustainable, and scalable computational services. Hence timely, repeatable, and controllable methodologies for performance evaluation of new cloud applications and policies before their actual development are reqruied. Because utilization of real testbeds limits the experiments to the scale of the testbed and makes the reproduction of results an extremely difficult undertaking, simulation may be used.

CloudSim goal is to provide a generalized and extensible simulation framework that enables modeling, simulation, and experimentation of emerging Cloud computing infrastructures and application services, allowing its users to focus on specific system design issues that they want to investigate, without getting concerned about the low level details related to Cloud-based infrastructures and services.

CloudSim is developed in [the Cloud Computing and Distributed Systems (CLOUDS) Laboratory](http://cloudbus.org/), at [the Computer Science and Software Engineering Department](http://www.csse.unimelb.edu.au/) of [the University of Melbourne](http://www.unimelb.edu.au/).

More information can be found on the [CloudSim's web site](http://cloudbus.org/cloudsim/).


# Main features #

  * support for modeling and simulation of large scale Cloud computing data centers
  * support for modeling and simulation of virtualized server hosts, with customizable policies for provisioning host resources to virtual machines
  * support for modeling and simulation of application containers
  * support for modeling and simulation of energy-aware computational resources
  * support for modeling and simulation of data center network topologies and message-passing applications
  * support for modeling and simulation of federated clouds
  * support for dynamic insertion of simulation elements, stop and resume of simulation
  * support for user-defined policies for allocation of hosts to virtual machines and policies for allocation of host resources to virtual machines


# Download #

The downloaded package contains all the source code, examples, jars, and API html files.

# Publications #

  * Anton Beloglazov, and Rajkumar Buyya, [Optimal Online Deterministic Algorithms and Adaptive Heuristics for Energy and Performance Efficient Dynamic Consolidation of Virtual Machines in Cloud Data Centers](http://beloglazov.info/papers/2012-optimal-algorithms-ccpe.pdf), Concurrency and Computation: Practice and Experience, Volume 24, Number 13, Pages: 1397-1420, John Wiley & Sons, Ltd, New York, USA, 2012.
  * Saurabh Kumar Garg and Rajkumar Buyya, [NetworkCloudSim: Modelling Parallel Applications in Cloud Simulations](http://www.cloudbus.org/papers/NetworkCloudSim2011.pdf), Proceedings of the 4th IEEE/ACM International Conference on Utility and Cloud Computing (UCC 2011, IEEE CS Press, USA), Melbourne, Australia, December 5-7, 2011.
  * **Rodrigo N. Calheiros, Rajiv Ranjan, Anton Beloglazov, Cesar A. F. De Rose, and Rajkumar Buyya, [CloudSim: A Toolkit for Modeling and Simulation of Cloud Computing Environments and Evaluation of Resource Provisioning Algorithms](http://www.buyya.com/papers/CloudSim2010.pdf), Software: Practice and Experience (SPE), Volume 41, Number 1, Pages: 23-50, ISSN: 0038-0644, Wiley Press, New York, USA, January, 2011. (Preferred reference for CloudSim)**
  * Bhathiya Wickremasinghe, Rodrigo N. Calheiros, Rajkumar Buyya, [CloudAnalyst: A CloudSim-based Visual Modeller for Analysing Cloud Computing Environments and Applications](http://www.cloudbus.org/papers/CloudAnalyst-AINA2010.pdf), Proceedings of the 24th International Conference on Advanced Information Networking and Applications (AINA 2010), Perth, Australia, April 20-23, 2010.
  * Rajkumar Buyya, Rajiv Ranjan and Rodrigo N. Calheiros, [Modeling and Simulation of Scalable Cloud Computing Environments and the CloudSim Toolkit: Challenges and Opportunities](http://www.cloudbus.org/papers/CloudSim-HPCS2009.pdf), Proceedings of the 7th High Performance Computing and Simulation Conference (HPCS 2009, ISBN: 978-1-4244-4907-1, IEEE Press, New York, USA), Leipzig, Germany, June 21-24, 2009.




[![](http://www.cloudbus.org/logo/cloudbuslogo-v5a.png)](http://cloudbus.org/)
