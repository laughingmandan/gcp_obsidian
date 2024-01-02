
Permissions are used to determine which operations are allowed on which resource. They usually corespond 1 to 1 with a REST method. A permission cannot be indiviually assigned to a [[User]]. Instead they must be put into a [[Role]] and the Role must be assigned to that User.

### Naming convention:
##### <service>.<resource>.<verb>
ex. 
-  pubsub.subscriptions.consume
- storage.objects.list