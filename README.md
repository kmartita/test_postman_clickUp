# ClickUp-Goals

## Overview

This repository contains a parameterized collection of tests for ClickUp's Key Results endpoint. The collection is designed to be dynamic and data-driven, ensuring efficient and comprehensive testing of various API endpoints as specified in the API requirements.

## Steps

1. **Pre-Request Script for Collection Initialization**
   Before running the `ClickUp-Lesson6-ByParameterisedKeyResults` collection, all existing test data related to goals is deleted. This ensures that each test starts with a clean slate. The required cleanup script is included in the Pre-request section of the collection.

2. **Dynamic Resolution of `teamId` and `userId`**
   The values for `teamId` and `userId` are dynamically retrieved based on the `userName`. This ensures that the tests are always executed with the most up-to-date and relevant user information.

4. **Goals Folder**
   The `Goals` folder contains tests for all endpoints described in the [API requirements](https://clickup.com/api/clickupreference/operation/GetGoals/). These tests ensure that all functionalities related to goals are thoroughly tested.

6. **Key Results (Parameterized) Folder**
   The `Key Results (Parameterized)` folder contains a single, parameterized test for the POST endpoint. This test is executed using a data-driven approach with a JSON file, allowing for comprehensive testing across multiple data sets.

## How to Run

1. **Setup Environment Variables**
   Ensure that all necessary environment variables such as `base_url`, `userId`, `teamId`, `userName`, and any other required variables are set in your Postman environment.

2. **Load JSON Data File**
   The parameterized test in the `Key Results (Parameterized)` folder uses a JSON data file (key_results.json). Load this file in the Postman Runner under the Data section.

3. **Run the Collection**
   Use the Postman Runner to execute the `ClickUp-Lesson6-ByParameterisedKeyResults` collection, ensuring the pre-run cleanup script is executed to maintain data integrity.
