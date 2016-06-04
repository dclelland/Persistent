# Persist

Simple type safe persistable values to use as settings within your app.

Currently supports `Bool`, `Int`, `Float`, and `Double`.

✓ Easy interface

```swift

// Configutation
struct Settings {

    static var darkMode = Persistent(value: false, key: "darkMode")
    static var openCount = Persist(value: 0, key: "openCount")
    static var volume = Persist(value: 1.0, key: "volume")

}

// Setting
Settings.darkMode.value = true
Settings.openCount.value = Settings.openCount.value + 1

// Getting

print(Settings.darkMode.value) // true
print(Settings.openCount.value) // 1

```

✓ Easily extend other types

```swift
// TODO

```

### Todo:

- Strings
- Arrays (might have to wait for extensible generics)
- Dictionaries (might have to wait for extensible generics)