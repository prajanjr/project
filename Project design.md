Project Design

The project design describes how the automated standard laptop procurement workflow is structured and how the different ServiceNow components interact. The design is centered on Flow Designer, the Service Catalog, the approval process, and automatic Catalog Task creation.

1. System Architecture

The proposed system follows this workflow:

              USER
                │
                ▼
       Service Catalog
       "Standard Laptop"
                │
                ▼
        Place Request
                │
                ▼
          Approval
                │
        ┌───────┴───────┐
        │               │
     Approved         Not Approved
        │               │
        ▼               ▼
  Flow Designer       Request
        │             Process Ends
        ▼
 Create Catalog Task
        │
        ▼
  Hardware Assignment
        │
        ▼
 Laptop Configuration
        │
        ▼
     Completed

The project document specifies that the flow is triggered through the Service Catalog and uses the Create Catalog Task action. The generated task is assigned to the Hardware group after approval.

2. Main Components
A. Service Catalog

The Standard Laptop is provided as a Service Catalog item. Users access the Hardware category, select Standard Laptop, and choose Order Now to submit their request.

B. Approval Module

The submitted request goes through the approval process. The workflow uses the Approved status before creating the configuration task.

C. Flow Designer

The main automation component is a Flow named “Standard Laptop Task.” It uses the Service Catalog as its trigger and automatically performs the required task creation activity.

D. Catalog Task

After approval, the system creates a Catalog Task with:

Short Description: Laptop need to Configured
Description: Laptop need to Configured
Assignment Group: Hardware
Approval: Approved

These values are configured in the Flow Designer action.

3. Process Design

The overall process is designed as:

Request → Approval → Automation → Task Creation → Hardware Assignment → Configuration

The Standard Laptop service item is configured to use the newly created flow, replacing the remaining automations for that item.

4. Task Monitoring Design

After the request is submitted and approved, the user can open the Requested Item and view the Catalog Tasks section. The task record displays the updated status, short description, and assigned group.

5. Design Objective

The design aims to create a simple automated workflow that minimizes manual intervention, ensures configuration tasks reach the appropriate Hardware team, reduces delays, and provides a more efficient laptop procurement experience.
