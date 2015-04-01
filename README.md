# chefconf-2015-building-a-private-supermarket-for-your-organization

Doesn't integrate with GitHub Enterprise (would be cool if it did, maybe we could write this).

# Authentication
```
/etc/opscode/chef-server.rb
od_id['administrators'] = 'who'

chef-server-ctl reconfigure
```
TODO Propose SCM interfaces discussion for cookbooks being prefixed with tw- to avoid namespace collisions.

Q and A

Privacy flag in the metadata (set this so you can't upload it to the private supermarket).

Q: isnt oc-id an OAuth2 provider.

A: Couldn't use just OAuth2 Plus the PEM file authentication.

Q: Why upload to both the Chef Server and the Supermarket

A: Basically just because. 

