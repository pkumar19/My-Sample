#%RAML 0.8
title: Email API
baseUri: https://api.covisintlabs.com/broadcast/v1
protocols: [HTTPS]
  
schemas:
  - resourceReferences: |
      {
        "id" : "http://api.covisint.com/schema/resourceReferences",
        "$schema" : "http://json-schema.org/draft-04/schema",
        "description" : "Collection of broadcast templates",
        "type" : "array",
        "items" :  { 
          "$ref": "http://api.covisint.com/schema/resourceReference#"
        }
      }

  - resourceReference: |
       {
         "id" : "http://api.covisint.com/schema/resourceReference",
         "$schema" : "http://json-schema.org/draft-04/schema",
         "description" : "Schema representing links",
         "type" : "object",
         "properties" : {
           "id" : {
             "type" : "string",
             "maxLength" : 36,
             "description" : "The unique identifier for the resource.",
             "required": true
           },
           "type" : {
             "type" : "string",
             "description" : "The type of the resource."
           },
           "realm" : {
             "type" : "string",
             "description" : "The realm of the resource."
           }
         }
       }

  - namedResourceReference : |
       {
         "id" : "http://api.covisint.com/schema/namedScopedResource",
         "$schema" : "http://json-schema.org/draft-04/schema",
         "type" : "object",
         "description" : "Expands on the basic resource reference and adds internationalized name and description.",
         "extends" : {
               "$ref" : "http://api.covisint.com/schema/resourceReference#"
         },
         "properties" : {
            "name" : {  
              "description": "Internationalized resource name.",
              "$ref" : "http://api.covisint.com/idm/schema/internationalString#"
            },
            "description" : {  
              "description": "Internationalized resource description.",
              "$ref" : "http://api.covisint.com/idm/schema/internationalString#"
            }
          }
       }
       
  - resource: |
       {
         "id" : "http://api.covisint.com/schema/resource",
         "$schema" : "http://json-schema.org/draft-04/schema",
         "description" : "Core schema",
         "definitions" : {
           "resource" : {
             "id" : "resource",
             "type" : "object",
             "description" : "A basic resource.",
             "properties" : {
               "id" : {
                 "type" : "string",
                 "maxLength" : 64,
                 "description" : "The unique identifier for this resource.",
                 "required": true
               },
               "version": {
                 "type" : "number",
                 "minimum" : 0,
                 "maximum" : 9223372036854775807,
                 "description" : "The current version for this resource.  Exists once the resource has been saved. This is mandatory for PUT requests, but should not be supplied for POST requests.",
                 "required": false
               },
               "creator" : {
                 "type" : "string",
                 "maxLength" : 64,
                 "description" : "The creator of this resource. This is mandatory if x-requestor header is NOT available",
                 "required": false
               },
               "creatorAppId" : {
                 "type" : "string",
                 "maxLength" : 64,
                 "description" : "The application id of the creator of this resource.",
                 "required": false
               },
               "creation" : {
                 "type" : "number",
                 "minimum" : 0,
                 "maximum" : 9223372036854775807,
                 "description" : "If this value is provided in a POST / PUT request body, it will be ignored and system will generate value as time, in milliseconds since the epoch, when this resource was created or upda",
                 "required": false            
               }
             }
           }
         }
       }
       
  - realmScopedResource : |
       {
         "id" : "http://api.covisint.com/schema/realmScopedResource",
         "$schema" : "http://json-schema.org/draft-04/schema",
         "type" : "object",
         "description" : "Expands on the base resource and adds a realm attribute.",
         "extends" : {
               "$ref" : "http://api.covisint.com/schema/resource#"
         },
         "properties" : {
           "realm" : {
             "type" : "string",
             "maxLength" : 25,
             "pattern" : "^[A-Za-z0-9]{2,25}$",
             "description" : "The realm in which this resource is being created. This is mandatory if x-realm header is NOT available",
             "required": false
           }
         }
       }
       
  - errorResponseSchema: |
       {
         "id" : "http://api.covisint.com/schema/errorResponseSchema",
         "$schema" : "http://json-schema.org/draft-04/schema",
         "type" : "object",
         "description" : "Representation of an HTTP 4xx/5xx error response.",
         "properties" : {
           "status" : { 
             "type" : "number",
             "minimum" : 400,
             "maximum" : 599,
             "description" : "The HTTP status code.",
             "required": true
           },
           "apiMessage" : { 
             "type" : "string",
             "description" : "A helpful, human-readable description of the error, useful for basic diagnostics." 
           },
           "apiStatusCode" : {
             "type" : "string",
             "description" : "The API-specific status code."
           }

         }
       }
  
  - serviceCode: |
       {
         "id" : "http://api.covisint.com/schema/serviceCodes",
         "$schema" : "http://json-schema.org/draft-04/schema",
         "type": "object",
         "description": "The site/service/location codes granted along with a service.",
         "properties": {
           "code": { "type": "string", "required": true, "maxLength": 200, "description": "The code value." },
           "codeKind": { "type": "string", "required": true, "maxLength": 36, "description": "The associated business unit." }
         }
       }     

  - serviceCodes : |
       {
         "type" : "array",
         "description" : "The site/service/location codes granted along with the service, if any.",
         "items" : { "$ref" : "http://api.covisint.com/schema/serviceCode#"},
         "required": false
       }

           

  - internationalString : |
       {
         "id": "http://api.covisint.com/idm/schema/internationalString",
         "$schema": "http://json-schema.org/draft-04/schema",
         "type": "array",
         "description" : "An internationalized string value, supporting one or more language translations.",
         "minItems": 1,
         "items": {
           "type": "object",
           "properties": {
             "lang": { "type": "string", "maxLength": 10, "description": "The language or locale in which the text is written." },
             "text": { "type": "string", "maxLength": 2000, "description": "The internationalized text value." }
           }
         }
       }
  - abstractTaskTargetResource: |
      {
        "id" : "http://api.covisint.com/schema/abstractTaskTargetResource",
        "$schema" : "http://json-schema.org/draft-04/schema",
        "type" : "object",
        "description" : "Expands on the base resource and adds state and error message attributes.",
        "extends" : {
              "$ref" : "http://api.covisint.com/schema/resource#"
        },
        "properties" : {            
          "state" : {
            "description": "The state of the task.",
            "required": true,
            "$ref" : "http://api.covisint.com/schema/resourceReferences#"
          },
          "errorMessage" : {
            "description": "Internationalized description. Language code must be a valid ISO language code.",
            "required": false,
            "$ref" : "http://api.covisint.com/idm/schema/internationalString#"
          }
        }
      }
       
