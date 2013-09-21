!SLIDE

# The Art of Trade-offs

!SLIDE

# The Art of Trade-offs

###### Email: cameron@theflokk.com
###### GitHub: @CamShaft
###### Twitter: @CameronBytheway

!SLIDE

# We are all artists

!SLIDE

# What is art?

From wikipedia:

> General descriptions mention an idea of human agency and creation through imaginative or technical skill.

!SLIDE

Decisions made while transforming this:

![flokk-api](images/flokk-api.png)

!SLIDE

Into this:

![flokk-ui](images/flokk-ui.png)

!SLIDE

# Media type

!SLIDE

# Many json flavors

* [collection+json](http://amundsen.com/media-types/collection/)
* [hal+json](http://stateless.co/hal_specification.html)
* [siren+json](https://github.com/kevinswiber/siren)
* [hyper+json](https://github.com/timshadel/hyper)

!SLIDE

# So which one is the best?

!SLIDE

# The answer is yes.

![silver bullet](images/silver-bullet.jpg)

!SLIDE

# H-Factors can help

![h-factors](images/collection+json.png)

!SLIDE

# Agnostic vs Domain-aware

!SLIDE

![browsers](images/browsers.png)

!SLIDE

[collection-json-explorer](http://collection-json-explorer.herokuapp.com/render?url=http%3A%2F%2Femployee.herokuapp.com%2Femployee#template)

!SLIDE

![flokk-admin](images/flokk-admin.png)

!SLIDE

![multi-resource](images/flokk-multiple-resources.png)

!SLIDE

# Small vs large resources

!SLIDE

Do you have a low-latency network?

![latency](images/latency.png)

!SLIDE

Do your resources naturally cache?

![caching](images/caching.png)

!SLIDE

Do your resources naturally invalidate their cache?

![invalidation](images/natural-invalidation.png)

!SLIDE

# Show/hide affordances based on user

!SLIDE

# Unauthenticated

![unauth](images/item-unauth.png)

!SLIDE

# Authenticated

![auth](images/item-auth.png)

!SLIDE

# Other trade-offs

* Languages
* Databases
* Platforms
* Authentication methods
* MV* client frameworks

!SLIDE

# Real-time

!SLIDE

We use [Pusher](http://pusher.com) for updates to resources

!SLIDE

# Steps

1. Client makes a request to resource owner
2. Client subscribes to resource using the URL as the key
3. Resource owner POSTs notifications to pusher
4. Pusher notifies each client interested in the resource
5. The client re-requests the resource, ignoring any cached values

!SLIDE

[Demo](https://www.theflokk.com)

!SLIDE

# Questions?

###### Email: cameron@theflokk.com
###### GitHub: @CamShaft
###### Twitter: @CameronBytheway
