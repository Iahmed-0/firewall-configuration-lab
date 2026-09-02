# Firewall Configuration and Traffic Validation Lab

## Overview

This project documents the configuration and testing of inbound and outbound firewall rules. I defined intended traffic behaviour, applied firewall rules, tested allowed and blocked connections, and recorded configuration and troubleshooting results.

## Skills demonstrated

- Inbound and outbound firewall-rule configuration
- Protocol, port, source, destination, and direction analysis
- Allow-versus-block testing
- Rule matching, priority, profile, and scope review
- Network connectivity validation
- Structured troubleshooting and documentation

## Lab environment

Complete the table using only the platform and configuration you actually used.

| Component | Lab value |
| --- | --- |
| Firewall platform | [WINDOWS / LINUX / APPLIANCE / OTHER] |
| Platform version | [VALUE] |
| Protected system | [SANITIZED SYSTEM ROLE] |
| Test source | [SANITIZED LAB HOST] |
| Test destination | [SANITIZED LAB HOST OR SERVICE] |
| Network topology | [BRIEF SANITIZED DESCRIPTION] |

## Rule-design record

Replace the examples with your real lab rules. Do not publish sensitive addressing.

| Rule | Direction | Action | Protocol/port | Scope | Business or lab purpose |
| --- | --- | --- | --- | --- | --- |
| [RULE NAME] | Inbound | [ALLOW/BLOCK] | [VALUE] | [SANITIZED] | [PURPOSE] |
| [RULE NAME] | Outbound | [ALLOW/BLOCK] | [VALUE] | [SANITIZED] | [PURPOSE] |

## Implementation summary

1. Documented the starting firewall state and intended network behaviour.
2. Created inbound and outbound rules using the required direction, action, protocol, port, and scope.
3. Confirmed the relevant firewall profile or policy was active.
4. Tested permitted and denied traffic from the appropriate source and destination.
5. Compared expected and actual results and reviewed rule matching when behaviour differed.
6. Documented the final configuration and troubleshooting observations.

## Validation matrix

| Test case | Rule or condition | Expected result | Actual result | Evidence |
| --- | --- | --- | --- | --- |
| Baseline before change | [CONDITION] | [EXPECTED] | [ACTUAL] | [LINK] |
| Intended allowed traffic | [RULE] | Allowed | [ACTUAL] | [LINK] |
| Intended blocked traffic | [RULE] | Blocked | [ACTUAL] | [LINK] |
| Rule disabled or removed, if tested | [CONDITION] | [EXPECTED] | [ACTUAL] | [LINK] |
| Final state | [CONDITION] | [EXPECTED] | [ACTUAL] | [LINK] |

## Screenshots to add

- Starting firewall profile or status
- Inbound rule with sensitive fields redacted
- Outbound rule with sensitive fields redacted
- Successful allowed-traffic test
- Failed or timed-out blocked-traffic test
- Relevant sanitized event or firewall log entry

## Troubleshooting method

When traffic does not match the expected result, check the path in layers:

1. Confirm the application or service is running and listening.
2. Confirm addressing, routing, and basic reachability.
3. Confirm the rule direction and action.
4. Confirm protocol and port values.
5. Confirm source, destination, interface, program, user, or network scope.
6. Confirm the active firewall profile, chain, or policy context.
7. Check rule order or precedence when the platform uses it.
8. Review logs and repeat the same controlled test.

Document a real incident in `docs/troubleshooting-log-template.md`.

## Lessons learned

- [WHAT YOU LEARNED ABOUT INBOUND VERSUS OUTBOUND FILTERING]
- [WHAT YOU LEARNED ABOUT RULE SCOPE OR PRECEDENCE]
- [HOW LOGS OR CONTROLLED TESTS HELPED VERIFY BEHAVIOUR]

## Security note

Use only authorized lab systems. Do not publish production firewall exports, credentials, public addresses, sensitive internal topology, or logs containing confidential traffic data.
