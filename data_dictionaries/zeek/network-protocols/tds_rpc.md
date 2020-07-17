# TDS RPC Log

## Description

Metadata extracted from any [Tabular Data Stream](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-tds/b46a581a-39de-4745-b076-ec4dbb7d13ec) (TDS) traffic observed on TCP port 1433.

Three other logs produced with this event:
- [tds.log](./tds.md)
- [tds_sql_batch.log](./tds_sql_batch.md)

[Zeek Source](https://github.com/amzn/zeek-plugin-tds)

## Data Dictionary

| Standard Name                   | Field Name                      | Type                            | Description                            | Sample Value                    |
| ------------------------------- | ------------------------------- | ------------------------------- | -------------------------------        | ------------------------------- |
| src_ip_addr                     | id.orig_h                       | ip                              | The originating/source IP address      | `10.81.0.10`                    |
| src_port                        | id.orig_p                       | integer                         | The originating/source port            | `58972`                         |
| dst_ip_addr                     | id.resp_h                       | ip                              | The responding/destination IP address  | `10.81.0.11`                    |
| dst_port                        | id.resp_p                       | integer                         | The responding/destination port        | `1433`                          |
| @timestamp                      | ts                              | date_time                       | Timestamp for when the event happened. | `1352718180.395182`             |
| event_uid                       | uid                             | string                          | Unique ID for the connection           | `ClEkABC3m5giqnMf4h`            |
| TBD                             | procedure_name                  | string                          |                                        | ``                              |
| TBD                             | parameters                      | array_string                    |                                        | ``                              |

## Event JSON

```json
```