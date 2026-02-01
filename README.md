# Oil-Spill-Detection-System-OSDS-
The purpose of this project is to enable faster detection and attribution of oil spills in ocean waters, allowing marine traffic authorities to initiate response and enforcement actions with minimal delay and preventing water pollution.

## System functional capabilities

### 1. Event awareness
The system can **become aware** that a oil spill has occured.
*What does this part do?*
- The system does not wait for manual reports
- Awareness may be probalistic, not absolute
- It values more awareness than perfect certainty

### 2. Spatial localization
The system can locate where the spill is occuring
*What does this enable?*
- Jurisdiction determination (Exact coordinates + maritime navigation contexys)
- Risk prioritization

### 3. Temporal context
The system can estimate when the spill likely occured
*Why is this part so important?*
- Improves attribution
- Reduce the number of the candidate vessels
- Affects reponse urgency
- Provides estimations for future investigations (Event reconstructions, correlation with vessel movements and escalation decisions)

### 4. Attribution support
The system is able to provide identification for the vessels responsible for the spill.
*Why is this part the axis of the project?*
- The system does not accuse, it narrows candidates
- Supports investigation, not replaces it
- Reduce ambiguity 

### 5. Action Triggering
The system is able to prompt timely action by the appropiate authorities to reduce time action.
*This is the system's main purpose*
- Awareness becomes reponse
- The time action is reduced by constant detection and quick response
- Notification and prioritazion

-------------------------------------------------------------------------------------------------

## INPUTS & OUTPUTS

***INPUTS***
### Class 1 -Marine Surface Anomaly Signals
*This input represents that something abnormal is occuring in the ocean surface*
- Spatially referenced (Tied to an specific location)
- May represent indirect evidence, not confirmation
  *How will this class recieve this information?*
  

### Class 2 -Maritime Traffic Movement Information
*This input represents how vessels move through maritime space over time*
- Idenity vessel presence in the area
- Include movements paths
- Allow time reconstruction

### Class 3 -Temporal Reference Information
*Support time-window estimation*
- Correlate anomalies with vessel movements
- Establish before/after patterns and relationships

### Class 4 -Maritime Judrisdiction and Context Information
  *Defines an action routing*
- What authoritiy applies
- Which actions are legally relevant


-------------------------------------------------------------------------------------------------

***OUTPUTS***
### Class 1 -Spill Suspicion Alerts
*Trigger awareness*
- It communicates that a suspected spill event exists
- Where it likely occurred
- When it likely began

### Class 2 -Candidate Vessel set
*Enable accountability and future investigation*
- It provides a short list of potential responsibles linked to the event
- It doesn't accuse, it prioritize investigation

### Class 4 -Event Record for follow-up
*Enable learning and patterns indetification*
- Events are not lost
- Patterns recognition for the future
