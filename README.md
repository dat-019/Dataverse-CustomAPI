# CustomAPI
Dataverse Custom API
- Dataverse Custom API vs former Custom Workflow Activity
- Why we should mirgate custom workflow activity (called in a custom action) to Dataverse Custom API:
  - Their comparison regarding the perfomance matter, Dataverse Custom API is slightly better perfomance, according to the following article https://akaskela.com/2021/07/08/dataverse-performance-custom-api-vs-action-with-cwa/
  - Also, they provide the possibility to be executed in a Background Operation reducing overall System Load. This feature is currently in preview. Once it reaches GA we can/should replace the Async-Execution with a Background Operation -> documentation https://learn.microsoft.com/en-us/power-apps/developer/data-platform/background-operations?tabs=sdk
- Demonstration: client js -> call custom API -> invoke Azure Endpoint API (previously custom api was custom action)
