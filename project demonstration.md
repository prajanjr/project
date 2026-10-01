Project Demonstration
The project demonstration shows how the Standard Laptop procurement workflow works in ServiceNow from placing a request to creating and assigning the configuration task. The demonstration follows the three milestones defined in the project.
1. Open ServiceNow
First, open ServiceNow and access the required modules through the All menu.
2. Create and Activate the Flow
Open Flow Designer and select the Standard Laptop Task flow. The flow uses Service Catalog as the trigger and Create Catalog Task as the action. The task is configured for the Hardware assignment group and approved requests.
3. Configure Standard Laptop Service
Open Maintain Items and search for Standard Laptop. Under the Process Engine section, remove the remaining automations and add the Standard Laptop Task flow.
4. Place a Laptop Request
Navigate to:
Service Catalog → Hardware → Standard Laptop → Order Now
The user submits the Standard Laptop request through the Service Catalog.
5. Approve the Request
After submitting the request, open the Request Number and navigate to the Approvers section. The request is then approved to continue the workflow.
6. Verify Automatic Task Creation
After approval:
Requested Item → Catalog Tasks → Open Task
The generated Catalog Task can be checked to verify its updated status, Short Description, and Assignment Group.
7. Demonstration Flow
Open ServiceNow
       ↓
   Open Service Catalog
       ↓
Select Standard Laptop
       ↓
Click Order Now
       ↓
Submit Request
       ↓
Request Approval
       ↓
Approval = Approved
       ↓
Flow Designer Triggered
       ↓
Catalog Task Created
       ↓
Assigned to Hardware
       ↓
Laptop Configuration
9. Demonstration Result
The demonstration confirms that an approved Standard Laptop request can automatically generate a configuration task and assign it to the Hardware team. This demonstrates the project's objective of reducing manual intervention, minimizing delays, and improving the efficiency of IT procurement.

Demo Video Link:https://drive.google.com/file/d/1fXrHoK98RcVkUemdMA0kQh-2sV06iKV3/view?usp=drivesdk

Summary

The project, “Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer,” focuses on improving the standard laptop procurement process in ServiceNow. The existing process involves manual activities that can cause delays, configuration oversights, and additional workload for the IT department. The proposed solution uses ServiceNow Flow Designer to automate the creation and assignment of laptop configuration tasks.

The workflow connects the Service Catalog, approval process, Flow Designer, and Catalog Tasks. When a user requests a Standard Laptop and the request is approved, the flow automatically creates a configuration task and assigns it to the Hardware group. The implementation is organized into flow creation, flow assignment, and Service Catalog configuration, followed by testing and verification.

Conclusion

The project demonstrates how ServiceNow Flow Designer can be used to automate the standard laptop procurement process. The automated workflow reduces manual intervention by creating the required Catalog Task after approval and assigning it to the Hardware team.

The implementation helps provide timely laptop configuration, reduced user waiting time, improved resource utilization, and greater efficiency in IT procurement operations. Overall, the project provides a streamlined workflow for handling standard laptop requests and supports a more efficient procurement process.

Available next action: 
Create a downloadable PDF file here in this chat containing the finalized decisions and immediate actions above
