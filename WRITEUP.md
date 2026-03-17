# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

I decided to go with Web App Service. The analysis and justification according to me for the same is below:

Azure Virtual Machines provide Infrastructure-as-a-Service (IaaS), which gives full control over the operating system and server configuration. However, this also means that the developer must manage system updates, security patches, runtime installation, and scaling manually. In addition, the VM continues to incur costs as long as it is running, even if the application has little or no traffic. 

In contrast, Azure App Service is a Platform-as-a-Service (PaaS) solution designed specifically for hosting web applications. It removes the need to manage the underlying infrastructure and provides built-in features such as automatic scaling, load balancing, and integrated deployment from GitHub or other CI/CD tools. 

This helped me save time and resources and allowed me to focus on the application rather than server maintenance.

### Assess app changes that would change your decision.

According to me, if the CMS application remained a typical web-based platform with standard dependencies, App Service would continue to be my preferred choice, but if the application required greater infrastructure control or specialized configurations, migrating to a Virtual Machine environment would be justified. 

Azure Virtual Machines would become a more suitable option if the application required full control over the operating system, custom server configurations, or installation of specialized software that is not supported by Azure App Service. For example, if the CMS application needed specific system-level dependencies, custom networking configurations, or background services running alongside the web application, a VM would provide the flexibility to configure and manage these components. 

Additionally, if the application evolved into a large-scale system requiring complex infrastructure management, custom load balancing, or integration with legacy systems that depend on direct server access, a VM-based deployment might be more appropriate. 
In contrast, Azure App Service works best for standard web applications that follow common frameworks and do not require deep operating system control.
