# Branding the OpenShift 4 Console

The default installation of OpenShift 4 leaves plenty of room for customization.

https://docs.openshift.com/container-platform/4.7/web_console/customizing-the-web-console.html

## Out of the Box Presentation

![Fresh install OpenShift console screenshot](/images/Topology-NoBranding.png)

## Custom Branding and Environment Banner

Updating the Red Hat default OpenShift logo helps give an organization a sense of pride and ownership in the product they have chosen for their most critical business applications.

Additionally, some organizations choose to operate multiple OpenShift clusters for separating workloads by environment. Adding a uniquely color coded banner can help to quickly visually distinguish these separate environments, potentially reducing errors. 

Multiple banners (optionally enriched with links) can appear at a time, in the event a Message of the Day or other temporary advisory is required. 

![Branded and color coded OpenShift console screenshot](/images/Topology-Branded.png)

## The "customProductName" setting in action
The documentation on customizing the web console makes reference to a setting called "customProductName" in the Console operator. The name of this setting is rather vague but it's really quite valuable.

The setting replaces the default out-of-the-box browser title bar description of "Red Hat OpenShift Container Platform"

By defining this setting (and making it unique per cluster), your browser history becomes slightly more valuable by having an easily distinguishable cluster description, instead of a sea of "Red Hat OpenShift Container Platform" entries.

![Screenshot of customProductName in browser history](/images/BrowserHistory-ProductName.png)
