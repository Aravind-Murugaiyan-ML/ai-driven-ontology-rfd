**System Design**
- instead of feeding prompts to external systems for generating ttl, integrate a prompting system(Agents) for generating ttl, this ttl has to be programatically(using Apache Jene) persisted into a Triple store and provide an interface to execute sparql on the Triple Store to extract values from the ontology specific for organization

phase 1:
I going to treat claude as my agent. To claude 