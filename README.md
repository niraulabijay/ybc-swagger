#Swagger Url: https://niraulabijay.github.io/ybc-swagger/


# File Upload Endpoints:


###
1. `/v1/file/upload` - this endpoint can receive a `POST` request with multipart-form data and is used to upload a document. 
    #### FORM-DATA: [
      organization_id => "string" <br/>
      directory => "string" <br/>
      attachment => File <br/>
    #### ]

2. `/v1/file/download` - this endpoint can receive a `GET` request with query params `organization_id` and `attachment_path` and is used to download a document. This endpoint returns a response in the form of multipart-form data with the key `attachment` containing the file.
    #### Params: {
      organization_id => "string". <br/>
      attachment_path => File <br/>
    #### }

3. `/v1/file/delete` - this endpoint can receive a `DELETE` request with JSON data containing keys `organization_id` and `attachment_path` which is used to delete a document.
    #### Params: {
      organization_id => "string", <br/>
      attachment_path => File <br/>
    #### }
