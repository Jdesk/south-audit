---


---

<h2 id="south-audit">South Audit</h2>
<ol>
<li>Naming Conventions on Resources in AWS<br>
a.  domain - prod / staging - group name -  (resource group name) - resource type:</li>
</ol>
<h4 id="eg.-south.io-prod-south1a-elb">eg. south.io-prod-south1a-ELB</h4>
<ol start="2">
<li>Resource Group Creation - Resources in every stack will be part of the relevant resource group in aws</li>
<li>Security Groups - must also follow the naming conventions</li>
<li>Volumes - must also following naming convention strategy</li>
<li>Moving our domains / sites into aws - eg.  <a href="http://south.io">south.io</a> / <a href="http://heystack.is">heystack.is</a> - why is this not being hosted here? We should use Route 53 for all DNS.</li>
<li>RDS - must also following naming conventions</li>
<li><a href="http://heystack.is">heystack.is</a> has no ssl cert installed.  however one was requested through aws - in this fashion - that cert will only be able to be put in use - on aws infrastructure - eg. elastic load balancer - which we should be using.</li>
<li>Credential storage using credstash, kms, and dynamodb - I will set this up - all sensative keys can be stored using this method.  we will be able to fetch keys a</li>
<li>move all dns to route53 - <a href="http://south.io">south.io</a> is using bluehost.  it’s betters well to have everything under one roof</li>
<li>for all projects going forward - we can use docker - and a container scheduling / management service to scale apps as needed - I propose we use Rancher - because we will be able to effectively scale out applications, have them under one roof, deploy, and test our containerized applications across all clouds.</li>
<li>Documentation - we need a centralized area for documentation - atlassian confluence would be my choice - cut out google docs - let’s get it all under one space</li>
<li>All applications (unless developers recommend against) should be containerized.</li>
</ol>

