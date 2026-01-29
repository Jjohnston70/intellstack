# Shadow vs. Reality Quick Reference

The most important distinction in the framework. Shadows are representations of reality filtered through human reporting. Reality is direct measurement.

## Shadow Examples (What People Say)

| Shadow Variable | Why It's a Shadow |
|-----------------|-------------------|
| Deal stage in CRM | Sales rep's interpretation of where deal stands |
| Project status | PM's judgment call, often optimistic |
| Customer satisfaction score | Self-reported, subject to survey bias |
| Task completion % | Estimate, not measurement |
| Job status (open/in-progress/complete) | Manual update, often delayed |
| Lead quality score | Subjective assessment |
| Employee engagement rating | Self-reported |
| Inventory count (manual) | Point-in-time snapshot, immediately stale |

## Reality Examples (What Actually Happened)

| Reality Variable | Why It's Reality |
|------------------|------------------|
| Email timestamps | System-recorded, objective |
| GPS coordinates | Sensor data, continuous |
| Payment received date | Bank record, factual |
| Login timestamps | System log, automatic |
| Page view duration | Measured behavior |
| Call duration and frequency | Telecom records |
| Shipment scan events | Barcode/RFID capture |
| Sensor readings (temp, pressure, etc.) | Physical measurement |
| API response times | System-measured latency |
| File modification timestamps | Filesystem record |

## The Conversion Question

For every shadow variable, ask: "What reality could we measure instead?"

| Shadow | Reality Alternative |
|--------|---------------------|
| "Customer is interested" | Email response time < 24hrs, opened proposal doc |
| "Project on track" | Tasks completed vs. scheduled, commit frequency |
| "Employee is engaged" | Meeting attendance, response times, output volume |
| "Lead is qualified" | Budget confirmed in writing, decision timeline stated |
| "Job complete" | GPS at location + photo uploaded + signature captured |

## When Shadows Are Acceptable

Shadows aren't always bad. Use them when:
- Reality is impossible or impractical to measure
- The shadow is calibrated against reality periodically
- The cost of reality capture exceeds the value
- Human judgment genuinely adds information (expert assessment)

But be honest about what you're working with. A system built on shadows will always be less reliable than one built on reality.

## Red Flags

Your system is shadow-heavy if:
- Most data entry is manual
- Updates depend on someone "remembering to log it"
- You find out about problems from customer complaints
- Historical data doesn't match what people remember happening
- "The system says X but actually Y"

## The Physics Test

Ask: "Would this variable exist if no human reported it?"

- GPS location: Yes (satellite measures it)
- Deal stage: No (exists only because rep entered it)
- Payment timestamp: Yes (bank recorded it)
- Customer satisfaction: No (exists only because customer answered survey)
