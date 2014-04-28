Aria Systems Ruby SDK
============

The Aria Systems Ruby SDK supports Aria Systems' Core, Object Query, and AdminTools REST APIs. It is a simple way to integrate your Ruby application with Aria Systems billing solutions.

##Installation

```
gem install aria_sdk
```

##Examples

###REST API

The SDK has three classes for the Aria Systems APIs AriaCoreRestClient, AriaAdmintoolsRestClient, and AriaObjectQueryRestClient. To use one instantiate it with a client no and auth key then use the call method with the method name and parameters.

```ruby
api = AriaCoreRestClient.new(CLIENT_NO, AUTH_KEY)

puts api.call('get_client_currencies')
```

```ruby
api = AriaCoreRestClient.new(CLIENT_NO, AUTH_KEY)

puts api.call('get_plans_by_promo_code', { :promo_code => '63EUEBRFPNRUC5W2NC6RFACTMB5NV' })
```


###SOAP API

##More Information

Check out [Aria Developer Central](http://developer.ariasystems.net) for more examples, details, and support on [Aria](http://www.ariasystems.com/) services and features.

