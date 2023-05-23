# Index-based-Search-Enabler-REST-API-
### A simple Backend approach of generating a REST API that facilitates an easy and efficient search enabler using Indexes (can be Created as well as Deleted in the API), which is demonstrated using a Sample Movie DB

## ***STEPS TO BEGIN***
1. You can use this Project by simply installing the needed Packages (at your terminal), kindly refer the _"package.json"_ file and install the required, by cross checking the *"dependencies"* (NOTE make sure all these files/Folders are inside a __single Folder__ and then install the packages while inside that single Folder).
2. At the *.env* file, we can change *PORT* (to your desire Number) as well as add your own *MongoDB URI* so as to establish a connection to your Data base (NOTE: like right before the **'?'** in your URI you can add your Database name ,Existing or not as the Project already has a Schema (which you can change) which will handle the needed changes but you can add your DB's name if you want to merge the forthcoming Documents).
3. Based on  _"Routes.js"_ file, there are various routes to handle corresponding requests (and the corresponding responses are at *"Controller.js"*).
4. To run the Program type **"npm run api"** in the terminal (can be altered at _"package,json"_ file at *"scripts"*).
5. Recommend to test the API using Postman or Thunder Client, etc. (Extensions also avaialble in Visual Studio).

## ***API TESTING***
1. After successfully running the code, you can test this API using applications such as Postman, Thunder Client, etc. (Here we Illustrate using Postman).
2. This API has 8 requests set on *Routes.js* file, here we can show how to run these requests on Postman (__NOTE: *All Responses* are also shown in the Code's _Terminal___).
  ### A. To Get All Documents ***"localhost:5000/api/Movie/"***
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/e689a87e-d87c-4177-a490-7025b3cdf6ab)
  
  ### B. To Get a Single Document(s) Based on Key:Value ***"localhost:5000/api/Movie/Search?'field1'='value1'&'field2'='value2'"***
  
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/5e60c1fb-d2cc-4814-95c3-3b640a9255dc)
  
  **NOTE: Based on the query we will also get the _".explain('executionStats')"_ Part at the bottom of the Response**
  
  ### C. To Add a new Document ***"localhost:5000/api/Movie/AddMovie/"***
  
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/bc7732d5-e385-423c-ac43-19d3003f5726)

  ### D. To Update an Existing Document ***"localhost:5000/api/Movie/ModMovie/'Document Name'"***

  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/942fd750-a854-4569-88ad-00e78ec10035)

  ### E. To Delete Existing Document(s) ***"localhost:5000/api/Movie/DeleteMovie?'field1'='value1'&'field2'='value2'"***
  
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/2acfc4bb-2874-4090-aa93-c61b1a1611d5)

  ### F. To Get All Existing Indexes ***"localhost:5000/api/Movie/Index/"***
  
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/6ac8058d-7bec-4da7-b1db-612a9225bfbd)

  ### G. To Add New Index(es) ***"localhost:5000/api/Movie/Index/"***
  
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/65f7447e-d0f7-42e3-a38a-431b4b4434f0)
  
  **NOTE: Now that you have created Indexes, again try to perform some search query that has similar fileds that of the created Indexes and now check out the _"executionTimeMillis"_**

  ### H. To Delete Existing Index(es) ***"localhost:5000/api/Movie/DeleteIndex/"***
  
  ![image](https://github.com/5010w1ng91xy/Index-based-Search-Enabler-REST-API-/assets/110966686/49aa479d-691e-4e8a-9be5-d3641af8c755)


```diff 
! Enjoy (づ｡◕‿‿◕｡)づ   &&   Happy Coding (▀̿Ĺ̯▀̿ ̿)  !
