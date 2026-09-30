Brainstorming and Ideation
1. Brainstorming

Brainstorming is the initial stage of the project where different ideas are generated to identify problems in the existing IT procurement process and find possible solutions. The main focus was on reducing manual work, improving task allocation, and ensuring that standard laptop requests are processed efficiently.

During brainstorming, the following key problems were identified:

Standard laptop requests require manual processing.
Configuration tasks may be delayed or overlooked.
IT staff need to manually create and assign configuration tasks.
Manual intervention can result in errors and delays.
Users may experience longer waiting times before receiving a configured laptop.
IT resources are not always allocated efficiently.

The project therefore focused on creating an automated workflow using ServiceNow Flow Designer to automatically generate and assign configuration tasks after the required approval.

2. Ideation

Based on the brainstorming results, several ideas were considered for improving the procurement process. The selected idea was to automate the standard laptop ordering and configuration workflow using ServiceNow Flow Designer.

The proposed solution includes:

Create a dedicated flow named “Standard Laptop Task.”
Trigger the flow through the Service Catalog.
Automatically create a Catalog Task after the request is approved.
Set the task description to indicate that the laptop needs configuration.
Automatically assign the task to the Hardware assignment group.
Connect the flow to the Standard Laptop service catalog item.
Allow users to place laptop requests through the Service Catalog.
Track the request, approval, and catalog task status.

This approach was selected because it reduces manual intervention and automatically allocates configuration work to the appropriate hardware team.

3. Proposed Idea

The final idea is to develop an automated standard laptop procurement and configuration workflow in ServiceNow.

Input:
User requests a standard laptop through the Service Catalog.

Process:
Request → Approval → Flow Designer → Catalog Task Creation → Hardware Assignment → Laptop Configuration

Output:
A configuration task is automatically created and assigned to the Hardware team, helping ensure that the laptop is configured promptly upon arrival.

4. Expected Benefits
Reduced manual intervention
Faster processing of laptop requests
Automatic task creation and assignment
Reduced possibility of missed configuration tasks
Better utilization of IT resources
Reduced user waiting time
Improved procurement efficiency
Better overall user experience

The project's intended outcomes are consistent with the stated objective of improving efficiency, reducing errors, optimizing resource allocation, and providing a smoother user experience.
