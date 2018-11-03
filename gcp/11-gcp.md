# App Engine

If you just want to focus on your development and/or code, use **App Engine**.

## PaaS (Platform as a Service)
* App Engine platform manages hardware, and networking infrastructure require to run your code.
* App Engine makes deployment, maintenance, and scalability easy so you can focus on innovation
* App Engine will scale your application automatically in response of the amount of traffic that the application receives
* You pay only the resources that you use
* App Engine is especially suited for building scalable web applications and mobile backends

Type of App Engine environments:
* Standard Environment
  * It is simpler
  * Offers simple deployment experience
  * Fine grain autoscale
  * Offers daily free usage quota
  * Usage based pricing
  * Distinct: Low utilization application might be able to run at no charge
  * SDKs for development, testing and deployment
  * Requirements: (provides run time)
    * Specific version of Java, Python, PHP and Go are supported
    * If you want to code in another language, **Standard Environment** is not right for you
    * Restriction on your code, by making it run in sandbox:
      * No writing local files (could be database instead)
      * All requests are timed out at 60s
      * Limits on third-party software
      ![Alt text](images/appenginestandardworkflow.png?raw=true "App Engine Standard Workflow")
* Flexible Environment:
  * If sandbox model does not work for you
  * It lets you specify the container that your App Engine runs in
  * Build and deploy containerized apps with click
  * No sandbox constraints
  * Can access App Engine resources
  
![Alt text](images/appengineenvscomparison.png?raw=true "App Engine Envs Comparisson")
