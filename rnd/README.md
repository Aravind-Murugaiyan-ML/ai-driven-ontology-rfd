# Ontology development project for organizational strategy and planning structures

**Project Scope:**

- Developing an ontology for organizational strategy, vision, and planning
- Capturing entities like departments, goals, KPIs, budgets, and their relationships
- Multiple levels: organizational strategy → department plans → implementation

**Technical Approach:**

- Using AI tools (ChatGPT/Claude) to generate ontology definitions
- Output formats: RDF, OWL, or Neo4j
- Planning for iterative development
- Storage in GitHub repository for version control

**Development Strategy:**

- Start with core entities and relationships
- Validate AI-generated output manually
- Add entities incrementally (like budget associations)
- Focus on whether AI tools can generate usable ontologies before worrying about iteration

**Immediate Next Steps:**

- Test whether free AI tools can generate usable ontologies
- Sync up in the evening to review progress and assess capability
- Focus on proof-of-concept before considering iteration challenges

- prompt to ttl - done
- Visulaize this ttl inside visual code in human readable - has to work
- store the ttl to git to showcase how its iteratively imporvising - has to work

- ttl has to be persisted to graph db - not prioritized
- from graph db we have to generate the owl format to transfer over wire to different systems - not prioritized

- without ttl; from the prompt directly generate owl format. - we need to analyse

**System Design**
- instead of feeding prompts to external systems for generating ttl, integrate a prompting system(Agents) for generating ttl, this ttl has to be programatically(using Apache Jene) persisted into a Triple store and provide an interface to execute sparql on the Triple Store to extract values from the ontology specific for organization