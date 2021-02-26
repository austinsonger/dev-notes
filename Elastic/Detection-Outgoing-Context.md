# Network Detection Outgoing Context

SUBJECT: Mint - {{context.rule.severity}} - {{context.rule.name}}

Event Occurred at {{#context.alerts}}@timestamp{{/context.alerts}}

# Rule Information

**Link to Alerts:** {{{context.results_link}}}

Detection Name

{{context.rule.name}}

#### Description:

{{context.rule.description}}

#### Reasons for False Positives

{{context.rule.false_positives}}

#### Threat Framework

{{context.rule.threat}}

#### References
- {{context.rule.references}}


# Detection Details

---------------
### User 

{{#context.alerts}}

* user.domain
* user.name
* event.category
* event.outcome


{{/context.alerts}}

---------------
### Destination 

{{#context.alerts}}

* destination.geo.location
* destination.ip
* destination.port
* destination.packets

{{/context.alerts}}

---------------
### Source 

{{#context.alerts}}

- source.geo.location
- source.ip
- source.port
- source.packets

{{/context.alerts}}


---------------
### Network

{{#context.alerts}}

* network.direction
* network.packets
* network.protocol
* network.transport

{{/context.alerts}}


---------------
### DNS

{{#context.alerts}}

* dns.question.name
* dns.question.registered_domain
* dns.question.type
* dns.resolved_ip
* dns.response_code

{{/context.alerts}}

---------------
### Process

{{#context.alerts}}

* process.executable
* process.hash.md5
* process.hash.sha1
* process.hash.sha256
* process.name
* process.parent.executable
* process.parent.name
* process.pid
* process.ppid
* process.title
* process.working_directory
* agent.type
* event.action
* event.category
* event.code
* event.dataset
* event.module
* process.args
* user.id
* user.name

{{/context.alerts}}


-------------
### File

{{#context.alerts}}

* file.name
* file.owner
* file.path
* file.size
* file.target_path

{{/context.alerts}}


---------------
### TLS

{{#context.alerts}}

* tls.server.hash.sha1
* tls.server.issuer
* tls.server.ja3s
* tls.server.not_after
* tls.server.subject

{{/context.alerts}}


---------------
### HTTP Request Fields

{{#context.alerts}}

* http.request.method
* http.response.status_code
* url.domain
* url.path


{{/context.alerts}}



