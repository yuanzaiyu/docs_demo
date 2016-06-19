iOS API
===============

Authentication
--------------

RestfulAPI supports only HTTPS. Authentication is performed based on RestfulAPI Key and respective RestfulAPI Secret. Different from SDK's Vendor key/Sign Key, this API Key/Secret are used only for Restful API access.
The Restful API Key/ Secret should pass basic HTTP Authentication. For this, use key as username and secret as password.
You may access the Restful API Key from Dashboard -> Profile -> RestfulAPI

EndPoint
--------

All requests should be sent to https://api.agora.io/dev/v1


Request
-------

Parameters must be sent in JSON, with content type: Content-Type: application/json

Response
--------

Response content is JSON format.
Response status defined as below:

- Status 200: request handle successfully
- Status 401: unauthorized (incorrect API key/ secret pair)
- Status 400: input is in wrong format
- Status 404: wrong API invoking
- Status 500: internal error of Agora RestfulAPI service

APIs
----

Projects
^^^^^^^^

1. Get All Projects
~~~~~~~~~~~~~~~~~~~

Method::
    Get

Path::
    /projects/
Params::
    None

Response::

    {
        projects:[
            {
              id: 'xxxx',
              name: 'project1',
              vendor_key: '4855898a22ae4102a29b81ba76f2eae2',
              sign_key: '4855898a22ae4102a29b81ba76f2eae2',
              recording_server: '10.2.2.8:8080',
              status: 1,
              created: 1464165672
            }
        ]
    }

Status::
    - 1: active
    - 0: disable
