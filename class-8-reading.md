# Class 8 reading

## What is Role Based Access Control (RBAC) and why do we care?

RBAC is giving access to certain systems based on the the role of the user. This would compartmentalize the access to a specific area and even minimize the threat across the whole system.

## Describe a Role/Permission heirarchy that you might implement using RBAC

This is pretty much define a specific group of people (who need it) to have full or partial access to said doc. It would be like giving everyone access to the facebook code. There is a certaint level that some people who need to be in order to have full access. Especially when is comes to important documents. The editor of a publishing company does not need access to the billing

## What approach might you take to implement RBAC?

- inventory: Take accound for which systems you need to control access to.
- Analyze Workforce and create roles: Define the roles that require common access, an what role requires limited access.
- Assign people to the roles: Self explanatory.
- Never make "one-off" changes: Change roles as reqiured but dont bend for single employees... this can get out of hand very quickly.
- Audit: Periodically checj to make sure that employees have acceess to what ever they really need access to.

## If Authentication is “you are who you say you are,” what is Authorization?

This is checking to make sure that correct people have access to whatever makes sense.

## Name three primary rules defined for RBAC

- Role assignment: This is where the user is only able to use the permission that they have been assigned to.

- Role authorization: This is  the authorization of the role.

- Permission authorizatio: This is where the user can use a permission only if the permission is authorized for the users "role".

## Describe RBAC to a non-technical friend

This is like giving access only to those who actually need it for their given role. There is no need for the editor of a book company to have access to the payroll.. besides it being a conflict of interest the editor has no reason to have that access. This makes sure everything is compartmentalized.

## What Are access rights Associated with? The User? or The Role? Explain

The access rights are associated with the role. The user is the one who fills the role. This is a no bias approach to making sure that you are having access to what makes sense. This is like a cooling system not needing access to car stereo.

## Access Rights, or Authorization, is activated after a user successfully does what?

When a user authenticates themselves to the system. This puts them into their assigned roles and that would grant access.

## Explain how RBAC might benefit a business

This allows Users to focus on what they need to. The business is able to build a business and allows them to focus on that task whichout spreading them out too thin. This also makes it so there is no need to change things around when a user leaves, the system still stands with no requirement to be updated.