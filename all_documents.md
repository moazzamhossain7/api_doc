**All documents**
----
  Retrieve all documents data as json format

* **URL**

  `<SERVER URL>/api/file-document`

* **Method:**

  `GET`
  
* **Headers:**

  * **Accept:** `application/json` <br />
  * **Authorization:** `Bearer {token}`
  
*  **URL Params**

  None

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** 
    
      ```
      {
        "10000002": {
          "ff": "http://forth-line.local/file/62b62ccf-060d-4997-a3a7-15b0f7481632/download",
          "report": "http://forth-line.local/file/81248f34-125f-4d20-8672-6a68ed7124f1/download",
          "soa": "http://forth-line.local/file/94afde7a-7141-4f36-9da5-9a5604189c5c/download"
        }
      }
      ```
 
* **Error Response:**

  * **Code:** 401  <br />
    **Content:** `{ message : "UNAUTHORIZED" }`


* **Sample Call:**

  ``http://forth-line.local/api/file-document``

  * **Response:**

    ```
    {
          "10000002": {
            "ff": "http://forth-line.local/file/62b62ccf-060d-4997-a3a7-15b0f7481632/download",
            "report": "http://forth-line.local/file/81248f34-125f-4d20-8672-6a68ed7124f1/download",
            "soa": "http://forth-line.local/file/94afde7a-7141-4f36-9da5-9a5604189c5c/download"
          },
          "10000004": {
            "soa": "http://forth-line.local/file/1a7427b5-e692-450e-9f4f-3482a9238960/download",
            "note-1": "http://forth-line.local/file/94c26746-0220-4371-bc0c-db055bf24b2c/download",
            "report": "http://forth-line.local/file/db08f911-481c-47bc-80a2-a6c29e343b7a/download",
            "ff": "http://forth-line.local/file/de0480ca-b37c-478b-80ec-0b60a7975ffd/download"
          },
          "10000005": {
            "report": "http://forth-line.local/file/1a72a9d0-7898-49a3-9a11-9b1e534dcd34/download",
            "note-1": "http://forth-line.local/file/6bce462b-2d2b-4f01-be69-958dcb6573e4/download",
            "ff": "http://forth-line.local/file/99acb7e5-56ac-491e-8185-e4728459fcdf/download",
            "soa": "http://forth-line.local/file/a6a58b63-15a4-49ea-a4c7-794855e6436e/download"
          },
    }
    ```
