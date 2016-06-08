# SRX - Search and Rescue Data Exchange Protocol

SRX is an XML Schema document defining a common language for exchanging Search and Rescue data between different software packages.


## Motivation

This project is intended to provide a standard way for software packages used in search and rescue to easily communicate with each other. 

By providing a standard we hope to save time and effort spent on searches. On those big operations, where multiple groups work together, getting lists of personnel and resources into a common database when the groups use different software can be time-consuming and wasteful of resources. We hope to solve that by developing a communication standard - a common language - that works for the benefit of the whole search and rescue sector. While it may seem easier to simply mandate that everyone should use the same software package, different packages suit different groups' needs, and diversity is a good thing. Experience also shows that the software world changes rapidly, providers and products come and go and the only sure thing is that whatever tools we are using today will be obsolete in five years time. 


A data communication standard helps to insure against obsolescence by enabling import and export of data in a common format. 


## Contributing to SRX

#### If you are a software developer:

Please consider adopting the SRX format into your search and rescue software. The simplest way would be to build SRX import and export functions using standard XML libraries. This will help to ensure that your software is compatible with others and will help to make your software more efficient and effective. See the Developers section below for technical details. 

#### If you're a SAR practitioner:

Use software that supports the SRX standard. When you make decisions about which software to adopt consider whether it supports standard ways of communication or standard ways to import and export your data. While spreadsheets are a valuable tool thay are not a standard. We want to achieve a way to prevent your data being "locked in" to any one product, so that you can easily work togther with other groups when the need arises. 

If the software you currently use doesn't support SRX, contact the developers and ask them to add it in. 

#### If you are in a governance role:

Consider the need for data standards in the SAR sector. Just as we adopt common terminology to make our incident management teams able to interoperate, we need standards to ensure the interoperability of our software. Technology investment can be expensive, and to get the best returns we need strategies to deal with rapid evolution of software and hardware. Defining and adopting standards is key to mitigating the risks of technological obsolescence. Please encourage your organisation to develop and adopt data standards - including this one. 



## Developer notes

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

See the [SRX Schema file formatted as documentation](http://www.landsar.org.nz/SRX/1/0/srx.xml) 

### Sample files

Some sample files are included in the examples directory.

### To Do
 
   - Complete the development of Section 2 Operational information.
   - Develop Section 3 Post-operational information. 
   - Write reference implementation apps.




   