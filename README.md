# `ring-hmac-check`

[Ring](http://github.com/mmcgrana/ring) middleware that checks POST requests have a valid HMAC of the HTTP POST body in the header.

In development, not currently working properly!

### Usage

#### With Noir - in server.clj
      (server/add-middleware wrap-hmac-check {:algorithm "HmacSHA512" :header-field "AUTH-HMAC"
                                              :secret-key "FIXME put key here"})
