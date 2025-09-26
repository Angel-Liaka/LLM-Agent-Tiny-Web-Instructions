# [NAME] Testing v[X.Y.Z]

```
LEGEND: UNIT:unit-tests INT:integration E2E:end-to-end COV:coverage MOCK:mock-data
VARS: X:coverage-target Y:test-count Z:performance-threshold
```

## STRATEGY
```
UNIT:[X]% INT:[Y]% E2E:[Z]% TOTAL-COV:[X]% THRESHOLD:[fail-below-X]%
FRAMEWORK:[jest|mocha|vitest] RUNNER:[node|browser|both]
```

## UNIT TESTS
```
[module]/[function] → INPUT:[data] EXPECT:[result] MOCK:[dependencies]
[module]/[class] → SETUP:[instance] TEST:[method] ASSERT:[behavior]
```

## INTEGRATION TESTS
```
[featureA]+[featureB] → FLOW:[steps] VERIFY:[end-state] DATA:[fixtures]
[api]+[database] → REQUEST:[payload] RESPONSE:[expected] CLEANUP:[reset]
```

## E2E SCENARIOS
```
[user-journey] → STEPS:[action]→[action]→[result] VERIFY:[final-state]
[critical-path] → START:[condition] ACTIONS:[sequence] SUCCESS:[criteria]
```

## TEST DATA
```
FIXTURES:[file] SIZE:[X]kb TYPE:[json|sql|mock] CLEANUP:[auto|manual]
MOCKS:[service]→[mock-response] STUBS:[function]→[return-value]
```

## PERFORMANCE TESTS
```
LOAD:[X]users/[Y]sec → RESPONSE:[Z]ms MAX-MEMORY:[X]mb
STRESS:[breaking-point] SPIKE:[sudden-load] ENDURANCE:[duration]
```

## CI/CD PIPELINE
```
TRIGGER:[push|pr|schedule] RUN:[test-suite] FAIL:[threshold]% NOTIFY:[team]
STAGES: 1.unit→[X]min 2.integration→[Y]min 3.e2e→[Z]min
```

## COVERAGE RULES
```
REQUIRED:[X]% EXCLUDE:[generated|vendor] REPORT:[html|json|lcov]
MISSING:[critical-paths] IGNORED:[trivial-getters] ENFORCE:[ci-gate]
```

## DEBUG/TROUBLESHOOTING
```
FAILING:[test-name]→[debug-steps] FLAKY:[test]→[stabilization]
TIMEOUT:[increase-to-X]ms RETRY:[X]attempts ISOLATION:[parallel|serial]
```

## VALIDATION
```
✓all-features-covered ✓edge-cases-tested ✓performance-verified ✓ci-passing
```
