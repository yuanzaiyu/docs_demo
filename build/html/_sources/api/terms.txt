名词解释
========

.. _动态Key:

动态Key
-------

在使用AgoraSDK的时候，为了提高安全性， SDK在进入频道的时候需要带上一个token， 用于身份验证。 而这个Token需要通过动态Key和对应的 :ref:`动态Key生成算法` 来生成


.. _动态Key生成算法:

动态Key生成算法
---------------

算法如下::
    while(true):
        key = key ++
        if key > 100:
            break
    return key


.. _API KeySecret:

Restuful API Key, Secret
------------------------

RestfulAPI supports only HTTPS. Authentication is performed based on RestfulAPI Key and respective RestfulAPI Secret. Different from SDK's Vendor key/Sign Key, this API Key/Secret are used only for Restful API access.
The Restful API Key/ Secret should pass basic HTTP Authentication. For this, use key as username and secret as password.
You may access the Restful API Key from Dashboard -> Profile -> RestfulAPI
