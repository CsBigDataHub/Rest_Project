This is my rest Project
##HTTP Methods
-> GET - This  is a read only method . Its is safe to duplicate the GET method
-> POST - this is a write method
-> PUT - this is a write method
-> DELETE - this is a write method

GET, PUT and DELETE are repeatable methods. these methods are Idempotent methods.
POST method cannot be repeated safely. this is non-idempotent methods.

#Uncommon HTTP Methods 
-> Head
-> Options

##HTTP status codes
 200 - success
 201 - created
 204 - No content - typically used for DELETE methods
 302 - found
 304 - Not modified
 307 - Temporary Redirect
 400 - bad request
 401 - Unautherized
 403 - Forbidden
 404 - not found
 415 - Unsupported media type
 500 - internal server error


##Best practises

#PUT vs POST
1. you use PUT to update a message
1. you use POST to create a message

##status codes
1XX Informational codes
2XX success codes
3XX redirection
4XX Client error
5XX server error

-> Hypermedia As The Engine Of Application State(HATEOAS)

# JAX-RS , Jersy and RestEasy are the common library  API.

#To get JSON suppot in the application add the following dependency
 <!-- uncomment this to get JSON support-->
        <dependency>
            <groupId>org.glassfish.jersey.media</groupId>
            <artifactId>jersey-media-json-binding</artifactId>
        </dependency>

