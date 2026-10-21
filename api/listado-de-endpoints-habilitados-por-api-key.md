# Listado de Endpoints habilitados por API-Key

A continuación se listan los endpoints disponibles para su consumo mediante API Key. Para ver el detalle de parámetros, mensajes y una explicación detallada de su uso, puede consultar el repositorio de documentación [API GlobalSuite®](https://docs.globalsuitesolutions.com/docs/)

|  |  |  |
| --- | --- | --- |
| **Recurso** | **Operación** | **URL / Endpoint** |
| Analysis Asset | GET | /analysis/{analysisId}/assets |
|  | POST | /analysis/{modelId}/assets/{objectId} |
|  | DELETE | /analysis/{modelId}/assets/{objectId} |
|  | PUT | /analysis/{modelId}/assets/{objectId} |
| Analysis Asset Control Calculate Request | POST | /analysis/{modelId}/assets/{assetId}/controls/{controlId}/calculateRequest |
| Analysis Asset Threat Calculate Request | POST | /analysis/{modelId}/assets/{assetId}/threats/{threatId}/calculateRequest |
| Analysis Asset Threat Control Calculate Request | POST | /analysis/{modelId}/assets/{assetId}/threats/{threatId}/controls/{controlId}/calculateRequest |
| Analysis Controls | GET | /analysis/{modelId}/controls |
|  | GET | /analysis/{modelId}/controls/{objectId} |
|  | POST | /analysis/{modelId}/controls |
|  | DELETE | /analysis/{modelId}/controls |
|  | DELETE | /analysis/{modelId}/controls/{objectId} |
| Analysis Controls Actions | PUT | /analysis/{modelId}/controls/{controlId}/actions/{actionId} |
| Analysis Controls Dimensions | PUT | /analysis/{modelId}/controls/{objectId}/dimensions/{dimensionId} |
| Assets | GET | /assets |
|  | POST | /assets |
|  | GET | /assets/{modelId} |
|  | DELETE | /assets/{modelId} |
|  | PUT | /assets/{modelId} |
| Asset Dependency | PUT | /assets/{modelId}/dependency/{objectId} |
|  | POST | /assets/{modelId}/dependency/{objectId} |
|  | DELETE | /assets/{modelId}/dependency/{objectId} |
|  | PUT | /assets/{modelId}/dimensions/{objectId} |
| Asset Threat | GET | /assets/{assetId}/threats/{threatId} |
|  | POST | /assets/{assetId}/threats/ |
|  | PUT | /assets/{assetId}/threats/{threatId} |
|  | DELETE | /assets/{assetId}/threats/{threatId} |
| Asset Threat Supervisor | PUT | /assets/{assetId}/threats/{threatId}/supervisor |
| Asset Threat Risk | POST | /assets/{assetId}/threats/{threatId}/risks/{riskId} |
|  | DELETE | /assets/{assetId}/threats/{threatId}/risks/{riskId} |
| Asset Threat Control | GET | /assets/{assetId}/threats/{threatId}/controls |
| Asset Analysis Threats | GET | /assets/{assetId}/analysis/{analysisId}/threats/ |
|  | PUT | /assets/{assetId}/threats/{threatId}/dimensions/{dimensionId} |
| AssetAttributes | GET | /assetAttributes |
|  | GET | /assetAttributes/{modelId} |
| Category | PUT | /categories/{modelId} |
|  | GET | /categories/{modelId} |
|  | GET | /categories |
|  | POST | /categories |
| Company Analysis | GET | /companies/{modelId}/analysis/ |
| Company Roles | GET | /companies/{modelId}/roles |
| Company Rules | PUT | /rules |
| Controls | PUT | /controls/{modelId} |
| Dimensions | GET | /dimensions |
|  | GET | /dimensions/{modelId} |
| Dimension Level | GET | /dimensions/{modelId}/levels |
|  | GET | /dimensions/{modelId}/levels/{levelId} |
| Dimension Group | GET | /dimensionGroups |
|  | GET | /dimensionGroups/{modelId} |
| Employees | GET | /employees |
|  | GET | /employees/{modelId} |
|  | POST | /employees |
| Processes | GET | /processes |
|  | GET | /processes/{modelId} |
| Risk | GET | /risks |
| Roles | GET | /roles |
| Services | GET | /services |
|  | GET | /services/{modelId} |
|  | PUT | /services/{modelId} |
|  | POST | /services |
|  | DELETE | /services/{modelId} |
| Tickets | GET | /tickets |
|  | GET | /tickets/{modelId} |
|  | PUT | /tickets/{modelId} |
|  | POST | /tickets/{modelId}/copy |
|  | DELETE | /tickets/{modelId} |
| Ticket Employees | GET | /tickets/{modelId}/employees |
|  | PUT | /tickets/{modelId}/employees/{objectId} |
|  | POST | /tickets/{modelId}/employees/{objectId} |
|  | DELETE | /tickets/{modelId}/employees/{objectId} |
| Ticket Files | POST | /tickets/{modelId}/files |
| TicketFields Options | GET | /ticketFields/{modelId}/options |
| TicketFields Option SubOptions | GET | /ticketFields/{modelId}/options/{objectId}/subOptions |
| TicketMenu Type | GET | /ticketMenu/{modelId}/type |
| TicketOptions | GET | /ticketOptions |
| TicketTableStructures | GET | /ticketTableStructures |
| TicketTypes | GET | /ticketTypes |
| TicketType Fields | GET | /ticketTypes/{modelId}/fields |
|  | POST | /ticketTypes/{modelId}/tickets |
| TicketType Fieldsets | GET | /ticketTypes/{modelId}/fieldSets |
| Users | GET | /users |
|  | GET | /users/{modelId} |
|  | POST | /users |
|  | PUT | /users/{modelId} |
|  | DELETE | /users/{modelId} |
| Workflows | GET | /workflows |
