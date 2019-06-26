# REDISSCACHEAZURE

Azure Cache for Redis is based on the popular software Redis. It is typically used as a cache to improve the performance
and scalability of systems that rely heavily on backend data-stores. Performance is improved by temporarily copying 
frequently accessed data to fast storage located close to the application. With Azure Cache for Redis, 
this fast storage is located in-memory with Azure Cache for Redis instead of being loaded from disk by a database.

Create a cache

1. To create a cache, first sign in to the Azure portal. Then select Create a resource > Databases > Azure Cache for Redis.
2. In New Azure Cache for Redis, configure the settings for your new cache.
Setting	Suggested value	Description
DNS name	Globally unique name	The cache name. It must be a string between 1 and 63 characters and contain only numbers, letters, and the - character. The cache name cannot start or end with the - character, and consecutive - characters are not valid.
Subscription	Your subscription	The subscription under which this new Azure Cache for Redis instance is created.
Resource group	TestResources	Name for the new resource group in which to create your cache. By putting all the resources for an app in a group, you can manage them together. For example, deleting the resource group deletes all resources that are associated with the app.
Location	East US	Choose a region near to other services that will use your cache.
Pricing tier	Basic C0 (250 MB Cache)	The pricing tier determines the size, performance, and features that are available for the cache. For more information, see Azure Cache for Redis Overview.
Pin to dashboard	Selected	Pin the new cache to your dashboard to make it easy to find.


In this way we can simply create cache for Azure.

There are few advance option which we need to remebr.

1.  Azure provide you automatic scalling if exissitng memory exeed 
2.  It Also provide you Persistenet storage to azure file - this will help you to backup everything if you resrtart rediss cache
    for any reason.
3. It also provide Master Sleve switching , when node which has master running get failed, it will switch to Another node and make them as
   master.
 