# -------------------------------------------------------------------------------------------------------------------------------- End Common Schema
  - emails: |
      {
        "id" : "http://api.covisint.com/schema/emails",
        "$schema" : "http://json-schema.org/draft-04/schema",
        "description" : "Collection of emais",
        "type" : "array",
        "items" :  { 
          "$ref": "http://api.covisint.com/schema/email#"
        }
      }

  - email: |
      {
        "id" : "http://api.covisint.com/schema/email",
        "$schema" : "http://json-schema.org/draft-04/schema",
        "type" : "object",
        "description" : "Schema representing an email",
        "extends" : {
              "$ref" : "http://api.covisint.com/schema/abstractTaskTargetResource#"
        },
        "properties" : {            
          "message" : {
            "description": "The actual message of the email.",
            "required": true,
            "type":"string",
            "maxLength" : 4000
          },
          "subject" : {
            "description": "The subject of the email.",
            "required": true,
            "type":"string",
            "maxLength" : 255
          },
          "recipientAddress" : {
            "description": "The recipient email address to the email.",
            "required": true,
            "type":"string",
            "maxLength" : 255
          },
          "disclaimer" : {
            "description": "The disclaimer displayed in the email.",
            "required": false,
            "type":"string",
            "maxLength" : 3000
          },
          "fromAddress" : {
            "description": "The from address of the email. If no from address mentioned, the default from address mentioned in the email server will be used.",
            "required": false,
            "type":"string",
            "maxLength" : 255
          },		  
          "processed" : {
            "description": "The instant that the email was processed.",
            "required": false,
            "type" : "number",
            "minimum" : 0,
            "maximum" : 9223372036854775807
          }
        }
      }
 # -------------------------------------------------------------------------------------------------------------------- Start Common Traits
traits:
  - secured:
      usage: Apply this to any method that needs to be secured
      description: Requests requires authentication using a bearer token.
      headers:
        Authorization:
          description: Access token that is obtained from the /token endpoint of the oauth API.
          pattern: ^Bearer .*$
          example: Bearer ZCtYUGpYRXpET0JvVE1rZzlWV3I1Yk
          required: true
      responses:
        401: &401
          description: Unauthenticated request.  This is returned if the access token is missing, invalid, or expired.  Access tokens are obtained through the /token endpoint of the Oauth API.
          body: 
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema
        403: &403
          description: Unauthorized request.  The requestor is not authorized to perform the requested operation.  
          body: 
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema
  - getResponse:
        responses:
          404: &404
            description: |
              The URI requested is invalid or the resource requested does not exist.
              ___
              Substatus codes and error messages are mentioned below:
              + (If a resource id is a URI parameter) framework:resource:missing - A resource with the following ID was not found: {resourceId}
              + No message for an invalid URI
            body: 
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema
                        
          406: &406
            description: |
              Unable to produce content of specified 'Accept' media type
              ___
              Substatus codes and error messages are mentioned below:
              + framework:request:unsupported:mediatype - The server is unable to produce content of type {acceptMediaType}
            body: 
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema
          
          500: &500
            description: |
              An unknown server error occurred
              ___
              Substatus codes and error messages are mentioned below:
              + framework:unknown
            body:      
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema                  
# A GET that is a search of a collection of resources
  - getSearchResponse:
        responses:
          406: *406
          500: *500
  - postResponse:
        responses:
          406: *406
          415: &415
            description: |
              Unable to consume content of specified 'Content-Type' media type
              ___
              Substatus codes and error messages are mentioned below:
              + framework:request:unsupported:mediatype - The server is unable to consume content of type {contentMediaType}
            body:      
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema   
                   
          500: *500
  - deleteResponse:
        responses:
          500: *500
  - putResponse:
        responses:
          404: *404
          406: *406
          409: &409
            description: |
              There is a conflict in identifying the resource being acted on.  There are two categories.  (1) The unique identifier in the URL and in the body are different.  (2) The current version of the resource being updated and the version sent in the body of the request. This may be an indication that the resource has changed since the client loaded it. The conflict should be resolved and the update resubmitted with the current version of the resource.
              + framework:resource:conflict
              + framework:resource:conflict:id - The ID of the resource in the request, {requestedId}, does not match the ID of the given resource, {resourceId}
              + framework:resource:conflict:version - The version of the provided resource, {requestVersion}, does not match the current version of the resource, {latestVersion}
            body:      
              application/vnd.com.covisint.error.v1+json:
                schema: errorResponseSchema   
          415: *415
          500: *500
