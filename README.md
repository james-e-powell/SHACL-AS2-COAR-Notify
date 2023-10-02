# SHACL-AS2-COAR-Notify
SHACL shape files for AS2 and COAR-Notify messages

This repository hosts SHACL shape description files for various AS2 and COAR-Notify protocol messages. These shapefiles describe minimum requirements for RDF payloads that  utilize either AS2 or both AS2 and the COAR-Notify protocol. There is a companion service that is linked below, which automatically selects the best match validation shape when a message is posted to its LDN inbox. When the validation service receives an RDF payload, it identifies the action predicates in the message, as well as the context(s), and attempts to match these with statements in the SHACL file that identify the structure to which they correspond, via  ex:ValidationShape predicates. To confirm whether the message had the appropriate structure, the developer can access the Web interface of the validation service, find their message in the inbox, and select the validation icon in the far left column. By validating example messages, developers determine whether the RDF structure of messages sent by their applications are compliant with applicable standards. This is particular useful for applications that may generate a high volume of messages.

### More info about relevant projects: 
- [Activity Streams](https://www.w3.org/TR/activitystreams-core/)
- [COAR-Notify](https://www.coar-repositories.org/notify/)
- [Shapes Constraints Language : SHACL](https://www.w3.org/TR/shacl/)

### Below is a list of shapefiles used by the  [COAR-notify validation service](https://notify-inbox.info/)
| Filename | RDF for Validator |
| --------- | ---------- |
| *acknowledge-and-accept-shape.ttl* | ` ex:ValidationShape rdfs:label "Acknowledge and Accept AS2 COAR-Notify Shape".`|
| *acknowledge-and-reject-shape.ttl* | ` ex:ValidationShape rdfs:label "Acknowledge and Reject AS2 COAR-Notify Shape".` |
| *acknowledge-and-tentative-accept-shape.ttl* | ` ex:ValidationShape rdfs:label "Acknowledge and Tentative Accept AS2 COAR-Notify Shape".` |
| *acknowledge-and-tentative-reject-shape.ttl* | ` ex:ValidationShape - rdfs:label "Acknowledge and Tentative Reject AS2 COAR-Notify Shape".` |
| *announce-endorse-shape.ttl* | ` ex:ValidationShape rdfs:label "Announce-Endorsement AS2 COAR-Notify Shape".`|
| *announce-ingest-shape.ttl* | ` ex:ValidationShape rdfs:label "Announce-Ingest AS2 COAR-Notify Shape".` |
| *announce-relationship-shape.ttl* | `ex:ValidationShape rdfs:label "Announce-Relationship AS2 COAR-Notify Shape".` |
| *announce-review-shape.ttl* | `ex:ValidationShape rdfs:label "Announce-Review AS2 COAR-Notify Shape".` |
| *announce-shape.ttl* | `ex:ValidationShape rdfs:label "Announce AS2 COAR-Notify Shape". `|
| *offer-endorse-shape.ttl*  | `ex:ValidationShape rdfs:label "Offer-Review AS2 COAR-Notify Shape".`|
| *offer-ingest-shape.ttl* | `ex:ValidationShape rdfs:label "Offer-Ingest AS2 COAR-Notify Shape".`|
| *offer-review-shape.ttl* | `ex:ValidationShape rdfs:label "Offer-Review AS2 COAR-Notify Shape".`|
| *undo-shape.ttl* | `ex:ValidationShape rdfs:label "Undo AS2 COAR-Notify Shape".` |

