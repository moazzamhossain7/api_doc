**Filter documents**
----
  Retrieve documents data using filter

* **URL**

  `<SERVER URL>/api/file-document?{docType}&{soaType}`

* **Method:**

  `GET`
  
* **Headers:**

  * **Accept:** `application/json` <br />
  * **Authorization:** `Bearer {token}`
  
*  **URL Params**

   **docType:** List of docType <br />
   **soaType:** List of soaType
   
   **Optional:**
 
   `docType=[ ff,  rp, soa, note-1, note-2, note-3, fds, opt-in, report  ]`
   
   **Optional:**
 
   `soaType = [ soa-new-client,  soa-review-client, roa ]`

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** 
    
      ```
      {
        "10000550": {
          "note-2": "http://forth-line.local/file/1f031deb-e585-4b3d-bf11-be5b7e63ae53/download"
        }
      }
      ```
 
* **Error Response:**

  * **Code:** 401  <br />
    **Content:** `{ message : "UNAUTHORIZED" }`

  OR

  * **Code:** 200  <br />
    **Content:** `{ message : "Not Found" }`

* **Sample Call:**

  ``http://forth-line.local/api/file-document?docType=soa&soaType=roa,soa-new-client``

  * **Response:**

    ```
    {
        "10000001": {
          "soa": "http://forth-line.local/file/6c523ef9-b03c-49f1-a577-443cefd67326/download"
        },
        "10000002": {
          "soa": "http://forth-line.local/file/94afde7a-7141-4f36-9da5-9a5604189c5c/download"
        },
        "10000004": {
          "soa": "http://forth-line.local/file/1a7427b5-e692-450e-9f4f-3482a9238960/download"
        },
        "10000005": {
          "soa": "http://forth-line.local/file/a6a58b63-15a4-49ea-a4c7-794855e6436e/download"
        },
    }
    ```
