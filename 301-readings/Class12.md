
# CRUD

---

**In your own words, describe what each group of status code represents:**

**100's =** informational responses that indicate that the request was received and is continuing.

**200's =** successful responses that informs you that the the request was successfully processed.

**300's =** indicate that additional action is needed to complete the request.

**400's =** indicate the problem is caused by the client. 

**500's =** indicates that the problem is caused by the server.

**What is a status code 202?**

 It’s the basic status code to tell the client everything went good. Since we don’t create endpoint accessible resource when creating an access token

**
What is a status code 308?**

informs the client that there is a new URL that has the data instead of the current URL. 

**What code would you use if an update didn't return data to a client?**

204 or 404

**What code would you use if a resource used to exist but no longer does?**

409

**What is the 'Forbidden' status code?**

4.3

**Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

So that we hide it for others can change the path.

**What is middleware?**

A software between the OS and the Apps running on the OS, basically the hidden translator.

**What does app.use(express.json()) do?**

Parses the JSON requests then pusts the parsed data in req. 

**What does the /:id mean in a route?**

it's a dynamic route, so req.params.id will be whatever comes after summary/ in that specific request.

**What is the difference between PUT and PATCH?**

PUT is a method of modifying resource where the client sends data that updates the entire resource . PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.

**How do you make a default value in a schema?**

Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

**What does a 500 error status code mean?**

Is a generic error response. It means that the server encountered an unexpected condition that prevented it from fulfilling the request.

**What is the difference between a status 200 and a status 201?**

The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed. A 201 status code indicates that a request was successful and as a result, a resource has been created.

---
---

## Things I want to know more about


- Mongoose
- MongoDB
- SQL

 

