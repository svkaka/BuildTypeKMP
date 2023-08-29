# BuildType in Kotlin Multiplatform 

## Question
How do I configure different source sets for `debug` and `release` build types. I don't want to include debug only source files in release apk

having separate sources works on android with introducing `debug/release` directories look at [#92f084c](https://github.com/svkaka/BuildTypeKMP/commit/92f084cdb6b687f08bdcb0d6f8a4f281ae781d24)
```
common/src/debug/
common/src/release/
```

When running same configuration on iOS I get
```
../workspace/BuildTypes/common/src/commonMain/kotlin/com/example/common/App.kt:18:38 Unresolved reference: getBuildType
```
