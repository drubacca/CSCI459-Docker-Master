#Context

Config is what represents configuration data, usually what will be writable via the northbound agents (CLI, Netconf, Web, etc.), it is also what will be retrieved in a get-config Netconf operation.

Config is the representation of configuration data, this data is usually writable via northbound agents. Examples such as: CLI, Netconf, Web, etc.. Configuraton data is also what is received via a GET-config during a Netconf operation.

#Decision

Config data must be implemented to the project due to it's heavy reliance on the web. The mongo server is responsible for the webpage/database, however, the data must still be able to travel from user to host. 

