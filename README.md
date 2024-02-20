CONCEPTS OF GIT VERSION CONTROL SYSTEM AND IMPORTANT COMMANDS:

**WHAT IS GIT:** "Git is a distributed version control system that enables developers to collaboratively manage and track changes to source code. 
It allows developers to efficiently collect, maintain, and manage different versions of code in a decentralized manner. Through Git, teams can work 
together seamlessly, tracking changes, merging contributions, and maintaining a centralized repository of their project's history."

**TYPES OF VERSION CONTROL SYSTEMS:** There are two main types of version control systems: centralized version control systems and distributed version control systems.

**Centralized Version Control System (CVCS):
**
In a centralized version control system, developers commit and update code to a central repository, such as a remote server, folder, or storage location. This approach offers certain advantages and disadvantages:

**Advantages** :

Code Accessibility: All developers can easily access and track the code since it is stored in a central repository.

**Disadvantages** :

 Internet Dependency: An active internet connection is required for developers to access the code from the central repository. Without internet access, developers cannot retrieve 
 or update the code.

 Lack of High Availability: Since the code is solely stored in a central repository, any issues or downtime with the central repository can prevent developers from accessing the 
 code, leading to disruptions in the development process.

Overall, while centralized version control systems offer ease of access and collaboration among developers, they are susceptible to internet dependency and potential disruptions due to central repository issues.

Distributed version control system:

A distributed version control system (DVCS) empowers developers to seamlessly commit, update, push, and pull code between local repositories and central repositories like GitHub. The advantages of using a DVCS are manifold.

No Dependency on Internet Connection: With code committed to a local repository, developers can access it readily even in scenarios of limited internet connectivity.

High Availability: DVCS ensures High Availability (HAV) by storing code in both local and central repositories. Developers can access code from the local repository if unable to connect to the central repository, ensuring uninterrupted workflow.

Versioning Capabilities: DVCS automatically creates distinct versions of code upon each commit. Deleting a version does not affect other versions, providing a robust versioning mechanism for project history and rollback.

GitHub Integration: Through push/pull operations, developers synchronize code with central repository like Git-hub. This facilitates collaboration, enabling other developers to track changes and contribute to the project effectively.


