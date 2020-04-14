******
Globus
******

The Globus system ultimately allows researchers to store large amounts of data and share the data with external collaborators. Project NESE offers Globus institutional endpoint setup with flexible administrative tasks delegation to its institutional members and researchers. 

Delegation of roles
-------------------
Role delegation hierarchy consists of institutional NESE coordinators, research groups with shared collections administrators and researchers as the end users of the shared collection directories. 
Delegated roles tasks
A NESE coordinator at a school or a department of a NESE institutional member requests allocation of NESE resources and access to the NESE Globus institutional endpoint with aim to administer creation of Globus shard collections for their respective research groups. 
Research groups sponsored by a NESE institutional members place requests for Globus shared collections to their respective NESE coordinators who in turn create shared endpoints and delegate administrative tasks to their respective shared collection administrators. 
Shared collection administrators create subdirectories of a shared collection, manage Globus users permission access to specific subdirectories and promote Globus users to the administrator role at the shared collection level.
Researchers use their Globus accounts to transfer data between their local endpoints and the directories located in the shared collection.

Delegated Responsibilities
--------------------------
NESE Coordinator
	At university, school or department level
  		- Holds a Globus service account 
  		- Holds a NESE service account with a Unix password
	Creates shared endpoints (shared collections) using the Globus service account
	Assigns administrator roles to Globus users at shared collection level
	Familiar with Globus interface and affairs
	Answers user’s questions

**Shared Collection Administrator**

- Needs a Globus account only
- Submits shared Globus collection request to their NESE coordinator
- When the shared endpoint shows up in their Globus interface
  - Creates subdirectories
  - Manages Globus user’s access controls at subdirectory level
  - Is able to promote Globus users to administrator role at the shared collection level

**Researches, End users**

 - Need a Globus account only
 - Install globus connect on their local machine
 - Manage transfers through a Globus interface
   - Globus web interface
   - Globus command line interface

Globus Endpoint Types
---------------------
To facilitate transfers between the NESE hosted Globus endpoints and your local storage, install and set up a Globus endpoint on your side. Detailed set up instruction is available at http://www.globus.org/globus-connect-personal and http://www.globus.org/globus-connect-server

**NESE hosted Globus endpoint types**

1. Managed endpoint (institutional endpoint)
  - Not used by general Globus audience
  - Hosts shared endpoints (shared collections)
  - Facilitates shared endpoint creation
     - NESE Unix account authentication required

2. Shared endpoint (shared collection)
  - Readable and writable by any authorized Globus user
  - Administered by Globus users having an administrator role assigned
  - Access control administered at subdirectory level

Institutional access to the NESE managed endpoint request
---------------------------------------------------------
A NESE coordinator at a school or a department of a NESE institutional member shall request NESE managed Globus endpoint access and storage allocation with aim to administer creation of Globus shared collections for a specific group or a research project by sending a mail message to help@nese.mghpcc.org wit the following content:

- Username
- Encrypted Password
- Storage Allocation
- Sponsoring Institution
- Department/Group
- Contact Name
- Contact Email

Username is a Unix type of username which will be used during Globus managed endpoint access activation through the Globus user interface. The requested NESE Unix account is a service account intended for and shall be tied to a group/school/department; not to a specific person. Encrypted Password is an authentication string produced by running the following command on any modern unix or linux system::

	openssl passwd -1

when prompted type in a new password and then copy and paste the resulting string into the Encrypted Password field of your message. Storage Allocation is requested storage allocation for all shared collections under this group in usable terabytes subject to adjustment and approval. Project NESE is not responsible for data loss; users are advised to keep a copy of important data offline.

End user access to shared collections request
---------------------------------------------
Researchers sponsored by NESE institutional members shall request a Globus shared collection creation with aim to store and share out large data sets. Please submit a request to the NESE storage allocation coordinator at your school, department or research group with the following content:

- Collection Name
- Globus ID
- Storage Capacity
- Sponsoring Institution

*Collection Name* will be searchable and visible to Globus users through the Globus user interface. *Globus ID* is the Globus user who will be exercising the shared collection administrator role. Please spell out the Globus user identity exactly as displayed in the Account tab in the Globus web interface. *Storage Capacity* is requested storage capacity in terabytes subject to adjustment and approval. Project NESE is not responsible for data loss; users are advised to keep a copy of important data offline.

Globus Quick Start References
----------------------------
Globus web interface: https://docs.globus.org/how-to/get-started/ 
Create Globus Shared Collection: https://docs.globus.org/how-to/share-files/
Globus command line interface (CLI): https://docs.globus.org/cli/
Globus connect set up instruction is available at https://www.globus.org/globus-connect-personal and https://www.globus.org/globus-connect-server 
