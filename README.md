# spad interview task
<b><var>spad interview task</var></b>

<div>
  <img
      src="/data/task-completed.png"
      alt="spad interview task | task completed"
      style="max-width:100%;"
  />
</div>

# Preview and Codes
<div>
  <img
      src="/data/tree-the-task-codes.png"
      alt="spad interview task | tree the task codes"
      style="max-width:100%;"
  />
</div>

# What is this project
This project is the task of <strong>Spad Company</strong>

# TODOs
We need create and write:

        1) Generate a unque alias for the provided address

        2) The service should redirect users to original URLs when they access a short link 
        
        3) The short link have a lifetime
        
        4) The service should have a visits count 
        
        5) Docker image
        
        6) Use camelCase
        
        7) Clean code

# Does this project have any dependencies
***Yes***

# What technologies did we use
We used these technologies

  1. **Golang** 
  
  2. **Golang libraries**
  
  3. **Redis**
  
  4. **Docker**

# How to create a unique identifier for URL
<div>
We paid attention to these
  
  1. **Length**
  
  2. **Uniqueness**
  
  3. **Search**
</div>

# What settings did we use for this project
We put all the <var>Redis</var> settings in one **Json** file

And you can find all the settings in the ``configuration.json`` file
  
And You can change your settings in the ``configuration.json`` file

# How we worked with storage and Redis
We wrote a <var>Golang</var> code to do our job with **Redis**

And you can find this code in the ``storage.go`` file in the **storage directory**

# How we handled the whole project
We divided the tasks and wrote a *special code* for each task and wanted each section to do its job **efficiently**.

Base:
> base62.go

Config: 
> configuration.go

Handler:
> handler.go

Storage:
> storage.go

Docker:
> Dockerfile

Main:
> main.go

# Why didn't we use Postman
We also had the ability to use <var>Postman</var>, but we didn't want it to get too crowded, so we used **Redis** for fun.

# How to use this project
Get the modules and dependencies

```golang
go mod download
```

Run service

```golang
go run main.go
```

Create a short link 

```shell
curl -L -X POST 'localhost:8080/encode' -H 'Content-Type: application/json' --data-raw '{
    "url": "WRITE-YOUR-URL-IN-HERE",
    "expires": "WRITE-YOUR-EXPIRE-TIME-IN-HERE"
}'
```

we will get a **response** like:
```json
{
   "success": true,
   "shortUrl": "http://localhost:8080/THE-SHORT-URL"
}
```

Any short url can be included in the **THE-SHORT-URL** 

Get detailed **information** for the short link

```shell
curl -L -X GET 'http://localhost:8080/THE-SHORT-URL'
```

Open the browser and follow the **your short link**
```html
http://localhost:8080/THE-SHORT-URL
```

# How to use the Docker
Go to the ***task file*** and we will run in ***terminal command*** to build **Docker image**

```docker
docker build . -t task 
```

Run the **Docker image**

```docker
docker run -p 8080:8080 task
```

# Contact
**gmail**
- samprogram2007@gmail.com

<hr />

# Example
Run **main** file 

<img
      src="/data/example/run-main-file.png"
      alt="spad interview task | task completed | run-main-file"
      style="max-width:100%;"
/>

Run the **Redis Server**

<img
      src="/data/example/run-redis-server.png"
      alt="spad interview task | task completed | run-redis-server"
      style="max-width:100%;"
/>

Create a **short link**

<img
      src="/data/example/create-a-short-link.png"
      alt="spad interview task | task completed | create-a-short-link"
      style="max-width:100%;"
/>

Generated <var>short link</var> in **main** 

<img
      src="/data/example/generated-link-main-file.png"
      alt="spad interview task | task completed | generated-link-main-file"
      style="max-width:100%;"
/>

Get detailed information for the **short link**

<img
      src="/data/example/get-detailed-information-for-the-short-link.png"
      alt="spad interview task | task completed | get-detailed-information-for-the-short-link"
      style="max-width:100%;"
/>

Enter and wait after get **details** 

<img
      src="/data/example/eneter-and-wait-after-get-details.png"
      alt="spad interview task | task completed | eneter-and-wait-after-get-details"
      style="max-width:100%;"
/>

Open the **url** in your Browser 

<img
      src="/data/example/open-the-url.png"
      alt="spad interview task | task completed | open-the-url"
      style="max-width:100%;"
/>

<p>
Yoop !!!
We redirected !!!
</p>

<img
      src="/data/example/we-redirected.png"
      alt="spad interview task | task completed | we-redirected"
      style="max-width:100%;"
/>

# Docker
**First**

<img
      src="/data/docker/docker-one-task.png"
      alt="spad interview task | task completed | docker runed"
      style="max-width:100%;"
/>

**Second**

<img
      src="/data/docker/docker-two-task.png"
      alt="spad interview task | task completed | docker runed"
      style="max-width:100%;"
/>

<hr />


***('Sami Ghasemi)***
