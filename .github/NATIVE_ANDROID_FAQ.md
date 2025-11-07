# FAQ: Using BitooBitImageEditor with Native Android (Kotlin/Java)

## Can I use this library in my native Android Kotlin project?

**Short answer:** Not directly, but you have alternatives.

**Detailed answer:** BitooBitImageEditor is built on Xamarin.Forms, which requires the Xamarin/MAUI framework. Native Android Kotlin projects cannot directly consume Xamarin.Forms libraries without significant architectural changes.

## What are my options?

See the comprehensive guide: [KOTLIN_ANDROID_USAGE.md](../KOTLIN_ANDROID_USAGE.md)

**Quick recommendations:**

1. **Best option for native Android Kotlin:** Use a native library like:
   - [PhotoEditor](https://github.com/burhanrashid52/PhotoEditor) - Similar features, pure Android
   - [uCrop](https://github.com/Yalantis/uCrop) - Excellent cropping
   - [Android-Image-Cropper](https://github.com/CanHub/Android-Image-Cropper) - Modern, Kotlin-friendly

2. **If you must use BitooBitImageEditor:** Create a separate Xamarin.Android module or microservice

3. **Starting fresh?** Consider Xamarin.Forms or .NET MAUI for cross-platform development

## Feature comparison

| Feature | BitooBitImageEditor | PhotoEditor (Kotlin alternative) |
|---------|---------------------|----------------------------------|
| Platform | Xamarin.Forms | Native Android |
| Language | C# | Java/Kotlin |
| Text editing | ✅ | ✅ |
| Stickers | ✅ | ✅ |
| Drawing | ✅ | ✅ |
| Cropping | ✅ | ✅ |
| Filters | ❌ | ⚠️ Limited |
| APK size impact | ~15-20 MB (Xamarin runtime) | ~1-2 MB |

## Need more help?

Open an issue describing your specific use case, and we'll guide you to the best solution for your project.
