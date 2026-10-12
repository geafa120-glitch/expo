---
'expo-modules-jsi': patch
---

Fix objects autoreleased while a native state is released never being freed, which kept native objects such as `AVPlayer` alive after their shared object was released.
