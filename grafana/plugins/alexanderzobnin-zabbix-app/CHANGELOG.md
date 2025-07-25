# Change Log

## 5.2.0

🚀 Add possibility to run "Manual event actions"
🐛 Fix: `real_hosts` deprecated in version 6.2 and 6.4
🐛 Fix: handle multiple service status
⚙️ Chore: Bump grafana-plugin-sdk-go from 0.277.1 to 0.278.0

## 5.1.0

🚀 Problems Panel: Add option to show data source name
🐛 Variables: Fix item tag filtering in Items type
🐛 Fix: frontend error when running count triggers
⚙️ Chore: Bump grafana-plugin-sdk-go from 0.274.0 to 0.277.0

## 5.0.4

🐛 Fix: TLS handshake timeout issues by disabling post-quantum key exchange mechanism in go

## 5.0.3

🐛 Security: Update golang.org/x/net from v0.35.0 to v0.37.0
⚙️ Chore: Build plugin with go 1.24.1
🐛 Fix: Basic authentication in zabbix <7.2
⚙️ Chore: Bump grafana-plugin-sdk-go from 0.270.0 to 0.274.0

## [5.0.2] - 2025-02-27

- Chore: Fix error source for parsing of invalid json response
- Chore: Update github.com/grafana/grafana-plugin-sdk-go to v0.268.0

## [5.0.1] - 2025-02-24

- Bug fix: Fixed host groups not showing in problems panel
- Bug fix: Fixed problems panel broken when selecting triggers
- Chore: Update github.com/grafana/grafana-plugin-sdk-go to v0.266.0
- Chore: Update frontend dependencies
- Chore: Implement error source

## [5.0.0] - 2025-01-10

- Plugin now requires Grafana 10.4.8 or newer

## [4.6.1] - 2025-01-07

