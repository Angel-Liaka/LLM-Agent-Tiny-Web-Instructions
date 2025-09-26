# [NAME] v[X.Y.Z]

```
LEGEND: TGT:target DEP:dependencies ARC:architecture CMP:compatibility SZ:size PRF:performance CD:code BR:browser M/S/C:Must/Should/Could L:lines
VARS: X:src-size Y:min-size Z:nesting-depth A/B/C:feature-refs
```

## SPECS
```
TGT:[size|perf|mem] DEP:[0|native|libs] ARC:[spa|lib|tool] CMP:[br|node|both]  
SZ:src[X]kb,min[Y]kb PRF:load[X]ms CD:files[X],func[Y]L,nest[Z]
```

## FEATURES
```
M:[critical-must-have] S:[important-should-have] C:[nice-could-have]
```

## USERS
```
WHO:[target-users] USE:[key-scenarios] WIN:[success-metrics]
```

## SECURITY
```
AUTH:[method] DATA:[encryption] EXPOSE:[endpoints] RISKS:[top-3-threats]
```

## ROADMAP
```
v[X.0]:[core-features]→[milestone-goal]
v[X.1]:[feature-set-A]→depends:[prev-features]
v[X.2]:[feature-set-B]→unlocks:[future-capability]
GOAL:[primary-objective] DEPS:feat[A]→feat[B]→feat[C] BLOCKS:[external-waiting]
```

## API
```js
fn(p:type):ret | Class{prop:type,method():type}
```

## FLOW
```
IN→[process]→OUT | [state]↔[comp]↔[dom]
```

## BUILD+ARCH+RULES
```
BUILD: 1.[core]→[files]→[est-lines] 2.[feat]→[files]→[est-lines]
ARCH: /src/[name].js[X]kb /dist/[name].min.js[Y]kb /test/[name].test.js
RULES: fn:pure[10]L events:delegate dom:direct state:minimal
```

## LIMITS
```
PRF:load[X]ms,render[Y]ms DEP:[list]|NONE
```

## VALIDATE
```
✓M-features ✓PRF[X]ms ✓deps[0] ✓cross-browser ✓compressed
```

## EDGE+TEST
```
ERR:[case]→[fix] FALL:[new]→[old] LIM:inp[X],comp[Y]
UNIT:[fn]→[in]→[out] INT:[feat]→[flow]→[res] BR:[c|f|s|e]→[p/f]
```

```
PROTOCOL: DOC→CODE→OPT→MEASURE→VALIDATE
SUCCESS: 100%feat+SZ[target]+0regress
```
