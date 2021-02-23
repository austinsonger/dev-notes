## Host fields

These fields must be mapped to display host data in the Elastic Security app:

- `@timestamp`
- `host.name`

These fields can be mapped to display additional host data in the Elastic Security app:

- `cloud.instance.id`
- `cloud.machine.type`
- `cloud.provider`
- `cloud.region`
- `host.architecture`
- `host.id`
- `host.ip`
- `host.mac`
- `host.os.family`
- `host.os.name`
- `host.os.platform`
- `host.os.version`

#### Authentication fields

These fields must be mapped to display host authentication data in the Elastic Security app:

- `event.category`

  To display authentication data in the Elastic Security app, you must map authentication events to the `event.category` field with a value of `authentication`.

- `event.outcome`

This field can be mapped to display additional host authentication data in the Elastic Security app:

- `user.name`

#### Uncommon process fields

This field must be mapped to display host uncommon process data in the Elastic Security app:

- `process.name`

These fields can be mapped to display additional uncommon process data in the Elastic Security app:

- `agent.type`
- `event.action`
- `event.category`
- `event.code`
- `event.dataset`
- `event.module`
- `process.args`
- `user.id`
- `user.name`

## Network fields

These fields must be mapped to display network data in the Elastic Security app:

- `@timestamp`
- `destination.geo.location` (required for displaying
- `destination.ip`
- `source.geo.location` (required for displaying map data)
- `source.ip`

These fields can be mapped to display additional network data in the Elastic Security app:

- `destination.as.number`
- `destination.as.organization.name`
- `destination.bytes`
- `destination.domain`
- `destination.geo.country_iso_code`
- `source.as.number`
- `source.as.organization.name`
- `source.bytes`
- `source.domain`
- `source.geo.country_iso_code`

#### DNS query fields

These fields must be mapped to display DNS data in the Elastic Security app:

- `dns.question.name`
- `dns.question.registered_domain`

This field can be mapped to display additional DNS data in the Elastic Security app:

- `dns.question.type`

  If you want to be able to filter out PTR records, make sure relevant events populate the `dns.question.type` field with a value of `PTR`.

#### HTTP request fields
These fields must be mapped to display HTTP request data in the Elastic Security app:

- `http.request.method`
- `http.response.status_code`
- `url.domain`
- `url.path`

#### TLS fields

This field must be mapped to display TLS data in the Elastic Security app:

- `tls.server.hash.sha1`

These fields can be mapped to display additional TLS data in the Elastic Security app:

- `tls.server.issuer`
- `tls.server.ja3s`
- `tls.server.not_after`
- `tls.server.subject`

## Event and external alert fields

These fields must be mapped to display event and external alert data in the Elastic Security app:

- `@timestamp`

- `event.kind`

  For external alerts, the `event.kind` field value must be `alert`.

These fields can be mapped to display additional event and external alert data in the Elastic Security app:

- `destination.bytes`
- `destination.geo.city_name`
- `destination.geo.continent_name`
- `destination.geo.country_iso_code`
- `destination.geo.country_name`
- `destination.geo.region_iso_code`
- `destination.geo.region_name`
- `destination.ip`
- `destination.packets`
- `destination.port`
- `dns.question.name`
- `dns.question.type`
- `dns.resolved_ip`
- `dns.response_code`
- `event.action`
- `event.category`
- `event.code`
- `event.created`
- `event.dataset`
- `event.duration`
- `event.end`
- `event.hash`
- `event.id`
- `event.module`
- `event.original`
- `event.outcome`
- `event.provider`
- `event.risk_score_norm`
- `event.risk_score`
- `event.severity`
- `event.start`
- `event.timezone`
- `event.type`
- `file.ctime`
- `file.device`
- `file.extension`
- `file.gid`
- `file.group`
- `file.inode`
- `file.mode`
- `file.mtime`
- `file.name`
- `file.owner`
- `file.path`
- `file.size`
- `file.target_path`
- `file.type`
- `file.uid`
- `host.id`
- `host.ip`
- `http.request.body.bytes`
- `http.request.body.content`
- `http.request.method`
- `http.request.referrer`
- `http.response.body.bytes`
- `http.response.body.content`
- `http.response.status_code`
- `http.version`
- `message`
- `network.bytes`
- `network.community_id`
- `network.direction`
- `network.packets`
- `network.protocol`
- `network.transport`
- `pe.original_file_name`
- `process.args`
- `process.executable`
- `process.hash.md5`
- `process.hash.sha1`
- `process.hash.sha256`
- `process.name`
- `process.parent.executable`
- `process.parent.name`
- `process.pid`
- `process.ppid`
- `process.title`
- `process.working_directory`
- `rule.reference`
- `source.bytes`
- `source.geo.city_name`
- `source.geo.continent_name`
- `source.geo.country_iso_code`
- `source.geo.country_name`
- `source.geo.region_iso_code`
- `source.geo.region_name`
- `source.ip`
- `source.packets`
- `source.port`
- `user.domain`
- `user.name`

