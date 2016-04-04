# SRX - Search and Rescue Data Exchange Protocol

SRX is an XML Schema document defining a common language for exchanging Search and Rescue data between different software packages.

## Motivation




## Using SRX



## Contributing to SRX

Fork the project on github and send pull requests to have your changes incorporated into the spec.

## Documentation

The schema is divided into four sections. 

#### 1. Pre–Operational information.
   This includes anything we know before an operation begins.

   - SAR members
   - SAR Groups
   - Group officers
   - Pre-plans
   - Resources

#### 2. Operational information 

   This models information generated during a SAR operation. It is structured using the hierarchy found in an Incident Action Plan:

   - Incident Action Plan
      - Operation
         - Operational Period
            - Teams
            - Tasks
            - Subject
            - Communications Plan
            - Incident Objectives
            - Medical Plan
            - Safety Plan
            - Sector Assignments
            - Situation Report
            - Weather Forecast

#### 3. Post–Operational information

   This models any information generated after an operation. 
   - Debrief notes
   - Review notes
   - Statistical reports
		
#### 4. Type declarations

   This section contains utilty type declarations needed as building blocks for the above complex types. 
   
   
### Complete XSD specification 

See the [SRX Schema file formatted as documentation](http://www.landsar.org.nz/SRX/1/0) 

### Sample files

   