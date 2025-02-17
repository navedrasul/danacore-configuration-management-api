# API Endpoints and Service Contracts Definition Document
(for the Configuration Management App)

Below is a comprehensive list of APIs grouped by functionality:

---

## **1. User Role Management APIs**  
1. **Create Role** – `POST /roles` – Add a new role to the system.  
2. **Update Role** – `PUT /roles/{id}` – Modify an existing role.  
3. **Delete Role** – `DELETE /roles/{id}` – Remove a role from the system.  
4. **Get Role Details** – `GET /roles/{id}` – Retrieve detailed information about a specific role.  
5. **List Roles** – `GET /roles` – Fetch all available roles.  
6. **Assign Permissions to Role** – `POST /roles/{id}/permissions` – Assign a set of permissions to a specific role.  
7. **List Permissions** – `GET /permissions` – Retrieve all possible permissions available in the system.  

## **2. Workflow Configuration APIs**  
8. **Create Workflow** – `POST /workflows` – Add a new workflow definition.  
9. **Update Workflow** – `PUT /workflows/{id}` – Modify an existing workflow.  
10. **Delete Workflow** – `DELETE /workflows/{id}` – Remove a workflow definition.  
11. **Get Workflow Details** – `GET /workflows/{id}` – Fetch details of a specific workflow.  
12. **List Workflows** – `GET /workflows` – Retrieve a list of all workflows.  
13. **Activate/Deactivate Workflow** – `PATCH /workflows/{id}/status` – Enable or disable a specific workflow.  
14. **Test Workflow** – `POST /workflows/{id}/test` – Execute a test run for a specific workflow configuration.  

## **3. System Settings Management APIs**  
15. **Get Settings** – `GET /settings` – Retrieve the current system settings.  
16. **Update Settings** – `PUT /settings` – Modify one or more system settings.  
17. **Reset Settings** – `POST /settings/reset` – Reset settings to their default values.  
18. **List Default Values** – `GET /settings/defaults` – Fetch a list of default configuration values.  

## **4. Audit Logging APIs**  
19. **Get Audit Logs** – `GET /audit/logs` – Fetch logs with optional filters (e.g., date range, user, action type).  
20. **Export Audit Logs** – `POST /audit/logs/export` – Download logs in a specific format (e.g., CSV, JSON).  
21. **Get Audit Log Details** – `GET /audit/logs/{id}` – Retrieve detailed information for a specific log entry.  

## **5. Metadata and Support APIs**  
22. **Get Workflow Triggers** – `GET /workflows/triggers` – Fetch available triggers for workflows.  
23. **Get Workflow Actions** – `GET /workflows/actions` – Fetch available actions for workflows.  
24. **Health Check** – `GET /health` – Verify the app's health status.  
25. **Version Info** – `GET /version` – Retrieve the current version of the app.  