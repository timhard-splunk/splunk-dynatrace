# splunk-dynatrace
Splunk App &amp; Add-On for Dynatrace

## What's Needed?
- Downloads
    - Splunk Add-on for Dynatrace
    - Splunk App for Dynatrace


- Dynatrace Information Required
    - Dynatrace API base URL 
    - Dynatrace API Authorization Token
    
## Installation
The installation consists of installing both the *Splunk Add-on for Dynatrace* and the *Splunk App for Dynatrace*.   
  - The Add-on is responsible for executing the rest API calls and collecting the data from Dynatrace.  
  - The App provides a collection of dashboards and saved searches.  
  
To install, navigate to Apps --> Manage Apps and select the “Install app from File” button.  Specify the location of the file you downloaded and install it.   

## Configuration
The Splunk Add-on for Dynatrace contains a global configuration for your Instana account URL and API authorization token.  Enter those values on the **Configuration** tab in the Add-on.

From the Inputs menu, create new Input for the data you wish to collect.  Each Input requires 4 parameters:
  - Input Name 
  - Pollling interval
  - Splunk Index to use
  - Your Dynatrace tenant URL
  - Your Dynatrace API Key
  - The Timeseries Metrics Input collects a pre-defined set of Dynatrace metrics
  
## Start Searching
Once the Splunk Add-on for Dynatrace is installed and configured you can execute searches using any of the following searches: 
```
sourcetype="dynatrace:metrics"
sourcetype="dynatrace:problem"
sourcetype="dynatrace:entity"
sourcetype="dynatrace:single-metric"
```

----  