# A PUT response that will create a resource if it does not exist.
  - putCreateResponse:
        responses:
          406: *406
          409: *409
          415: *415
          500: *500
  - pagableRequest:
      queryParameters:
        page:
          description: Which page to return in the paginated results.  The first page is page 1.
          type: integer
          required: false
          minimum: 1
          default: 1
        pageSize:
          description: How many items per page in the paginated results.  
          type: integer
          required: false
          minimum: 1
          default: 50   
          maximum: 200 


# --------------------------------------------------------------------------------------------------------------- End Common Traits
/email:
  is: [secured]
  description: Collection endpoint for email.
  get:
    is: [getSearchResponse,pagableRequest]
    description: Search emails .[Entitlement:email-search-emails]
    headers:
      Accept:
        description: Media type. 
        example: application/vnd.com.covisint.core.email.v1+json;
        type: string
        required: true
    queryParameters:
      recipientAddress:
        description: Retrieve only Emails with the specified recipient address.
        type: string
        required: true
    responses:
      200:
        description: All emails were successfully retrieved (response collection may be empty).
        body:
          application/vnd.com.covisint.core.email.v1+json:
            schema: email
      400:
        description: |
          There was a problem with the client's request
          ___
          Substatus codes and error messages are mentioned below:
          + framework:request
          + framework:request:io
          + framework:request:io:read - Invalid input. There was an error while parsing.
          + framework:request:io:read:parsing
          + framework:request:io:write
          + framework:request:header:missing - Missing request header: {headerName}
          + framework:request:param:missing - Missing request parameter: {queryParameterName}
          + framework:request:data:missing - The following information was missing from the resource: {resourceFieldName(s)}
          + framework:request:invalid:header:value - Invalid x-requestor header value. Valid values are &#91;person, application&#93;
        body:
          application/vnd.com.covisint.error.v1+json:
            schema: errorResponseSchema
  post:
    is: [postResponse]
    description: Creates a new email.
    headers:
      Accept:
        description: Media type.
        example: application/vnd.com.covisint.core.email.v1+json
        type: string
        required: true
    body:
      application/vnd.com.covisint.core.email.v1+json:
        schema: email 
    responses:
      201:
        description: A new email was created. 
        body:
          application/vnd.com.covisint.core.email.v1+json:
            schema: email
      400:
        description: |
          There was a problem with the client's request
          ___
          Substatus codes and error messages are mentioned below:
          + framework:request
          + framework:request:io
          + framework:request:io:read - Invalid input. There was an error while parsing.
          + framework:request:io:read:parsing
          + framework:request:io:write
          + framework:request:header:missing - Missing request header: {headerName}
          + framework:request:param:missing - Missing request parameter: {queryParameterName}
          + framework:request:data:missing - The following information was missing from the resource: {resourceFieldName(s)}
          + framework:request:data:invalid - The following information should not be part of the resource: {resourceFieldName}
          + framework:resource:data:illegal - The following information was illegal from the resource:  {fieldSpecificError(s)}
          + framework:request:invalid:header:value - Invalid x-requestor header value. Valid values are &#91;person, application&#93;
        body:
          application/vnd.com.covisint.error.v1+json:
            schema: errorResponseSchema
  /{id}:
    description: Endpoint for a email.
    uriParameters:
    is: [secured]      
    get:
      is: [getResponse]
      description: Returns a email by its unique identifier.[Entitlement:email-get-email]
      headers:
        Accept:
          description: Media type.
          example: application/vnd.com.covisint.core.email.v1+json
          type: string
          required: true
      responses:
        200:
          description: The email was successfully retrieved.
          body:
            application/vnd.com.covisint.core.email.v1+json:
              schema: email
        400:
          description: |
            There was a problem with the client's request
            ___
            Substatus codes are mentioned below:
            + framework:request:invalid:header:value - Invalid x-requestor header value. Valid values are &#91;person, application&#93; 
          body:
            application/vnd.com.covisint.error.v1+json:
              schema: errorResponseSchema
