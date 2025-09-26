# [NAME] Requirements v[X.Y.Z]

```
LEGEND: USER:user-type STORY:user-story AC:acceptance-criteria PRI:priority BIZ:business-value
VARS: X:story-count Y:sprint Z:effort-points
```

## USER TYPES
```
[PrimaryUser]:[description] GOALS:[objectives] PAIN:[current-problems]
[SecondaryUser]:[description] GOALS:[objectives] PAIN:[current-problems]
```

## EPICS
```
[EpicName] → VALUE:[business-benefit] USERS:[affected-types] SIZE:[X]stories
OUTCOME:[measurable-result] TIMELINE:[X]sprints DEPS:[other-epics]
```

## USER STORIES
```
[US001] AS:[user-type] WANT:[capability] SO:[benefit] PRI:[1-5] POINTS:[X]
AC: 1.[criteria] 2.[criteria] 3.[criteria]
DEV: [implementation-notes] TEST: [verification-approach]
```

## BUSINESS RULES
```
[RuleName] → CONDITION:[when] ACTION:[then] EXCEPTION:[unless]
PRIORITY:[critical|high|medium|low] OWNER:[stakeholder]
```

## CONSTRAINTS
```
LEGAL:[compliance-requirements] TECH:[platform-limits] BIZ:[budget-time]
PERFORMANCE:[response-time] CAPACITY:[concurrent-users] SECURITY:[standards]
```

## SUCCESS METRICS
```
[MetricName]:[current]→[target] METHOD:[measurement] TIMELINE:[when]
KPI:[key-indicator] BASELINE:[starting-point] GOAL:[end-state]
```

## ASSUMPTIONS
```
[AssumptionName] → ASSUMPTION:[what] RISK:[if-wrong] VALIDATION:[how-to-verify]
OWNER:[responsible] STATUS:[unverified|verified|invalid]
```

## OUT OF SCOPE
```
[FeatureName] → REASON:[why-excluded] MAYBE:[future-version] ALTERNATIVE:[workaround]
```

## DEPENDENCIES
```
EXTERNAL:[system]→[integration-required] INTERNAL:[team]→[coordination-needed]
DATA:[source]→[format] INFRASTRUCTURE:[requirement]→[provisioning]
```

## ACCEPTANCE
```
DEMO:[stakeholder] CRITERIA:[sign-off-requirements] SUCCESS:[definition-of-done]
```
