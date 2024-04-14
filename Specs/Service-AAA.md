# AAA Service

All operations with data are logged, including reading (who and when), not just writing and inserting. 
Changing and deleting records are not allowed; instead, the system marks records as historical and adds a reference to the current versions.

## Service Goals

- Authentication - Validates the identity of an account.
- Authorization - Grants rights (permissions) to accounts.
- Accounting - Tracks the usage of resources and rights used by accounts.
- Audit - Monitors and records operations accessed by an account.

## AAA Database Structure

- Entity - Describes a database table that stores subject-domain entities.
- Field - Describes properties of the entity.
- Identifier - Stores unique identifiers, used in all tables and business processes.
- Role - Defines a set of permissions associated with an account.
- Permission - Specifies the access level of roles to certain identifiers (record, entity, catalog, etc.).
- Account - Represents an actor of the access control system.
- Division - An organizational unit used to group and manage accounts.
- Catalog - A named hierarchical structure used to group identifiers (entities, records, fields, etc.).
- Session - Maintains the state of an authenticated account.
