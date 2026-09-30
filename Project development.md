Project Development

Project development involves implementing the planned design of the automated standard laptop procurement workflow in ServiceNow. The development focuses on creating the Flow Designer workflow, connecting it with the Standard Laptop Service Catalog item, and testing the automatic task creation and assignment process.

1. Flow Creation

The first development activity is to create a new Flow Designer flow named “Standard Laptop Task.” The flow is created in the Global application and configured to run as a System User.

2. Trigger Configuration

A Service Catalog trigger is added to the flow. This allows the workflow to respond when the relevant Service Catalog process is initiated.

3. Catalog Task Development

A Create Catalog Task action is added to the flow. The Requested Item Record is used as the request item, and the task is configured with the required values:

Short Description: Laptop need to Configured
Description: Laptop need to Configured
Assignment Group: Hardware
Approval: Approved

The remaining fields are left at their default settings before completing the action.

4. Flow Activation

After configuring the actions, the flow is saved and activated. This makes the automation available for the Standard Laptop procurement process.

5. Service Catalog Integration

The Standard Laptop Service Catalog item is configured to use the newly developed Standard Laptop Task flow. The existing automations are removed and the new flow is added to the Process Engine configuration.

6. Request Processing

Users can access the Hardware section of the Service Catalog, select Standard Laptop, and choose Order Now to submit a request. The request then proceeds through the approval process.

7. Testing and Verification

After approval, the Requested Item is opened and the Catalog Tasks section is checked. The generated task is verified to ensure that the short description and assigned Hardware group have been updated correctly.

8. Development Outcome

The completed development provides an automated workflow in which an approved Standard Laptop request results in a configuration task being created and assigned to the Hardware team. This reduces manual processing and supports timely laptop configuration.
