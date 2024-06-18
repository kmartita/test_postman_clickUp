# Test API Postman Project

This repository includes a Postman collection with tests categorized into two folders: Goals and Key Results (Parameterized). The collection is designed to be dynamic and data-driven, ensuring efficient and comprehensive testing of different API endpoints outlined in the API specifications for the [GetGoals](https://clickup.com/api/clickupreference/operation/GetGoals/) operation.

## Table of Contents
1. Setup local machine<br/>
2. Prerequisites<br/>
3. Basic concepts for building a collection<br/>
4. How to run the collection<br/>

## 1. Setup local machine
#### This guide assumes the following:
* Have **Postman** version 11.2.1 or higher installed on your system

## 2. Prerequisites:
#### Before proceeding, ensure you have the following:
* Basic understanding of JavaScript coding

## 3. Basic concepts for building a collection
#### Pre-request script for collection initialization
Before running the `ClickUp-Goals` collection, all current test data associated with goals will be removed to ensure a fresh starting point for each test. The necessary cleanup script for this operation is included in the Pre-request section of the collection.

#### Dynamic resolution of `team_id` and `user_id`
The `team_id` and `user_id` values are dynamically fetched based on the `user_name`, guaranteeing that the tests are consistently run with the latest and pertinent user details.

#### Goals Folder
Within the `Goals` folder are tests covering all API endpoints outlined in the API documentation for the [GetGoals](https://clickup.com/api/clickupreference/operation/GetGoals/) operation. These tests aim to comprehensively verify all goal-related functionalities.

#### Key Results (Parameterized) Folder
Inside the `Key Results (Parameterized)` folder, there is a singular test for the POST endpoint that is parameterized. This test is conducted utilizing a data-driven method with a JSON file, enabling thorough testing across various data scenarios.

## 4. How to run the collection
* Import project.
* In the Key Results (Parameterized) folder, the test that is parameterized utilizes a JSON data file named `key_results.json`. Add this file to the Data section of the Postman Runner for loading during test execution.
* Use the Postman Runner to execute the ClickUp-Goals collection, ensuring the pre-run cleanup script is executed to maintain data integrity.