- Bug fix: Fixed a compatibility issue with zabbix 7. ( Fixes [#1935](https://github.com/grafana/grafana-zabbix/issues/1935) )

## [4.6.0] - 2024-12-16

- Feature: Added support for Zabbix 7. ( Fixes [#1914](https://github.com/grafana/grafana-zabbix/issues/1914) )
- Feature: Host ID alias function `$__zbx_host_id` ([#1913](https://github.com/grafana/grafana-zabbix/pull/1913))
- Bug Fix: Fixed a bug where mixed datasource with variable ref were not working #1909
- Bug Fix: Fixed a bug where multiple SLA queries not handled correctly #1910
- Chore: Updated grafana plugin SDK

## [4.5.7] - 2024-10-30

- Chore: Bump uplot to 1.6.31
- Chore: Bump grafana-plugin-sdk-go from 0.250.0 to 0.251.0

## [4.5.6] - 2024-10-21

- Fix: AlertList styling issues in grafana 11.0.0
- Chore: Migrate example dashboards from deprecated panels

## [4.5.5] - 2024-09-30

- Chore: Bump dompurify from 3.1.0 to 3.1.6
- Chore: Bump grafana-plugin-sdk-go from 0.250.0 to 0.251.0
- Chore: Bump grafana-plugin-sdk-go from 0.247.0 to 0.250.0

## [4.5.4] - 2024-09-12

- Chore: Bump path-to-regexp from 1.8.0 to 1.9.0
- Chore: Bump grafana-plugin-sdk-go from 0.236.0 to 0.247.0

## [4.5.3] - 2024-09-03

- Chore: Bump fast-loops from 1.1.3 to 1.1.4
- Chore: Bump webpack from 5.88.2 to 5.94.0
- Chore: Bump micromatch from 4.0.5 to 4.0.8
- Docs: Update documentation about Alias functions

## [4.5.2] - 2024-07-01

- Chore: Changes required for nested plugins
- Chore: Updated the executable path

## [4.5.1] - 2024-06-14

- Fix: Problems queries not working before zabbix version 7

## [4.5.0] - 2024-06-10

- Add support for Zabbix version 7

## [4.4.9] - 2024-04-30

- Fix: Improve compatibility with the scenes framework (#1822)
- Chore: Update dependencies

## [4.4.8] - 2024-04-15

- Chore: Update dependencies

## [4.4.7] - 2024-04-08

- Chore: Bump grafana-plugin-sdk-go from `v0.193.0` to `v0.220.0`
- Chore: Update plugin keywords

## [4.4.6] - 2024-03-07

- Fix: API token reset not working (#1797)
- Chore: Build with go 1.22

## [4.4.5] - 2024-01-10

- ⚙️ **Docs**: Documentation website moved from [github pages](https://grafana.github.io/grafana-zabbix) to [grafana.com/docs/plugins](https://grafana.com/docs/plugins/alexanderzobnin-zabbix-app/latest/) page
- Handle changed PostgreSQL plugin id [#1771](https://github.com/grafana/grafana-zabbix/pull/1771)

## [4.4.4] - 2023-11-21

### Feature

- Update configuration page to follow best practices

### Fix

- Dashboards not showing up in configuration

### Chore

- Added lint github workflow
- Update grafana-plugin-sdk-go to latest
- Remove legacy form styling

## [4.4.3] - 2023-10-10

### Chore

- Don't track requests on dashboard [#1707](https://github.com/grafana/grafana-zabbix/pull/1707)

## [4.4.2] - 2023-10-09

### Chore

- Upgrade dependencies [#1692](https://github.com/grafana/grafana-zabbix/pull/1692) [#1702](https://github.com/grafana/grafana-zabbix/pull/1702)
- Added feature tracking [#1688](https://github.com/grafana/grafana-zabbix/pull/1688)

### Docs

- Fix broken link in query editor and doc [#1701](https://github.com/grafana/grafana-zabbix/pull/1701)

## [4.4.1] - 2023-08-30

### Fixed

- Plugin unavailable, [#1604](https://github.com/alexanderzobnin/grafana-zabbix/issues/1604)

## [4.4.0] - 2023-08-17

### Added

- Support for secure socks proxy, [#1653](https://github.com/alexanderzobnin/grafana-zabbix/issues/1653)
- Able to use API tokens for authentication, [#1513](https://github.com/alexanderzobnin/grafana-zabbix/issues/1513)
- Problems: Able to select AND/OR tag evaluation rule, [#1600](https://github.com/alexanderzobnin/grafana-zabbix/issues/1600)

### Fixed

- Application filter does not work in some cases, [#1597](https://github.com/alexanderzobnin/grafana-zabbix/issues/1597)
- Application filter in the triggers query, [#1643](https://github.com/alexanderzobnin/grafana-zabbix/issues/1643)
- Problems: pagination on footer doesn't work [#1649](https://github.com/alexanderzobnin/grafana-zabbix/issues/1649)
- Single host items contain the hostname in the legend, [#1335](https://github.com/alexanderzobnin/grafana-zabbix/issues/1335)
- IT Services: displaying multiple SLA, [#1603](https://github.com/alexanderzobnin/grafana-zabbix/issues/1603)

## [4.3.1] - 2023-03-23

### Fixed

- Cannot create or edit variables (unexpected error happened), [#1590](https://github.com/alexanderzobnin/grafana-zabbix/issues/1590)
- Item tag filter not working properly, [#1594](https://github.com/alexanderzobnin/grafana-zabbix/issues/1594)
- SLA dates differ in Grafana and Zabbix, [#1595](https://github.com/alexanderzobnin/grafana-zabbix/issues/1595)
- Problems panel: invalid problem lastchange time for list layout, [#1596](https://github.com/alexanderzobnin/grafana-zabbix/issues/1596)
- Problems panel: tags filter doesn't work in history mode, [#1592](https://github.com/alexanderzobnin/grafana-zabbix/issues/1592)

## [4.3.0] - 2023-03-21

### Added

- SLA support in Zabbix 6.0, [#1437](https://github.com/alexanderzobnin/grafana-zabbix/issues/1437)
- Build for FreeBSD, [#1301](https://github.com/alexanderzobnin/grafana-zabbix/issues/1301)
- Problems panel: add operational data, [#1260](https://github.com/alexanderzobnin/grafana-zabbix/issues/1260)
- Problems panel: allow HTML in problem description, [#1557](https://github.com/alexanderzobnin/grafana-zabbix/issues/1557)
- Problems panel: show acknowledge author in message, [#1281](https://github.com/alexanderzobnin/grafana-zabbix/issues/1281)
- Problems panel: query problems with particular severity, [#572](https://github.com/alexanderzobnin/grafana-zabbix/issues/572)
- Show non-suppressed problems from maintenance hosts when "Show Maintenance Hosts" is not selected, [#830](https://github.com/alexanderzobnin/grafana-zabbix/issues/830)
- Set data frame name in triggers query mode, [#1441](https://github.com/alexanderzobnin/grafana-zabbix/issues/1441)
- Use trends by graph, [#1442](https://github.com/alexanderzobnin/grafana-zabbix/issues/1442)
- Improved performance of item tags, [#1315](https://github.com/alexanderzobnin/grafana-zabbix/issues/1315)
- Triggers query mode: add time range switcher, [#918](https://github.com/alexanderzobnin/grafana-zabbix/issues/918)

### Fixed

- Zabbix authentication does not work in 6.4, [#1544](https://github.com/alexanderzobnin/grafana-zabbix/issues/1544)
- Error `json: invalid use of ,string struct tag, trying to unmarshal into float64`, [#1325](https://github.com/alexanderzobnin/grafana-zabbix/issues/1325)
- Triggers: acknowledged filter doesn't work, [#985](https://github.com/alexanderzobnin/grafana-zabbix/issues/985)

## [4.2.10] - 2022-09-01

### Fixed

- Perl regex syntax no longer accepted in any filter, [#1264](https://github.com/alexanderzobnin/grafana-zabbix/issues/1264)
- InfluxDB direct DB connection error (`this.influxDS._seriesQuery(...).then is not a function`), [#1255](https://github.com/alexanderzobnin/grafana-zabbix/issues/1255)

## [4.2.9] - 2022-07-12

### Fixed

- Plugin is not working with Zabbix 6.2.0, [#1470](https://github.com/alexanderzobnin/grafana-zabbix/issues/1470)

## [4.2.8] - 2022-05-06

### Fixed

- `setAlias()` doesn't work in some cases, [#1444](https://github.com/alexanderzobnin/grafana-zabbix/issues/1444)
- Trend data displayed incorrectly when direct DB connection enabled, [#1445](https://github.com/alexanderzobnin/grafana-zabbix/issues/1445)

## [4.2.7] - 2022-05-04

### Fixed

- IT Services not working with Zabbix 6.0, [#1408](https://github.com/alexanderzobnin/grafana-zabbix/issues/1408)
- Problems panel: `Cannot read properties of undefined (reading 'trim')` error when tag has only name, [#1420](https://github.com/alexanderzobnin/grafana-zabbix/issues/1420)
- Dashboards not included into plugin, [#1407](https://github.com/alexanderzobnin/grafana-zabbix/issues/1407)
- Missing labels in response, [#1352](https://github.com/alexanderzobnin/grafana-zabbix/issues/1352)
- Query returns all application data when host not found, [#1427](https://github.com/alexanderzobnin/grafana-zabbix/issues/1427)
- Basic Auth is not working (401 Unauthorized), [#1327](https://github.com/alexanderzobnin/grafana-zabbix/issues/1327)
- _Show disabled items_ option is not working, [#1249](https://github.com/alexanderzobnin/grafana-zabbix/issues/1249)

## [4.2.6] - 2022-04-04

### Fixed

- Problems panel: incorrect problem name when PROBLEM event generation mode set to multiple, [#1403](https://github.com/alexanderzobnin/grafana-zabbix/issues/1403)

## [4.2.5] - 2022-02-17

### Fixed

- Problems panel: error when attempting to click on info button, [#1357](https://github.com/alexanderzobnin/grafana-zabbix/issues/1357)
- Error parsing regexp: invalid or unsupported Perl syntax, [#1318](https://github.com/alexanderzobnin/grafana-zabbix/issues/1318)
- json: cannot unmarshal number into Go struct field TimeSeriesData.series.TS of type int64, [#1320](https://github.com/alexanderzobnin/grafana-zabbix/issues/1320)
- json: cannot unmarshal number into Go struct field QueryModel.queryType of type string, [#1342](https://github.com/alexanderzobnin/grafana-zabbix/issues/1342)
- Grafana does not get units from Zabbix in 4.2, [#1321](https://github.com/alexanderzobnin/grafana-zabbix/issues/1321)

## [4.2.4] - 2021-09-27

### Fixed

- Time series is cut on certain conditions, [#1309](https://github.com/alexanderzobnin/grafana-zabbix/issues/1309)
- groupBy/aggregateBy handles interval improperly, [#1310](https://github.com/alexanderzobnin/grafana-zabbix/issues/1310)
- `top()` function returns incorrect set of series, [#1313](https://github.com/alexanderzobnin/grafana-zabbix/issues/1313)
- Some data alignment/stacking issues

## [4.2.3] - 2021-09-21

### Fixed

- Different collection intervals compatibility (stacked graph issue), [#1211](https://github.com/alexanderzobnin/grafana-zabbix/issues/1211)
- Graph broken when trend data used, [#1300](https://github.com/alexanderzobnin/grafana-zabbix/issues/1300)
- Zabbix API request error "EOF", [#1295](https://github.com/alexanderzobnin/grafana-zabbix/issues/1295)
- Item tag does not accept variables, [#1283](https://github.com/alexanderzobnin/grafana-zabbix/issues/1283)
- Failed to query data, rpc error, [#1262](https://github.com/alexanderzobnin/grafana-zabbix/issues/1262)
- Error `Cannot read property 'isZabbix54OrHigher' of undefined` when creating a variable template query, [#1282](https://github.com/alexanderzobnin/grafana-zabbix/issues/1282)

## [4.2.2] - 2021-08-25

### Fixed

- Different item intervals compatibility (stacked graph issue), [#1211](https://github.com/alexanderzobnin/grafana-zabbix/issues/1211)
- Random "Failed to call resource" errors and plugin restarts, [#1269](https://github.com/alexanderzobnin/grafana-zabbix/issues/1269)
- Top function does not work if number of series less than provided N, [#1267](https://github.com/alexanderzobnin/grafana-zabbix/issues/1267)
- Host names are not displayed on multiple selection (regular expression), [#1265](https://github.com/alexanderzobnin/grafana-zabbix/issues/1265)
- Cannot unmarshal number into Go struct field ZabbixDatasourceSettingsDTO.timeout of type string, [#1254](https://github.com/alexanderzobnin/grafana-zabbix/issues/1254)
- `sortSeries()` does not sort by series name, [#1274](https://github.com/alexanderzobnin/grafana-zabbix/issues/1274)

## [4.2.1] - 2021-08-10

### Fixed

- No data on queries with aggregation function
- Wrong percentile aggregation

## [4.2.0] - 2021-08-10

### Added

- Support functions on the backend (alerting with functions), [#869](https://github.com/alexanderzobnin/grafana-zabbix/issues/869)
- Support item tags instead of application in Zabbix 5.4, [#1258](https://github.com/alexanderzobnin/grafana-zabbix/issues/1258)

### Fixed

- Direct DB connection - No data in Grafana 8.0, [#1221](https://github.com/alexanderzobnin/grafana-zabbix/issues/1221)
- Error when attempting to acknowledge problems in Grafana 8.0, [#1239](https://github.com/alexanderzobnin/grafana-zabbix/issues/1239)
- Explore button in Problems view doesn't work (redirects to 404), [#1240](https://github.com/alexanderzobnin/grafana-zabbix/issues/1240)
- Zabbix value mapping doesn't work in Grafana 8.0, [#1222](https://github.com/alexanderzobnin/grafana-zabbix/issues/1222)
- Unable to see acknowledges if problem has tags, [#1233](https://github.com/alexanderzobnin/grafana-zabbix/issues/1233)
- Ack button is not visible on narrow layouts, [#1252](https://github.com/alexanderzobnin/grafana-zabbix/issues/1252)

## [4.1.5] - 2021-05-18

### Fixed

- Fix compatibility with Zabbix 5.4, [#1188](https://github.com/alexanderzobnin/grafana-zabbix/issues/1188)

## [4.1.4] - 2021-03-09

### Fixed

- `Field/Standard options/Display name` stopped working in 4.1 release, [#1130](https://github.com/alexanderzobnin/grafana-zabbix/issues/1130)
- Functions: trendsValue(sum) is not working, [#935](https://github.com/alexanderzobnin/grafana-zabbix/issues/935)

## [4.1.3] - 2021-03-05

### Fixed

- Explore: Error "Unexpected field length", [#1150](https://github.com/alexanderzobnin/grafana-zabbix/issues/1150)
- Problems: item last value truncated text, [#1145](https://github.com/alexanderzobnin/grafana-zabbix/issues/1145)
- Problems: minor UI bug, [#1149](https://github.com/alexanderzobnin/grafana-zabbix/issues/1149)
- Option to disable zabbix value mapping translation in query, [#1128](https://github.com/alexanderzobnin/grafana-zabbix/issues/1128)

## [4.1.2] - 2021-01-28

### Fixed

- Item ID query mode doesn't work, [#1148](https://github.com/alexanderzobnin/grafana-zabbix/issues/1148)
- IT Services: a.round_interval is not a function, [#1142](https://github.com/alexanderzobnin/grafana-zabbix/issues/1142)
- Problems: Text overlap between the tooltip and description boxes, [#1138](https://github.com/alexanderzobnin/grafana-zabbix/issues/1138)
- Problems: expanded row overwritten on refresh, [#1143](https://github.com/alexanderzobnin/grafana-zabbix/issues/1143)

## [4.1.1] - 2020-12-30

### Fixed

- Graphs with dependent items failed to render, [#1123](https://github.com/alexanderzobnin/grafana-zabbix/issues/1123)

## [4.1.0] - 2020-12-28

### Added

- [Data Frames](https://grafana.com/docs/grafana/latest/developers/plugins/data-frames/)
  support, [#10820](https://github.com/alexanderzobnin/grafana-zabbix/issues/10820). This solves various issues below:
- Use units configured in Zabbix if possible
- Use value mappings from Zabbix
- Align points in each series to prevent stacking graph issues
- Fill missing points with null values, [#1109](https://github.com/alexanderzobnin/grafana-zabbix/issues/1109)
- Problems: filter problems by time range, [#1094](https://github.com/alexanderzobnin/grafana-zabbix/issues/1094)
- ARM build (ARM64 and ARM v6), [#1028](https://github.com/alexanderzobnin/grafana-zabbix/issues/1028)

### Fixed

- Grafana doesn't prevent from saving alerts with template variables, [#1100](https://github.com/alexanderzobnin/grafana-zabbix/issues/1100)
- Query inspector is not working, [#1097](https://github.com/alexanderzobnin/grafana-zabbix/issues/1097)
- Problems panel query editor issues, [#988](https://github.com/alexanderzobnin/grafana-zabbix/issues/988)
- Problems: unable to change severity to Not Classified, [#1104](https://github.com/alexanderzobnin/grafana-zabbix/issues/1104)
- Problems: ack message limited to 64 characters, [#1122](https://github.com/alexanderzobnin/grafana-zabbix/issues/1122)

## [4.0.2] - 2020-11-13

### Fixed

- Query mode Text returns no data for last value, [#1062](https://github.com/alexanderzobnin/grafana-zabbix/issues/1062)
- Able to configure API request timeout, [#1046](https://github.com/alexanderzobnin/grafana-zabbix/issues/1046)
- Support basic auth for backend requests, [#1048](https://github.com/alexanderzobnin/grafana-zabbix/issues/1048)
- Problems: fix empty problems list when null value used as a filter
- Problems: fix long item values displaying

## [4.0.1] - 2020-09-02

### Fixed

- Plugin is not signed, [#1038](https://github.com/alexanderzobnin/grafana-zabbix/issues/1038)
- Datasource: "Parse error Invalid JSON. An error occurred on the server while parsing the JSON text"
  , [#1004](https://github.com/alexanderzobnin/grafana-zabbix/issues/1004)
- Datasource: Skip TLS Verify button does not work, [#1029](https://github.com/alexanderzobnin/grafana-zabbix/issues/1029)
- Config: can't select Direct DB Connection in Grafana 7.1.5, [#1027](https://github.com/alexanderzobnin/grafana-zabbix/issues/1027)
- Problems: trigger dependencies not resolved, [#1024](https://github.com/alexanderzobnin/grafana-zabbix/issues/1024)

## [4.0.0] - 2020-08-25

### 4.0 Feature highlights

Grafana-Zabbix 4.0 comes with a bunch of changes under the hood. The most important thing introduced is a backend, which brings a number of benefits:

- Alerting support (limited, data processing functions are not supported yet).
- Fixed security issues related to exposing data source credentials to the Grafana frontend and storing password as a plain text in database.
- Improved performance (plugin can cache queries and process data on the backend).
- With improved security it makes easier to add actions (execute scripts, close problems, etc).

### Installation

**Prerequisites**: plugin requires Grafana 7.0 to run.

Use the grafana-cli tool to install Zabbix from the command-line:

1. `grafana-cli plugins install alexanderzobnin-zabbix-app`
1. Unsigned plugins are not loading by default, so allow it in the Grafana config file:
   ```sh
   allow_loading_unsigned_plugins = alexanderzobnin-zabbix-datasource
   ```
1. restart Grafana server

Refer to [`allow_loading_unsigned_plugins`](https://grafana.com/docs/grafana/latest/installation/configuration/#allow-loading-unsigned-plugins)
option description for more information.

### Security

- Zabbix credentials available for everyone who can see dashboard, [#380](https://github.com/alexanderzobnin/grafana-zabbix/issues/380)
- Store password encrypted, [#800](https://github.com/alexanderzobnin/grafana-zabbix/issues/800)

### Added

- Alerting support (limited, data processing functions are not supported yet)
  , [#801](https://github.com/alexanderzobnin/grafana-zabbix/issues/801)
- Problems: execute scripts, [#978](https://github.com/alexanderzobnin/grafana-zabbix/issues/978)
- Problems: tooltip with problem description
- Problems: use severity filter from panel options

### Fixed

- Problems: problems history
- Problems: sorting by severity, [#921](https://github.com/alexanderzobnin/grafana-zabbix/issues/921)
- Datasource: reconnecting on request error
- Problems: filtering by tags
- Problems: sorting order
- Problems: performance improvements (remove unnecessary queries)
- Problems: empty problem list, [#955](https://github.com/alexanderzobnin/grafana-zabbix/issues/955)
- Problems: panel migrations when panel options is not opened (options not saved after reload)
- Problems: item value tooltip placement

### Removed

- Old alerting feature (show heart icon on the panel), replaced by Grafana alerting

## [4.0.0-alpha4] - 2020-07-21

### Fixed

- Problems: filtering by tags
- Problems: sorting order
- Problems: performance improvements (remove unnecessary queries)

## [4.0.0-alpha3] - 2020-07-17

### Fixed

- Problems: empty problem list, [#955](https://github.com/alexanderzobnin/grafana-zabbix/issues/955)

## [4.0.0-alpha2] - 2020-06-18

### Fixed

- Problems: panel migrations when panel options is not opened (options not saved after reload)
- Problems: item value tooltip placement

### Added

- Problems: use severity filter from panel options

### Removed

- Old alerting feature (show heart icon on the panel), replaced by Grafana alerting

## [4.0.0-alpha1] - 2020-06-04

### 4.0 Feature highlights

Grafana-Zabbix 4.0 comes with a bunch of changes under the hood. The most important thing introduced is a backend, which brings a number of benefits:

- Alerting support (limited, data processing functions are not supported yet).
- Fixed security issues related to exposing data source credentials to the Grafana frontend and storing password as a plain text in database.
- Improved performance (plugin can cache queries and process data on the backend).
- With improved security it makes easier to add actions (execute scripts, close problems, etc).

### Installation

**Prerequisites**: plugin requires Grafana 7.0 to run.

Version 4.0 is currently in alpha state and not published at grafana.com. In order to install it, follow these steps:

1. Go to the [GitHub releases](https://github.com/alexanderzobnin/grafana-zabbix/releases) and find latest `4.0.0`
   release.
1. Download `.zip` package with plugin from release assets (asset name is `grafana-zabbix-4.0.0-<alphaX|betaX>.zip`).
1. Unpack it and put into grafana plugins folder.
1. Unsigned plugins are not loading by default, so allow it in config:
   ```sh
   allow_loading_unsigned_plugins = alexanderzobnin-zabbix-datasource
   ```
1. restart Grafana server

Refer to [`allow_loading_unsigned_plugins`](https://grafana.com/docs/grafana/latest/installation/configuration/#allow-loading-unsigned-plugins)
option description for more information.

### Security

- Zabbix credentials available for everyone who can see dashboard, [#380](https://github.com/alexanderzobnin/grafana-zabbix/issues/380)
- Store password encrypted, [#800](https://github.com/alexanderzobnin/grafana-zabbix/issues/800)

### Added

- Alerting support (limited, data processing functions are not supported yet)
  , [#801](https://github.com/alexanderzobnin/grafana-zabbix/issues/801)
- Problems: execute scripts, [#978](https://github.com/alexanderzobnin/grafana-zabbix/issues/978)

## [3.12.2] - 2020-05-28

### Fixed

- Annotations feature doesn't work, [#964](https://github.com/alexanderzobnin/grafana-zabbix/issues/964)
- Alias variables do not work with direct DB connection enabled, [#965](https://github.com/alexanderzobnin/grafana-zabbix/issues/965)

## [3.12.1] - 2020-05-25

### Fixed

- Problems: panel fails with error (cannot read property 'description' of undefined)
  , [#954](https://github.com/alexanderzobnin/grafana-zabbix/issues/954)
- Problems: problem name filter doesn't work, [#962](https://github.com/alexanderzobnin/grafana-zabbix/issues/962)
- Problems: acknowledged filter doesn't work, [#961](https://github.com/alexanderzobnin/grafana-zabbix/issues/961)

## [3.12.0] - 2020-05-21

### Added

- Variables: able to query item values, [#417](https://github.com/alexanderzobnin/grafana-zabbix/issues/417)
- Functions: expose host, item, app to the alias functions, [#619](https://github.com/alexanderzobnin/grafana-zabbix/issues/619)
- Problems: navigate to Explore and show graphs for the problem, [#948](https://github.com/alexanderzobnin/grafana-zabbix/issues/948)
- Problems: able to show Problems/Recent problems/History, [#495](https://github.com/alexanderzobnin/grafana-zabbix/issues/495)
- Problems: icon with acknowledges count, [#946](https://github.com/alexanderzobnin/grafana-zabbix/issues/946)
- IT Services: support SLA intervals, [#885](https://github.com/alexanderzobnin/grafana-zabbix/issues/885)

### Fixed

- Explore doesn't work with Zabbix datasource, [#888](https://github.com/alexanderzobnin/grafana-zabbix/issues/888)
- SLA value is incorrect, [#885](https://github.com/alexanderzobnin/grafana-zabbix/issues/885)
- Graph panel randomly shows no data, [#861](https://github.com/alexanderzobnin/grafana-zabbix/issues/861)
- Variables: unable to edit variables in Grafana 7.0.0, [#949](https://github.com/alexanderzobnin/grafana-zabbix/issues/949)
- Variables: wrong variable scope inside repeated rows, [#912](https://github.com/alexanderzobnin/grafana-zabbix/issues/912)
- Problems: resolve macros in URLs, [#190](https://github.com/alexanderzobnin/grafana-zabbix/issues/190)
- Problems: unable to acknowledge resolved problem, [#942](https://github.com/alexanderzobnin/grafana-zabbix/issues/942)
- Problems: resolved problems color and severity set to Not classified, [#909](https://github.com/alexanderzobnin/grafana-zabbix/issues/909)
- Problems: can't acknowledge alert in panel with a single problem, [#900](https://github.com/alexanderzobnin/grafana-zabbix/issues/900)
- Annotations: `ITEM.VALUE` behaves like `ITEM.LASTVALUE` in annotations, [#891](https://github.com/alexanderzobnin/grafana-zabbix/issues/891)
- Alert state on the panel (heart icon) doesn't work in Grafana 6.7, [#931](https://github.com/alexanderzobnin/grafana-zabbix/issues/931)
- Consolidated average is not accurate with direct DB connection, [#752](https://github.com/alexanderzobnin/grafana-zabbix/issues/752)

### Changed

- Problems panel uses new `problem.get` API which is not compatible with Zabbix 3.x, [#495](https://github.com/alexanderzobnin/grafana-zabbix/issues/495)
- Problems panel is metrics panel now, problems query editor moved to the data source.
- Zabbix version is auto detected now, [#727](https://github.com/alexanderzobnin/grafana-zabbix/issues/727)

## [3.11.0] - 2020-03-23

### Added

- Improve variable query editor, [#705](https://github.com/alexanderzobnin/grafana-zabbix/issues/705)
- Transform/percentile function, [#868](https://github.com/alexanderzobnin/grafana-zabbix/issues/868)

### Fixed

- Problems panel: stopped working in Grafana 6.7.0, [#907](https://github.com/alexanderzobnin/grafana-zabbix/issues/907)
- Problems panel: event severity change, [#870](https://github.com/alexanderzobnin/grafana-zabbix/issues/870)
- Problems panel: color is changed to acknowledged even if there is only message without acknowledgment, [#857](https://github.com/alexanderzobnin/grafana-zabbix/issues/857)
- Percentile function returns incorrect results, [#862](https://github.com/alexanderzobnin/grafana-zabbix/issues/862)

## [3.10.5] - 2019-12-26

### Added

- SLA over time graphs, [#728](https://github.com/alexanderzobnin/grafana-zabbix/issues/728)
- Additional time ranges in functions, [#531](https://github.com/alexanderzobnin/grafana-zabbix/issues/531)

### Fixed

- Problems panel: query editor broken in Grafana 6.4, [#817](https://github.com/alexanderzobnin/grafana-zabbix/issues/817)
- Datasource: function editor is not working, [#810](https://github.com/alexanderzobnin/grafana-zabbix/issues/810)
- Datasource: cannot add a function to query from typeahead, [#468](https://github.com/alexanderzobnin/grafana-zabbix/issues/468)
- Datasource: annotations editor broken in Grafana 6.x, [#813](https://github.com/alexanderzobnin/grafana-zabbix/issues/813)
- React plugins issue, [#823](https://github.com/alexanderzobnin/grafana-zabbix/issues/823)

## [3.10.4] - 2019-08-08

### Fixed

- Problems panel: query editor broken in Grafana 6.3, [#778](https://github.com/alexanderzobnin/grafana-zabbix/issues/778)
- Problems panel: some heart icons are missing, [#754](https://github.com/alexanderzobnin/grafana-zabbix/issues/754)

## [3.10.3] - 2019-07-26

### Fixed

- Direct DB Connection: can't stay enabled, [#731](https://github.com/alexanderzobnin/grafana-zabbix/issues/731)
- Triggers query mode: count doesn't work with Singlestat, [#726](https://github.com/alexanderzobnin/grafana-zabbix/issues/726)
- Query editor: function editor looks odd in Grafana 6.x, [#765](https://github.com/alexanderzobnin/grafana-zabbix/issues/765)
- Alerting: heart icon on panels in Grafana 6.x, [#715](https://github.com/alexanderzobnin/grafana-zabbix/issues/715)

## [3.10.2] - 2019-04-23

### Fixed

- Direct DB Connection: provisioned datasource fails to load, [#711](https://github.com/alexanderzobnin/grafana-zabbix/issues/711)
- Functions: `sumSeries` doesn't work in couple with other aggregation functions, [#530](https://github.com/alexanderzobnin/grafana-zabbix/issues/530)
- Problems panel: performance and memory issues, [#720](https://github.com/alexanderzobnin/grafana-zabbix/issues/720)
  , [#712](https://github.com/alexanderzobnin/grafana-zabbix/issues/712)
- Problems panel: hide acknowledge button for read-only users, [#722](https://github.com/alexanderzobnin/grafana-zabbix/issues/722)
- Problems panel: "no data" overlaps table header when font size increased, [#717](https://github.com/alexanderzobnin/grafana-zabbix/issues/717)
- Problems panel: problem description does not resize problem bar, [#704](https://github.com/alexanderzobnin/grafana-zabbix/issues/704)
- Triggers query mode: problems not filtered by selected groups, [#709](https://github.com/alexanderzobnin/grafana-zabbix/issues/709)

## [3.10.1] - 2019-03-05

### Fixed

- Problems panel: unable to edit panel in Grafana 6.0, [#685](https://github.com/alexanderzobnin/grafana-zabbix/issues/685)
- Problems panel: datasource selector is empty, [#692](https://github.com/alexanderzobnin/grafana-zabbix/issues/692)
- Problems panel: "acknowledged" filter doesn't work
  correctly, [#678](https://github.com/alexanderzobnin/grafana-zabbix/issues/678) [#691](https://github.com/alexanderzobnin/grafana-zabbix/issues/691)
- Problems panel: acknowledged color isn't working, [#676](https://github.com/alexanderzobnin/grafana-zabbix/issues/676)
- Problems panel: highlight background doesn't work correctly for resolved events in List view, [#681](https://github.com/alexanderzobnin/grafana-zabbix/issues/681)
- Problems panel: duplicated page size entries, [#696](https://github.com/alexanderzobnin/grafana-zabbix/issues/696)
- Direct DB Connection: unable to get trends data from InfluxDB, [#675](https://github.com/alexanderzobnin/grafana-zabbix/issues/675)
- Annotations are not displayed when time set to a full day/week/month, [#680](https://github.com/alexanderzobnin/grafana-zabbix/issues/680)
- Datasource provisioning with direct DB connection enabled failed [#688](https://github.com/alexanderzobnin/grafana-zabbix/issues/688)
- Functions: `offset` function returns `NaN` in singlestat panel, [#683](https://github.com/alexanderzobnin/grafana-zabbix/issues/683)
- Functions: `median()` doesn't correspond to `aggregateBy(median)`
  , [#690](https://github.com/alexanderzobnin/grafana-zabbix/issues/690)
- Docs: add warnings about installation methods, [#693](https://github.com/alexanderzobnin/grafana-zabbix/issues/693)

## [3.10.0] - 2019-02-14

### Added

- Table-like layout for Problems (former Triggers)
  panel, [#673](https://github.com/alexanderzobnin/grafana-zabbix/issues/673)
- Problems panel: able to show last problems from dashboard time range, [#550](https://github.com/alexanderzobnin/grafana-zabbix/issues/550)
- Problems panel: filter problems by event tags, [#487](https://github.com/alexanderzobnin/grafana-zabbix/issues/487)
- Problems panel: option for displaying groups and proxy, [#418](https://github.com/alexanderzobnin/grafana-zabbix/issues/418)
- Support InfluxDB as Direct DB Connection datasource, [#640](https://github.com/alexanderzobnin/grafana-zabbix/issues/640), collaboration with [Gleb Ivanovsky aka @i-ky](https://github.com/i-ky)
- Support datasource provisioning with direct DB connection enabled, [#614](https://github.com/alexanderzobnin/grafana-zabbix/issues/614)
- Functions: `offset` function, [#387](https://github.com/alexanderzobnin/grafana-zabbix/issues/387), thanks to [@drakosha](https://github.com/drakosha)
- Functions: `removeAboveValue`, `removeBelowValue`, `transformNull`
  functions, [#562](https://github.com/alexanderzobnin/grafana-zabbix/issues/562), thanks to [@gelonsoft](https://github.com/gelonsoft)

### Fixed

- _t.replace is not a function_ error when adding new metric, [#661](https://github.com/alexanderzobnin/grafana-zabbix/issues/661)
- Problems panel: error when acknowledging problems in Zabbix 4.0, [#629](https://github.com/alexanderzobnin/grafana-zabbix/issues/629)
- Problems panel: direct link rendered image, [#605](https://github.com/alexanderzobnin/grafana-zabbix/issues/605)
- Direct DB Connection: _Cannot read property 'name' of null_ error when no series returned, [#571](https://github.com/alexanderzobnin/grafana-zabbix/issues/571)
- Direct DB Connection: `consolidateBy(sum)` does not work correctly, [#603](https://github.com/alexanderzobnin/grafana-zabbix/issues/603)
- Direct DB Connection: `consolidateBy()` affects other metrics in a panel, [#602](https://github.com/alexanderzobnin/grafana-zabbix/issues/602)

### Changed

- Disable auto-creation of Zabbix/Linux Server dashboards (still can be imported from datasource config page)
  , [#422](https://github.com/alexanderzobnin/grafana-zabbix/issues/422)
- Use Webpack for building plugin, [#632](https://github.com/alexanderzobnin/grafana-zabbix/issues/632)
- `dist/` folder removed from repo, installation from github repo doesn't work anymore, [#693](https://github.com/alexanderzobnin/grafana-zabbix/issues/693)

## [3.9.1] - 2018-05-02

### Fixed

- Datasource fails when "Direct DB connection"
  enabled [#564](https://github.com/alexanderzobnin/grafana-zabbix/issues/564)
- Alerting and health icons on panels [#556](https://github.com/alexanderzobnin/grafana-zabbix/issues/556)
- Alerting threshold error [#549](https://github.com/alexanderzobnin/grafana-zabbix/issues/549)

## [3.9.0] - 2018-03-23

### Added

- Table format support for text data [#492](https://github.com/alexanderzobnin/grafana-zabbix/issues/492)
- Option to enable triggers background highlighting [#532](https://github.com/alexanderzobnin/grafana-zabbix/issues/532)
- Option to disable acknowledges for read-only users [#481](https://github.com/alexanderzobnin/grafana-zabbix/issues/481)

### Fixed

- Triggers panel has broken styles in Grafana 5.0 [#522](https://github.com/alexanderzobnin/grafana-zabbix/issues/522)
- Undefined username in acknowledges [#393](https://github.com/alexanderzobnin/grafana-zabbix/issues/393)

## [3.8.1] - 2017-12-21

### Fixed

- Triggers panel multiple targets bug (typing in one target affects other)
- Triggers panel event source icon

## [3.8.0] - 2017-12-20

### Added

- Multiple data sources support for triggers panel, [#431](https://github.com/alexanderzobnin/grafana-zabbix/issues/431)

### Changed

- Triggers Panel fully redesigned, closed a bunch of issues: #431, #488, #299, #485, #412, #157, #483, #487, #248
- Tests migrated to [Jest](http://facebook.github.io/jest/)

### Fixed

- Triggers panel refreshing issues
- aggregateBy() function bug, [#498](https://github.com/alexanderzobnin/grafana-zabbix/issues/498)

## [3.7.0] - 2017-10-24

### Added

- PostgreSQL support for Direct DB Connection.
- _Triggers_ query mode which allows to count active alerts by group, host and application, [#141](https://github.com/alexanderzobnin/grafana-zabbix/issues/141)
- `sortSeries()` function that allows to sort multiple timeseries by name, [#447](https://github.com/alexanderzobnin/grafana-zabbix/issues/447), thanks to [@mdorenkamp](https://github.com/mdorenkamp)
- `percentile()` function, thanks to [@pedrohrf](https://github.com/pedrohrf)
- _Zabbix System Status_ example dashboard.

### Changed

- Included dashboards moved to data source. Go to the data source config to import it.

### Fixed

- Direct DB connection doesn't work with `ONLY_FULL_GROUP_BY` option enabled, [#445](https://github.com/alexanderzobnin/grafana-zabbix/issues/445)
- Application selection doesn't work, [#352](https://github.com/alexanderzobnin/grafana-zabbix/issues/352)
- "data points outside time range" error when there is no datapoints and aggregation function is used
- Missed Max data points option in Grafana 4.5+
- Missed query editor help in Grafana 4.5+
- Alert threshold detection with `<=` `>=` `=` operators, thanks to [@akotynski](https://github.com/akotynski).

## [3.6.1] - 2017-07-26

### Fixed

- _cannot read property 'enable' of undefined_ error after upgrade, [#436](https://github.com/alexanderzobnin/grafana-zabbix/issues/436)

## [3.6.0] - 2017-07-26

### Added

- Direct DB Connection, which allows to use existing SQL data source for querying history data directly from Zabbix database.
- **Docs**: Direct DB Connection reference and configuration.
- `consolidateBy` function, which allows to specify aggregation function for time series data.
- `movingAverage` and `exponentialMovingAverage` functions.
- _Item ID_ editor mode for querying items by id.

### Changed

- IT Services query editor. Now user able to select multiple services by using regex, [#415](https://github.com/alexanderzobnin/grafana-zabbix/issues/415)

### Fixed

- Template variables support in annotations and triggers panel (trigger name field)
  , [#428](https://github.com/alexanderzobnin/grafana-zabbix/issues/428)
- Parsing of template variable query with braces, [#432](https://github.com/alexanderzobnin/grafana-zabbix/issues/432)
- `sumSeries()` function bug, [#286](https://github.com/alexanderzobnin/grafana-zabbix/issues/286)

## [3.5.1] - 2017-07-10

### Fixed

- Bug with alerting when template queries are used, [#424](https://github.com/alexanderzobnin/grafana-zabbix/issues/424)

## [3.5.0] - 2017-07-05

### Added

- rate() function, which calculates per-second rate for growing counters.
- Benchmarks for time series functions. Used [Benchmark.js](https://github.com/bestiejs/benchmark.js) library.

### Changed

- Template query format. New format is `{group}{host}{app}{item}`. It allows to use names with dot. Updated
  [templating docs](https://grafana.com/docs/plugins/alexanderzobnin-zabbix-app/latest/templating#query-format),
  [#254](https://github.com/alexanderzobnin/grafana-zabbix/issues/254)
- Update included dashboards. Add templated zabbix datasource and use it for all metrics.
- Improved performance of groupBy() functions (at 6-10x faster than old).
- Fill empty intervals by _null_ when aggregations are used, [#388](https://github.com/alexanderzobnin/grafana-zabbix/issues/388)

### Fixed

- Item name expanding when key contains commas in quoted params, like my_key["a=1,b=2",c,d]
- Incorrect points order when trends are used [#202](https://github.com/alexanderzobnin/grafana-zabbix/issues/202)
- Triggers panel styles for light theme
- Bug with text metrics when singlestat or table shows NaN, [#325](https://github.com/alexanderzobnin/grafana-zabbix/issues/325)

## [3.4.0] - 2017-05-17

### Added

- **Alerting**: highlight panel contained metrics with fired triggers.
- **Alerting**: add thresholds to panels from zabbix triggers.
- **Docs**: add docs for setAliasByRegex() from [@v-zhuravlev](https://github.com/v-zhuravlev)
- Support millisecond resolution on graphs. Patch from Jay Dawes <ajaxous@gmail.com>.
- Sum and count aggregations.
- Expand user macros in items [#212](https://github.com/alexanderzobnin/grafana-zabbix/issues/212)
- replaceAlias() function [#287](https://github.com/alexanderzobnin/grafana-zabbix/issues/287)
- Additional `Range` config option for trends [#364](https://github.com/alexanderzobnin/grafana-zabbix/issues/364)

### Changed

- Add template variables to dropdown metric list [#310](https://github.com/alexanderzobnin/grafana-zabbix/issues/310)
- Add all value regex `/.*/` to host dropdown.
- Replace native map() and forEach() methods by lodash.

### Fixed

- Templatig issue when no values returned [#354](https://github.com/alexanderzobnin/grafana-zabbix/issues/354)
- Add host name for multiple text metrics.
- Timeshift issue (Datapoints outside time range) for multiple targets with timeshift()
  , [#338](https://github.com/alexanderzobnin/grafana-zabbix/issues/338)

## [3.3.0] - 2017-02-10

### Added

- **Triggers panel**: allow to hide hosts in maintenance [#186](https://github.com/alexanderzobnin/grafana-zabbix/issues/186)
- **Triggers panel**: allow to change font size [#351](https://github.com/alexanderzobnin/grafana-zabbix/issues/351).
- **Triggers panel**: table pagination [#229](https://github.com/alexanderzobnin/grafana-zabbix/issues/229)
- **Triggers panel**: add 'enable scroll' control and page size input.

### Changed

- **Triggers panel**: rearrange options.

### Fixed

- Grunt: fix watch task.

## [3.2.1] - 2017-02-02

### Added

- **Docs**: add building instructions.
- setAliasByRegex() function

### Changed

- **Docs**: deprecate special repo with built plugins.
- **Triggers panel**: remove 'default' from datasources list (cause error), iss [#340](https://github.com/alexanderzobnin/grafana-zabbix/issues/340)
- Add dist/ directory to repo to correspond development guide http://docs.grafana.org/plugins/development/

### Fixed

- **Triggers panel**: metrics suggestion.
- **Triggers panel**: event acknowledge.
- **Triggers panel**: panel styles.
- **Query editor**: options styles.
- **Docs**: fixed timeShift() docs
- Error for new empty panel [#337](https://github.com/alexanderzobnin/grafana-zabbix/issues/337)
- Checking query for variables.

## [3.2.0] - 2017-02-02 [YANKED]

### Added

- timeShift() function [#307](https://github.com/alexanderzobnin/grafana-zabbix/issues/307)
