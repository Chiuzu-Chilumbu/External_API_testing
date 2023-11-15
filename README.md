# ComfyWings-Python External API Testing

Welcome to the ComfyWings-Python External API Testing Repository. This repository has been specifically established to facilitate Continuous Integration/Continuous Deployment (CI/CD) pipeline activities for the Amadeus API, which is integral to the ComfyWings Python project. Key highlights of this repository include:

1. **CI/CD Pipeline for Amadeus API**:
   - The primary purpose of this repository is to enable an automated CI/CD pipeline for the Amadeus API integration within the ComfyWings Python project.
   
2. **API Testing Using Postman**:
   - Comprehensive testing of the Amadeus API is conducted utilizing the Postman testing framework.
   
3. **JavaScript Test Suites**:
   - Test suites within this repository have been meticulously crafted using JavaScript to ensure thorough and reliable API testing.

## API Test Documentation

1. **Req Desc (Requirement Description)**: A brief description of what the API call is supposed to do or the specific requirement being tested.
2. **TC ID (Test Case ID)**: A unique identifier for each test case.
3. **Test Description**: A detailed description of what the test case will validate.
4. **Test Data**: Any input data used for the test case.
5. **Expected Result**: What the outcome should be if the API is working as intended.
6. **Actual Result**: The actual outcome received when the test case is executed.
7. **Test Execution**: Status of the test (e.g., Pass, Fail, Blocked, Not Executed).
8. **Defects**: Whether any defects were found during the test (Yes/No).
9. **Def Desc (Defect Description)**: A description of the defect, if any, including steps to reproduce, severity, and screenshots if applicable.
10. **Notes**: Additional remarks or observations relevant to the test case.


Below is the API test documentation detailing the test cases and their outcomes:

| Req Desc | TC ID | Test Description | Test Data | Expected Result | Actual Result | Test Execution | Defects | Def Desc | Notes |
|----------|-------|------------------|-----------|-----------------|---------------|----------------|---------|----------|-------|
| Token Authentication - Obtain Access Token | TC-01 | Verify that the environment variables are set and not empty. Post to obtain access token. | `{ "client_id": "xxxx", "client_secret": "xxxx", "grant_type": "client_credentials" }` | 200 OK, Token received in response, Environment variable set with token. | 200 OK, Token received, Environment variable set. | Pass | No | - | Response received in 643ms. |
| Token Authentication - Get Token Information | TC-02 | Perform a GET request to verify the token information is correct. | - (Token from previous test) | 200 OK, Response contains the expected properties. | 200 OK, Expected properties present in response. | Pass | No | - | Response received in 284ms. |
