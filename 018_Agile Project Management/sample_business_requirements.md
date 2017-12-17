# Fulfillment and Distribution System

## Executive Summary

Fulfillment and Distribution System is an application catered to businesses for product fulfillment and distribution.

## Business Objectives

The objective of this application is to provide the ability to automate processes for fulfillment and distribution.  This reduces errors, delays and overhead costs.

## Background

This application is will benefit our client because currently the client has no manpower to process and fulfill from packaging to shipping their products to their customers. 

## Scope

The scope of the application must have the ability to:
  Import the files 
  Process the information to the Fulfillment System
  Merge the documents using a word processing software
  Generate the print files

## Functional requirements

#### Import the files 

This process takes the import files from the client's site and transfers data to the local database. It is then ready for processing into the Fulfillment System.

#### Process the information to the Fulfillment System

1. Validation Check. This process undergoes null or empty validations. 
    Checks for empty OrderIds
    Checks for empty orders
    Checks for empty shipping and billing addresses
    Checks if the order items exist in Inventory table
    
2. Inventory Check - This process checks if there is enough quantity. If there is not enough quantity, the order will be rejected.

3.  Container Processing - This process calculates the weight and other dimensions of the orders to determine the correct shipping container.

4. Mail Carrier Service - This process determines the type of mail service to use whether via USPS, UPS, priority mail, express mail, etc.

5. Jobbing Process - This will process the job orders. It will also generate the mailing labels, assign tracking numbers and calculate shipping cost.

6.  Print Packing Slip – This process will generate and print the packing slip.

## Personnel requirements

A team of a project lead, a senior developer and 2 junior developers will be recommended for the project to handle the design, prototyping, development, QA, documentation and deployment.

## Delivery schedule

Phase 1 – This is the Import phase. A project will be developed whose objective is to import files from Client's site via FTP and import them to our system. This process involves extracting the zip files, reading and transfering data to the various tables such as Orders, Inventory, Address, etc. in our local databases. Phase 1 is expected to be delivered in one month.

Phase 2 – This is the Validation phase of the Fulfillment System. It will read data from the various tables and undergo the process of validation by checking for empty or null values. Phase 2 is expected to be delivered in 2 weeks.

Phase 3 – This is the Inventory phase of the Fulfillment System. It first checks the inventory of all the items. If there is enough inventory, the fulfillment process will continue. Otherwise, the system will reject the orders. Phase 3 is expected to be delivered in one month.

Phase 4 -  This is the Container phase of the Fulfillment System. The system calculates the dimensions and weight of the orders to determine the correct box size for shipping. Phase 4 is expected to be delivered in one month.

Phase 5 – This is the Mailing phase of the Fulfillment System. The system will provide the best shipping option for a particular order, whether sent locally or international. Phase 5 is expected to be delivered in 1.5 months.

Phase 6 – This is the Jobbing phase of the Fulfillment System. The system will provide the list of items, quantity to pull out from the warehouse. The system will also generate the mailing labels, assign tracking numbers and calculate shipping costs. Finally, printing of the packing slip is processed here. Phase 6 is expected to be delivered in 1.5 months.

Phase 7 – This is the testing phase. Testing is expected to be completed in 3 weeks.

Phase 8 – This will be the deployment phase. 

## Other requirements


## Assumptions

The system will be reliant on the availability of USPS API and UPS API for mailing services. It is also reliant on inventory of materials.

## Limitations

Processing of customer returns is not included in the scope of the project.

## Risks

Personnel retention and experience is seen as a risk that may cause delay or failure of the project.  
