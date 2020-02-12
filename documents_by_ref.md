**Documents by File Reference**
----
  Retrieve documents data by file reference no

* **URL**

  `<SERVER URL>/api/file-document/:fileRefNo`

* **Method:**

  `GET`
  
* **Headers:**

  * **Accept:** `application/json` <br />
  * **Authorization:** `Bearer {token}`
  
*  **URL Params**

   **fileRefNo:** file reference no
   
   **Required:**
 
   `fileRefNo=[integer]`

* **Data Params**

  None

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** 
    ```
    {
      "10000632": {
        "soa": "http://forth-line.local/file/358260ae-5e7e-40d4-a26e-a187a0d9d58c/download",
        "rp": "http://forth-line.local/file/372c0c49-7a9c-42e1-b984-8b1b04c59c3e/download",
        "toeFile": "http://forth-line.local/file/3fb9823e-d284-423a-8690-eea241ea94da/download",
        "note-3": "http://forth-line.local/file/6a116c24-2e18-4ce8-ba20-9ffca794cf96/download"
      }
    }
    ```
 
* **Error Response:**

  * **Code:** 401 <br />
    **Content:** `{ message : "UNAUTHORIZED" }`


* **Sample Call:**

  ```
  {
    "10000632": {
      "soa": "http://forth-line.local/file/358260ae-5e7e-40d4-a26e-a187a0d9d58c/download",
      "rp": "http://forth-line.local/file/372c0c49-7a9c-42e1-b984-8b1b04c59c3e/download",
      "toeFile": "http://forth-line.local/file/3fb9823e-d284-423a-8690-eea241ea94da/download",
      "note-3": "http://forth-line.local/file/6a116c24-2e18-4ce8-ba20-9ffca794cf96/download"
    }
  }
  ```
