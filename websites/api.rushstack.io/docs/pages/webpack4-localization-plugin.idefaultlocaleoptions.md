---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@rushstack/webpack4-localization-plugin](./webpack4-localization-plugin.md) &gt; [IDefaultLocaleOptions](./webpack4-localization-plugin.idefaultlocaleoptions.md)

## IDefaultLocaleOptions interface

**Signature:**

```typescript
export interface IDefaultLocaleOptions
```

## Properties

| Property                                                                                                                | Modifiers | Type    | Description                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------- | --------- | ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [fillMissingTranslationStrings?](./webpack4-localization-plugin.idefaultlocaleoptions.fillmissingtranslationstrings.md) |           | boolean | <i>(Optional)</i> If this option is set to <code>true</code>, strings that are missing from <code>localizedData.translatedStrings</code> will be provided by the default locale |
| [localeName](./webpack4-localization-plugin.idefaultlocaleoptions.localename.md)                                        |           | string  | This required property specifies the name of the locale used in the <code>.resx</code>, <code>.loc.json</code>, and <code>.resjson</code> files in the source                   |